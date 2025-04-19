# WoW Classic (Vanilla) P5 熊T装备评分模型 | WoW Classic (Vanilla) Phase 5 Bear Tank Gear Scoring Model (v4.4)

![WoW Classic Logo](https://img.shields.io/badge/WoW%20Classic-Vanilla%20(1.12)-blue) ![Phase 5](https://img.shields.io/badge/Phase-P5%20(安其拉神庙)-purple) ![Guardian Druid](https://img.shields.io/badge/Class-Guardian%20Druid%20(Bear%20Tank)-orange) ![Version](https://img.shields.io/badge/Version-v4.4%20(2020.08.18)-brightgreen)

---

## Introduction

This project presents **Version 4.4**of an equipment scoring model for Bear Tanks (Guardian Druids) in World of Warcraft Classic (Level 60 Vanilla Era), specifically focused on**Phase 5 (Naxxramas)** content. The last update was on**August 18, 2020**.

Originally created and shared via **Shimo Docs**, this model aims to provide Bear Tank players in the later stages of Vanilla WoW (especially AQ and Naxx) with a quantitative tool to evaluate and compare gear. The core goal isto strike a balance between the complex demands of Survival (EHP - Effective Health Pool) and Threat (TPS - Threat PerSecond).

Following a recent request from a fellow player ("水友"), I decided to organize and**open-source** this document on GitHub for broader community access, use, and discussion.

## Background

In Vanilla WoW, especially within high-difficulty raids like Naxxramas, gearing a Bear Tank is highly challenging. Players must meticulously weigh survival stats (Stamina, Armor, Agility, Defense Skill, Dodge, etc.) against threat stats (Strength, Agility, Hit, Crit, AP, Weapon Procs, etc.) from a limited yet diverse gear pool. This model attempts to:

1.**Quantify Stat Values**: Assign relative scores to various stats based on a mathematical model.
2.**Balance Survival & Threat**: Introduce the concept of a "Threat-Survival Weight" (`p`) allowing users to adjust scoring emphasis based on their role (e.g., Main Tank, Off-Tank) orspecific boss encounters.
3.**Consider Spike Damage**: Since v4.2, the model incorporates considerations for "spike damage," placing more emphasis on stats that contribute to smoother health pools.
4.**Support Decision Making**: Provide intuitive score comparisons to aid in building Best-in-Slot (BiS) lists.

## Core Model & Methodology (v4.4)

***Core Metrics**: The model quantifies gear based on its contribution to**Effective Health Pool (EHP)**and**Threat PerSecond (TPS)**.
***Threat-Survival Weight (`p`)**: A key adjustable parameter representing how much EHP valueis considered equivalent to a 1% TPS increase.
    *   `p=1`: Treats 1% EHP increase and1% TPS increase as equally valuable (relatively balanced or threat-leaning).
    *   `p=5`: Considers a 5% EHP increase equivalent to a 1% TPS increase (prioritizes survival, suitable for high-pressure situations or "turtle" playstyles).
    *   The model likely provides multiple scores based on different `p` values (e.g., Balanced Score, Turtle Score, Feral Score) to suit various scenarios and player preferences.
***Spike Damage Consideration**: Weights of certain stats (like Stamina, Armor) are adjusted to reflect their importance in mitigating sudden bursts of high damage.
***Score Calculation**: Utilizes complex formulas (detailed in the model file) toconvert gear stats, set bonuses, and potentially enchants/gems into comparable scores.
***Baseline Environment (v4.4 Reference)**: Scoring may be based onspecific assumed conditions:
    *   Talents: Standard Bear Tank spec (e.g., 11/33/7)
    *   Scenario: TAQ/NAXX Boss fights
    *   Raid Buffs: Common world/raid buffs like Spirit of Zandalar, Dire Maul Tribute, Songflower Serenade, Power Word: Fortitude, Prayer of Spirit, Mark of the Wild, etc.
    *   Consumables: Elixir of the Mongoose, Spirit of Zanza, Greater Stoneshield Potion, Dirge's Kickin' Chimaerok Chops, Gordok Green Grog, etc.
***Score Additivity**: Scores for different items in the same slot are directly comparable. Scores for enchants, buffs, and consumables are also calculated based on their EHP/TPS contributions and can theoretically be added to gear scores to measure total improvement, but are mainly used forlike-for-like comparisons.

For detailed scoring rules, attribute weights, calculation formulas, and scores for individual items, please refer to the core model file within this repository:

**[Current Phase (P5) Bear Tank Gear Score.xlsx](ranking/当前阶段(P5)熊T装备评分.xlsx)**

## How to Use

1.**Clone or download** this repository to your local machine.
    ``bash     git clone https://github.com/lamueno/classicDruid.git     ``
    Or simply click "Code" -> "Download ZIP" on the repository page.
2.**Locate andopen** the core model file ([`Current Phase (P5) Bear Tank Gear Score.xlsx`](ranking/当前阶段(P5)熊T装备评分.xlsx)). This is a spreadsheet file located in the `ranking` directory and requires software like Microsoft Excel, Google Sheets, or LibreOffice Calc.
3.**Consult the Model**: Understand the scores under different weight configurations (Balanced, Turtle, Feral, etc.) andcheck the scores for individual items.
4.**Apply and Compare**: Use the scores to evaluate gear you own or plan to acquire. Choose the appropriate weighting standard (`p` value) based on your team's needs and personal playstyle.
5.  **Note**: The model is built on specific assumptions and theories. Actual performance can be influenced by fight complexity, raid composition, individual skill, etc. Use it as a guide alongside your own experience.

## Change History

Please refer to the **[CHANGELOG.md](CHANGELOG.md)** file for a detailed update history.

## Contributing

While this model was last updated in 2020 for the now concluded Classic Era P5, if you have any thoughts, corrections, or find errors regarding its theory, data, or presentation, feel free to discuss via:

* **Submitting an Issue**: Raise questions or suggestions on the [Issues](https://github.com/lamueno/classicDruid/issues) page of this repository.
* **Submitting a Pull Request**: Fork this repository (`https://github.com/lamueno/classicDruid/fork`), make your changes on your own branch, and then create a Pull Request to merge your changes back.

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

* Thanks to the **fellow player ("水友")** whose private message prompted this open-source release.
* Thanks to all the players on the **NGA forums and Shimo Docs** who followed, used, discussed, and provided feedback during **2019-2020**.
* Thanks to **Blizzard Entertainment** for creating World of Warcraft.

---

May this resource from the past be helpful to those who need it! ʕ•ᴥ•ʔ
