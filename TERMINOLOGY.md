# 术语对照与校对说明

校对日期：2026-10-29。

依据：《怒火与荣耀2E总规则》0.2，译者：青甘甬宁战棋俱乐部。
以下页码均为这份 416 页 PDF 在阅读器中的页序，从封面计第 1 页，
不是正文中的“详见第 X 页”交叉引用。正文的引用页码与本 PDF 的实际页序并不一致。

本表列出与旧版模组不同的主要规则译名。译名差异不全是误译；为便于玩家对照规则书，
本次统一采用该 PDF 的用词。双语条目继续保留其英文部分，下表为便于阅读主要列出中文。

## 优先修正的混淆与误译

| 英文术语 | 旧译名 | 现译名 | PDF 页序 | 代表性 JSON 键 | 理由 |
| --- | --- | --- | --- | --- | --- |
| Resilience | 坚韧 | 抗性 | 33 | `HEADER.RESILIENCE`、`HEADER.RES` | 区分属性 Toughness；抗性用于减免伤害。 |
| Wrath Critical | 愤怒要点 | 怒火暴击 | 158 | `CHAT.WRATH_CRITICAL_TITLE` | 指怒火骰掷出 6 的特殊结果。 |
| Complication | 并发症 | 异变 | 158、355 | `ABILITY_TYPE.COMPLICATION` | 指检定中的叙事意外，不是医学并发症。 |
| Wrath Complication | 怒火并发症 | 怒火异变 | 158 | `CHAT.WRATH_COMPLICATION_TITLE` | 同上。 |
| Mutation | 异变 | 变异 | 322 | `TYPES.Item.mutation`、`ROLL.MUTATION` | 与 Complication 区分。 |
| Force | 力场 | 灵能 | 208 | `TRAIT.Force` | 指引导灵能的武器特性。 |
| Power Field | 动力场 | 力场 | 248 | `TRAIT.PowerField` | 指护甲的能量屏障特性，与 Force 区分。 |
| Full / Full-Round Action | 完整动作 | 全回合动作 | 174 | `ACTIVATION.FULL` | 表明动作所占用的回合资源。 |
| Invulnerable | 不易受损 | 特殊保护 | 247 | `ARMOUR.INVULNERABLE` | 专指 AP 不会降低抗性的护甲规则。 |
| Rare | 珍惜 | 稀有 | 205 | `RARITY.RARE` | “珍惜”用字错误，且需统一稀有度等级。 |
| Very Rare | 极珍惜 | 罕见 | 205 | `RARITY.VERY_RARE` | 同上。 |
| Cumbersome | 笨重 | 不便 | 248 | `TRAIT.Cumbersome` | 区分武器特性 Unwieldy（笨重）。 |

上述规则名也同步用于检定按钮、聊天提示、自动计算选项及 `WH.Models.*` 字段标签。
修改按英文键名区分含义，未把所有“坚韧”或“异变”一律替换。

## 角色与技能

| 英文术语 | 旧译名 | 现译名 | PDF 页序 | 代表性 JSON 键 |
| --- | --- | --- | --- | --- |
| Tier | 阶级 | 位阶 | 13 | `ADVANCE.TIER`、`ARCHETYPE.TIER` |
| Archetype | 原型 | 职业 | 15、81 | `TYPES.Item.archetype`、`BIO.ARCHETYPE` |
| Archetype Ability | 原型能力 | 职业能力 | 84 | `ARCHETYPE.ABILITY` |
| Faction | 派系 | 阵营 | 15、21 | `TYPES.Item.faction`、`BIO.FACTION` |
| Ascension | 晋升 | 位阶晋升 | 144 | `TYPES.Item.ascension` |
| Talent | 天赋 | 天赋专长 | 2、19、82 | `TYPES.Item.talent`、`HEADER.TALENT` |
| Wargear | 装备 | 战争装备 | 15、36 | `ARCHETYPE.WARGEAR`、`TITLE.WARGEAR` |
| Augmetic | 植入体 | 义体 | 263 | `TYPES.Item.augmentic`、`HEADER.AUGMETIC` |
| Fellowship | 社交 | 魅力 | 115 | `ATTRIBUTE.FELLOWSHIP` |
| Determination | 坚定 | 毅力 | 33、194 | `HEADER.DETERMINATION`、`ROLL.DETERMINATION` |
| Wounds | 伤势 | 承伤 | 33、190 | `HEADER.WOUNDS`、`CHAT.WOUNDS` |
| Memorable Injury | 难忘伤害 | 濒死损伤 | 192 | `TYPES.Item.memorableInjury` |
| Traumatic Injury | 创伤性伤害 | 重创 | 192、193 | `TYPES.Item.traumaticInjury` |
| Passive Awareness | 被动察觉 | 被动警觉 | 34、176 | `HEADER.PASSIVEAWARENESS` |
| Stealth Score | 潜行分 | 潜行值 | 176 | `HEADER.STEALTH_SCORE` |
| Athletics | 运动 | 体能 | 116 | `SKILL.ATHLETICS` |
| Ballistic Skill | 弹道技能 | 射击 | 116 | `SKILL.BALLISTIC_SKILL` |
| Cunning | 狡诈 | 狡猾 | 116 | `SKILL.CUNNING` |
| Insight | 洞悉 | 洞察 | 117 | `SKILL.INSIGHT` |
| Leadership | 领导 | 领导力 | 118 | `SKILL.LEADERSHIP` |
| Persuasion | 劝说 | 说服 | 119 | `SKILL.PERSUASION` |
| Psychic Mastery | 灵能掌握 | 灵能精通 | 120 | `SKILL.PSYCHIC_MASTERY` |
| Weapon Skill | 武器技能 | 格斗 | 121 | `SKILL.WEAPON_SKILL` |

