This repository contains localization keys and documentation only. It does not contain the source code of MDWS.
## License
Localization keys and documentation in this repository may be used and contributed to for MDWS localization and documentation purposes.
This repository does not contain or license the source code, models, textures, or other assets of MoreDifficultWitherStorm.
## 前置与署名

本模组是 Cracker's Wither Storm Mod 的非官方附属模组，需要安装适用于 Minecraft 1.20.1 的 Cracker's Wither Storm Mod 4.2.1。

本项目与 Cracker's Wither Storm Mod 及其开发团队没有隶属、合作或官方认可关系，也不包含、分发或重新授权前置模组及其资源。

Cracker's Wither Storm Mod 由 nonamecrackers2 创作。请从[官方 CurseForge 页面](https://www.curseforge.com/minecraft/mc-mods/crackers-wither-storm-mod)下载前置模组。

## 模组特色

MoreDifficultWitherStorm 是一个围绕 Cracker's Wither Storm Mod 扩展玩法的附属模组。

本模组并不只是简单提高凋灵风暴的生命值、伤害等数值，而是通过新的挑战规则、阶段机制和特殊玩法扩展凋灵风暴的完整游戏体验。

玩家可以在创建世界或多人游戏中选择不同的挑战条件，通过承担额外风险获得更高的风暴点数，并面对更加危险、具有更明显阶段变化的凋灵风暴。

除此之外，本模组也在逐步加入不同于传统逃生玩法的扩展内容，例如让玩家以凋灵风暴的形态进行游戏，并体验成长、吞噬、牵引光束、副首攻击等与凋灵风暴相关的能力。
### 风暴逃生挑战

- 创建新世界时可以选择“风暴逃生”，进入专门的挑战规则面板。
- 开局玩家出生在 `(0, 0)`，获得受保护的护身符。
- 召唤凋灵风暴前，世界边界会限制在半径 15 的准备区域内。
- 准备阶段只能放置或破坏凋灵骷髅头，无法取用容器物品。
- 准备阶段玩家会保持满饥饿、满饱和度和抗性效果；召唤凋灵风暴后解除这些保护，并锁定雷暴。
- 支持风暴点数、游戏难度、复活次数、无敌时间等挑战条件。

### 强化模式与命令方块等级

强化模式下，凋灵风暴的命令方块会根据风暴点数升级：

- 低于 10 点：脉冲型命令方块。
- 达到 10 点：连锁型命令方块，需要更多攻击次数。
- 达到 20 点：循环型命令方块，会更频繁发射火焰凋灵导弹。
- 达到 40 点：彩虹命令方块，拥有更高最终攻击次数，并带来更危险的强化规则。

命令方块等级越高，凋灵风暴内部奖励箱的奖励也会更好。

### 凋灵风暴内部重力反转

- 在强化相关规则中，最终战攻击命令方块后可以触发凋灵风暴内部重力反转。
- 玩家、怪物和部分实体会受到反转重力影响。
- 已对视角、控制和部分实体表现做兼容处理，让重力反转更接近“挑战机制”，而不是单纯失控。

### 新物品与附魔扩展

- 附魔金苹果炖菜：以附魔金苹果为核心制作，效果比原版附魔金苹果更强，并提供对凋零病的长期保护方向。
- 腐败抑制剂：用于延缓凋零病死亡，适合前期缺少腐败物品时使用。
- 通用命令方块附魔书：可通过铁砧让可附魔物品获得“命令方块”相关强化。
- 拥有“命令方块”附魔的工具和护甲会获得额外攻击力或护甲值，并可参与针对命令方块实体的战斗规则。

### 结算界面

- 挑战成功、挑战失败、猎人胜利、放置方胜利等情况会进入专门结算界面。
- 结算会展示挑战模式、凋灵风暴类型、游戏难度、风暴点数、挑战用时和本局主要条件。
- 单人模式失败时会替换原版死亡界面，更像一次完整挑战的结束。

### 多人逃杀与猎人逃杀

多人玩法目前处于早期实现阶段，已经具备基础房间、身份和胜负逻辑：

- 多人逃杀：领队开房，其他玩家加入；领队死亡则游戏结束。
- 猎人逃杀：通过指令指定放置者，其他参赛者默认为猎人；放置者死亡则猎人胜利，放置者击败凋灵风暴则放置方胜利。
- 猎人逃杀：风暴化身：需要 Identity、Identity2 或 Woodwalkers 之一。可以指定一名玩家化身凋灵风暴，放置者召唤凋灵风暴时会替换为该玩家的风暴化身。

常用多人指令：

```mcfunction
/mdws multiplayer panel
/mdws multiplayer join
/mdws multiplayer identity summoner <玩家>
/mdws multiplayer identity wither_storm <玩家>
/mdws multiplayer identity status
/mdws multiplayer start
```

## 当前状态

本项目仍在开发中，部分内容属于实验性玩法，尤其是多人猎人定位、完整阵营 UI、风暴化身细节和更复杂的胜负条件仍可能继续调整。建议在正式游玩前备份存档。
