# 更新日志 | Change Log

本文档记录了 "当前阶段(P5)熊T装备评分" 模型的主要变更历史。
This document records the main change history of the "Current Phase (P5) Bear Tank Gear Score" model.

## [v4.4] - 2020/08/18

*   模型更新到v4.4，平衡了「最大有效生命」和「残存有效生命」的关系。
    *   Model updated to v4.4, balancing the relationship between "Max Effective Health" and "Remaining Effective Health".
*   增加：[P5]其拉守护者坠饰
    *   Added: [P5] Qiraji Guardian's Pendant

## [v4.3] - 2020/08/11 & 2020/08/13

*   修正：[P5]固化异种虫皮手套 耐力属性
    *   Corrected: [P5] Gauntlets of Steadfast Determination Stamina value.
*   模型更新到v4.3，采用了二次圆桌的击中模型。
    *   Model updated to v4.3, adopting a "secondary attack table hit model".
*   增加：多个TAQ掉落戒指
    *   Added: Several AQ drop rings.
*   更新P5推荐配装
    *   Updated P5 recommended gear set.

## [v4.2] - 2020/04/15 - 2020/05/18

*   **2020/05/18**: 增加：多个副手物品 (Added: Several off-hand items)
*   **2020/05/12**: 增加：[P5]堕落神明披风、[P1.5]艾斯卡达尔的毛皮 (Added: [P5] Cloak of the Fallen God, [P1.5] Eskhandar's Pelt)
*   **2020/05/11**: 增加：[P4]风矛斗篷 (Added: [P4] Cape of the Black Baron)
*   **2020/05/07**: 增加：[P4]原始蝙蝠皮外套 (Added: [P4] Primal Batskin Jerkin)
*   **2020/05/06**: 增加：多个主动类饰品 (Added: Several on-use trinkets)
*   **2020/04/23**:
    *   模型更新到v4.2：考虑了尖峰伤害，并完善了场景profile。现在耐力属性会更加重要，并增加了赞扎之魂作为默认buff。
        *   Model updated to v4.2: Considered spike damage and improved the scenario profile. Stamina is now more important, and Spirit of Zandalar is added as a default buff.
    *   评分改动：增加了boss战和小怪战的独立评分，团本场景依然为BWL。目前各战斗数据为手工收集，后续考虑写wcl爬虫以确保数据公允。
        *   Scoring changed: Added separate scores for boss fights and trash fights, raid scenario remains BWL. Battle data currently collected manually, considering a WCL scraper for future data accuracy.
    *   增加：一系列自然抗装备，以备战P5。
        *   Added: A series of Nature Resistance gear in preparation for P5.
*   **2020/04/15**:
    *   更新模型v4：重写了技能比例，引入怒气机制，能体现各项防御属性的负仇恨收益。
        *   Updated Model v4: Rewrote skill ratios, introduced rage mechanics, reflecting the negative threat impact of various defensive stats.
    *   考虑白字偏斜和暴击上限问题。
        *   Considered glancing blows and crit cap issues.
    *   已知问题：需要进一步细化AttackTable，考虑白字偏斜和暴击上限问题。
        *   Known Issue: AttackTable needs further refinement, considering glancing blows and crit cap.

## [v3.0 & P4 additions] - 2020/03/04 - 2020/04/05

*   **2020/04/05**:
    *   修改评分系统：原综合分修改为「均分得分」，同时新增「乌龟得分」（仇恨/生存=0.25）与「疯狗得分」（仇恨/生存=5）。
        *   Revised scoring system: Original composite score changed to "Balanced Score", added "Turtle Score" (Threat/Survival=0.25) and "Feral Score" (Threat/Survival=5).
    *   增加：[P4]龙牙饰物、多个T2.5部件。
        *   Added: [P4] Drake Fang Talisman, several T2.5 pieces.
    *   已知缺失物品：大地之击、虫群卫士徽章、梦境之末、谴责者、支配披风
        *   Known missing items: Earthstrike, Badge of the Swarmguard, Shroud of Infinite Mystery, The Hungering Cold, Cloak of Dominion
*   **2020/04/01**: 增加：「基础属性」和「权重评价」sheet (Added: "Base Stats" and "Weight Evaluation" sheets)
*   **2020/03/31**: 完全重写模型，目前版本v3.0。同时更新了评价基准。(Complete model rewrite, current version v3.0. Updated evaluation baseline.)
*   **2020/03/07**: 增加：附魔披风-强效抗性、哨兵/护卫的蜥蜴皮裤、阿拉希声望物品、NAXX部分掉落 (Added: Enchant Cloak - Greater Resistance, Sentinel/Outrider's Lizardhide Pants, Arathi Basin rep items, some Naxx drops)
*   **2020/03/04**: 增加：[P4]龙刺裹布 (Added: [P4] Dragon's Touch)

## [v2.x & P3 additions] - 2020/02/20 - 2020/03/03

*   **2020/03/03**:
    *   修正了生存模型，目前版本v2.2。主要改动：考虑了灵感buff的覆盖，提升了护甲及敏捷的生存分；根据BWL伤害环境，考虑了火焰、暗影伤害。
        *   Corrected survival model, current version v2.2. Main changes: Considered Inspiration buff uptime, increased survival score from Armor and Agility; considered Fire/Shadow damage based on BWL environment.
    *   增加：[P5]隐没秘密披风、牛王之皮、火焰抗性之灰烬护臂、火焰抗性之熔渣护手、地穴行者护腿、[P5]青铜龙军团的徽记之戒 (保护者之路)
        *   Added: [P5] Cloak of Concealment, Hide of the Wild, Fire Resist Bracers/Gloves, Cryptstalker Legguards, [P5] Signet Ring of the Bronze Dragonflight (Protector's path)
*   **2020/02/29**: 增加：多个zug掉落 (Added: Several ZG drops)
*   **2020/02/28**: 增加：肩部附魔sheet (Added: Shoulder enchant sheet)
*   **2020/02/26**:
    *   增加：武器附魔Sheet、普瑞斯托的阴谋饰物、火喉披风、飞龙披风、芬克的熔岩挖掘器
        *   Added: Weapon Enchant Sheet, Prestor's Talisman, Firemaw's Clutch, Onyxia Scale Cloak, Finkles Lava Dredger
    *   修正了仇恨模型，目前版本v2.1
        *   Corrected threat model, current version v2.1
*   **2020/02/21**: 增加：参考配装sheet (Added: Reference gear set sheet)
*   **2020/02/20**: 增加：强者斗篷、飞龙披风、迅击戒指、R12-R13军阶套装 (Added: Puissant Cape, Onyxia Scale Cloak, Quick Strike Ring, R12-R13 PvP sets)

## [v2.0 & Pre-P3] - 2019/10/24 - 2020/01/07

*   **2020/01/07**: 增加：Buff与药剂评分 (Added: Buff and consumable scores)
*   **2019/12/10**: 更新：R7-R10军阶套装 (Updated: R7-R10 PvP sets)
*   **2019/12/09**: 增加：奥山声望物品 (Added: Alterac Valley reputation items)
*   **2019/12/05**: 更新v2.0模型数据 (Updated v2.0 model data)
*   **2019/11/05**: 增加：魔皮软帽、征服者勋章、敏捷之暗月卡牌、赞达拉占卜师护腕、巨狼皮靴、殉难者的意志 (Added: Devilsaur Gauntlets, Conqueror's Spaulders, Darkmoon Card: Agility, Zandalar Haruspex's Bracers, Timbermaw Brawlers, Will of the Martyr)
*   **2019/10/30**:
    *   附魔：全部更新完成。武器部分附魔详见「双手」页面。(Enchants: All updated. Weapon enchants detailed on "Two-Hand" page.)
    *   增加：麦格尼的意志 (Added: Might of Menethil)
    *   开始更新附魔：头腿附魔 (Started updating enchants: Head/Leg enchants)
*   **2019/10/29**: 增加：防御之阿塔莱护手、强制者手套 (Added: Atal'ai Gloves of Defense, Force Reactive Disk) / 完成了饰品点评 (Completed trinket reviews)
*   **2019/10/27**: 增加：耐力之阿塔莱肩甲、迅影手套 (Added: Atal'ai Spaulders of Stamina, Shadowcraft Gloves)
*   **2019/10/25**:
    *   修正：阿格曼奇之戒属性和评价，紧绷的龙皮护肩的属性
        *   Corrected: Archimtiros' Ring stats and evaluation, Taut Dragonhide Shoulderpads stats
    *   增加：南风头盔、浴血面具、克苏恩印记、屠龙大师勋章、流沙坠饰、邪恶复仇衬肩、几丁质护肩、强烈仇恨披风、金巢披风、中士的斗篷、厚重异种虫胸甲、处决者的外衣、猥琐者咽喉护腕、固化异种虫皮手套、野熊之熔渣护手、雄鹰之熔渣护手、厚重其拉腰带、前锋之靴、维克洛尔大帝之戒、青铜龙军团的徽记之戒（征服者之路）、屠龙大师之戒、阿基迪罗斯的清算之戒、无息指环、源力之环、禁锢之戒、雷暴护肩、纳特·帕格的超级钓鱼靴、埃其亚基的皮、奥术师衬肩、黑龙束带
        *   Added: Helm of the South Wind, Mask of the Unforgiven, Seal of C'Thun, Mark of the Champion, Choker of the Shifting Sands, Mantle of Wicked Revenge, Chitinous Shoulderguards, Cloak of Concentrated Hate, Golden Mantle of the Dawn, Sergeant's Cloak, Thick Silithid Chestguard, Executioner's Garb, Wristguards of Gargantuan Grip, Gauntlets of Steadfast Determination, Slag Bearer's Gauntlets (Bear), Slag Bearer's Gauntlets (Eagle), Thick Qirajihide Belt, Boots of the Vanguard, Ring of Emperor Vek'lor, Signet Ring of the Bronze Dragonflight (Conqueror's path), Mark of the Dragon Lord, Band of Accuria, Ring of Unspoken Names, Band of Elemental Fury, Ring of Binding, Storm Pylon Shoulders, Nat Pagle's Extreme Anglin' Boots, Hide of Echtheachy, Arcanist Mantle, Onyxia Hide Belt
    *   增加了饰品点评 (Added trinket reviews)
*   **2019/10/24**: 从NGA迁移，本文档初始始化 (Migrated from NGA, document initialized)