`Fellowship` 的界面简称相应由“社”改为“魅”。
`Gear` 作为物品分类及装备页签改为“装备”；通用的 Foundry `Item` 仍译“物品”。

## 骰子、战斗与灵能

| 英文术语 | 旧译名 | 现译名 | PDF 页序 | 代表性 JSON 键 |
| --- | --- | --- | --- | --- |
| Icon | 标记 | 标识 | 153、154 | `CHAT.ICONS`、`EDIT.ICONS` |
| Exalted Icon | 昂升标记 | 卓越标识 | 154 | `CHAT.WRATH_CRITICAL_PSY` |
| Shift / Shifting | 转化 | 灵活调用 | 160、161 | `BUTTON.SHIFT`、`CHAT.SHIFTING` |
| Penalty | 减值 | 惩罚 | 156 | `DIALOG.PENALTY` |
| Simple Action | 简易动作 | 简单动作 | 173 | `ACTIVATION.SIMPLE` |
| Called Shot | 精确射击 | 精准射击 | 183 | `WEAPON.CALLED_SHOT` |
| Seize the Initiative | 夺取先攻 | 抢占先手 | 171 | `COMBAT.SEIZE` |
| Annihilation | 歼灭 | 湮灭 | 356 | `ABILITY_TYPE.ANNIHILATION` |
| Mob | 群体 | 集群 | 202、358 | `THREAT.MOB` |
| Average (Size) | 常规 | 普通 | 188 | `SIZE.AVERAGE` |
| Blinded | 目盲 | 失明 | 198 | `CONDITION.Blinded` |
| Hindered | 阻碍 | 妨碍 | 199 | `CONDITION.Hindered` |
| On Fire | 着火 | 燃烧 | 199 | `CONDITION.OnFire` |
| Pinned | 牵制 | 压制 | 199 | `CONDITION.Pinned` |
| Perils of the Warp | 亚空间威胁 / 亚空间危害 | 亚空间灾厄 | 287、288 | `TABLE.PERILS_OF_THE_WARP`、`TableSetting.perils` |
| Bound | 受缚 | 束缚 | 285、286 | `PSYCHIC_POWER.BOUND` |
| Unbound | 解缚 | 无缚 | 285、286 | `PSYCHIC_POWER.UNBOUND` |
| Transcendent | 超越 | 超凡 | 285、286 | `PSYCHIC_POWER.TRANSCENDENT` |
| Power Level | 灵能等级 | 能量强度等级 | 285、286 | `DIALOG.POWER_LEVEL` |
| Potency | 效能 | 威能等级增幅 | 292、293 | `PSYCHIC_POWER.POTENCY`、`SHIFT.POTENCY` |
| Activation (psychic power) | 激活 | 激活动作 | 292 | `PSYCHIC_POWER.ACTIVATION` |
| Range (psychic power) | 射程 | 作用范围 | 292 | `PSYCHIC_POWER.RANGE` |

`Potency` 的依据是灵能格式与消耗卓越标识的强化说明；PDF 此处未保留英文标题，
其作用与系统对应字段相同。灵能增幅提示中的“超载”也改用“威能等级增幅”，
避免与武器 `Supercharge`（过载）混淆。

战斗异变表、异变后果表的名称分别依据 PDF 第 189、158 页。
掩护标签统一使用第 176 页的“掩体”：界面的 `Half Cover` / `Full Cover` 分别为“半掩体” / “全掩体”，
这是依据规则用词组合的界面标签，PDF 未逐字列出这两个英文名称。

## 武器、护甲与稀有度

| 英文术语 | 旧译名 | 现译名 | PDF 页序 | 代表性 JSON 键 |
| --- | --- | --- | --- | --- |
| Armour Rating | 等级 | 护甲等级 | 246 | `ARMOUR.RATING` |
| Traits | 特征 | 特性 | 206、246 | `WEAPON.TRAITS`、`ARMOUR.TRAITS` |
| Salvo | 齐射 | 射速 | 206 | `WEAPON.SALVO` |
| Combi Weapon | 组合武器 | 复合武器 | 240 | `WEAPON.COMBIWEAPON` |
| Long Range | 远程 | 长程 | 206 | `RANGE.LONG` |
| Agonising | 痛苦 | 剧痛 | 207 | `TRAIT.Agonising` |
| Inflict (Condition) | 造成（状态） | 施加（状态） | 209 | `TRAIT.Inflict` |
| Parry | 架招 | 格挡 | 210 | `TRAIT.Parry` |
| Rending | 撕裂 | 破甲 | 210、211 | `TRAIT.Rending` |
| Silent | 无声 | 消音 | 211 | `TRAIT.Silent` |
| Spread | 扩散 | 散射 | 211 | `TRAIT.Spread` |
| Bulk | 重量 | 沉重 | 248 | `TRAIT.Bulk` |
| 'Ere We Go! | 俺们走！ | 俺们上！ | 248 | `TRAIT.EreWeGo` |
| Powered | 驱动 | 动力 | 248 | `TRAIT.Powered` |
| Common | 常见 | 普通 | 205 | `RARITY.COMMON` |
| Uncommon | 罕见 | 少有 | 205 | `RARITY.UNCOMMON` |

稀有度完整顺序为：普通（Common）、少有（Uncommon）、稀有（Rare）、罕见（Very Rare）、唯一（Unique）。

## PDF 内部存在多种译法时的取舍

| 术语 | 本模组采用 | 依据与取舍 |
| --- | --- | --- |
| Tier | 位阶 | 第 13 页定义为“游戏位阶”；部分后文写“阶位”。本次依用户指示，以 PDF 覆盖此前的“阶级”。 |
| Resilience | 抗性 | 第 33 页定义标题；部分例文写“韧性”，不采用。Toughness 仍为“坚韧”（第 114 页）。 |
| Determination | 毅力 | 第 194 页专节标题；同页流程及第 198 页出现“意志检定”，不沿用，以免与 Willpower 混淆。 |
| Shock | 震慑 | 第 193 页专节标题；第 33 页另有“精神值”“精神震慑值”。保留模组现有“震慑”。 |
| Mortal Wounds | 致命伤 | 第 190 页标题；正文也有“致命承伤”。保留现有“致命伤”。 |
| Memorable Injury | 濒死损伤 | 第 192 页定义与表名；第 127、138 页另有“标志伤疤”“标志伤痕”。 |
| Icon / Exalted Icon | 标识 / 卓越标识 | 第 153、154 页掷骰定义；其他段落也出现“标记”“卓越标记”。 |
| Shift | 灵活调用 | 第 160 页定义；装备及灵能段落另有“灵活调整”“转移”“转化”。承伤转为震慑的普通动词“转化”仍保留。 |
| Blast | 爆炸 | 第 208 页特性标题；同页表格另写“爆破”。保留“爆炸Blast”。 |
| Bound | 束缚 | 第 285 页表格及第 286 页小节；第 287 页个别示例写“缚定”。 |
| Perils of the Warp | 亚空间灾厄 | 第 287 页标题及第 288-290 页表名；个别示例写“亚空间灾变”。 |
| Salvo | 射速 | 第 206 页武器参数定义；后面的敌人说明也出现“齐射选项”。 |
| Talent | 天赋专长 | 第 2 页章节标题及第 19、82 页说明；其他段落也简称“天赋”。 |

其余已一致的词汇，如力量、坚韧、敏捷、反应、意志、智力、警觉、欺诈、威吓、调查、医疗、驾驶、
学识、潜行、生存、科技、信念、决心、怒火、荣耀、毁灭、爆炸、热熔，沿用现有译名。
PDF 未覆盖的载具扩展特性及系统管理功能不据此推定为误译。

## 同步校验与补漏

本次依据本地 Wrath & Glory 系统 8.2.0 的英文语言文件核对文本键。
这仅是语言数据核对，不代表已完成 Foundry 界面或全部系统功能的兼容性实测。

校验结果：更新 158 条现有文本，补全 7 条新文本；中英文均为 692 个键，
无缺失键、额外键或变量占位符差异。原有双语术语中的英文部分全部保留。

- 修正 `CHAT.STEALTH_RESULT`：将被误译的变量 `{潜行}` 恢复为 `{stealth}`，使其能接收系统传入的潜行数值。
- 补全 `ARCHETYPE.SUGGESTED_POWERS`：推荐灵能（PDF 第 94 页）。
- 补全 `WH.Models.psychicPower.FIELDS.discipline.label`：灵能学科（PDF 第 280 页）。
- 补全 `WH.Trigger.ShiftDice`：灵活调用骰子，以第 160 页术语命名系统事件。
- 补全 `WEAPON.CALLED_SHOT_BYPASS`：破甲射击（PDF 第 183 页）。
- 补全 `WEAPON.SURPRISE`：突袭（PDF 第 176 页）。
- 补全 `DIALOG.CHOOSE_ACTOR`：选择角色；`WH.Trigger.Targeted`：被选为目标。这两项是系统界面用语。
- 同步灵能增幅说明中的 `test.dn` 示例，并闭合原本缺失的 HTML 列表结束标签。
- 翻译原有自动计算标签、仅对护甲应用 AP 的残留英文提示；保留既有完整双语术语的英文部分。

本次不调整系统规则、数值、模块版本或兼容性声明；不修改已导入世界中的角色、物品、日志和表格名称。
