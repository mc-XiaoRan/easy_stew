# Easy Stew

![Minecraft Java Edition 1.21.4 – 1.21.11](https://img.shields.io/badge/Minecraft%20Java-1.21.4%20%E2%80%93%201.21.11-green)
![Minecraft Java Edition 26.1 – 26.2](https://img.shields.io/badge/Minecraft%20Java-26.1%20%E2%80%93%2026.2-green)
![Environment](https://img.shields.io/badge/environment-datapack-orange)
![License MIT](https://img.shields.io/badge/license-MIT-blue)

Any two mushrooms can craft mushroom stew and suspicious stew, and both stews now stack up to 64.
任意两个蘑菇即可合成蘑菇煲和谜之炖菜，两者堆叠上限提升至 64。

[Modrinth](https://modrinth.com/datapack/easy_stew) · [Issues](https://github.com/mc-XiaoRan/easy_stew/issues)

---

## What it changes / 功能说明

| Recipe / 配方 | Vanilla / 原版 | Easy Stew / 本数据包 |
| --- | --- | --- |
| Mushroom stew / 蘑菇煲 | 1 red + 1 brown mushroom + bowl | **any 2 mushrooms** + bowl |
| 蘑菇煲 | 棕蘑菇、红蘑菇各 1 个 + 碗 | **任意 2 个蘑菇** + 碗 |
| Suspicious stew / 谜之炖菜 | 1 red + 1 brown mushroom + bowl + flower | **any 2 mushrooms** + bowl + flower |
| 谜之炖菜 | 棕蘑菇、红蘑菇各 1 个 + 碗 + 花 | **任意 2 个蘑菇** + 碗 + 花 |
| Stack size / 堆叠上限 | 1 | **64** |
| 堆叠上限 | 1 | **64** |

`Any two mushrooms` means the pack reads the `#minecraft:mushrooms` item tag, so any two items in that tag work — red + red, brown + brown, or one of each.
「任意 2 个蘑菇」指数据包读取 `#minecraft:mushrooms` 物品标签，标签内任意 2 个都能用——红+红、棕+棕，或各 1 个都可以。

### Flower effects / 花的效果

Suspicious stew keeps the vanilla effects, one flower per effect.
谜之炖菜保持原版效果，一朵花对应一种效果。

| Flower / 花 | Effect / 效果 |
| --- | --- |
| Allium / 绒球葱 | Fire Resistance 3s / 抗火 3 秒 |
| Azure Bluet / 蓝花美耳草 | Blindness 11s / 失明 11 秒 |
| Blue Orchid / 兰花 | Saturation 0.35s / 饱和 0.35 秒 |
| Closed Eyeblossom / 闭合的眼眸花 | Nausea 7s / 反胃 7 秒 |
| Cornflower / 矢车菊 | Jump Boost 5s / 跳跃提升 5 秒 |
| Dandelion / 蒲公英 | Saturation 0.35s / 饱和 0.35 秒 |
| Golden Dandelion / 金蒲公英（26.x only / 仅 26.x） | Saturation 0.35s / 饱和 0.35 秒 |
| Lily of the Valley / 铃兰 | Poison 11s / 中毒 11 秒 |
| Open Eyeblossom / 眼眸花 | Blindness 11s / 失明 11 秒 |
| Orange Tulip / 橙色郁金香 | Weakness 7s / 虚弱 7 秒 |
| Oxeye Daisy / 滨菊 | Regeneration 7s / 生命恢复 7 秒 |
| Pink Tulip / 粉红色郁金香 | Weakness 7s / 虚弱 7 秒 |
| Poppy / 虞美人 | Night Vision 5s / 夜视 5 秒 |
| Red Tulip / 红色郁金香 | Weakness 7s / 虚弱 7 秒 |
| Torchflower / 火把花 | Night Vision 5s / 夜视 5 秒 |
| White Tulip / 白色郁金香 | Weakness 7s / 虚弱 7 秒 |
| Wither Rose / 凋灵玫瑰 | Wither 7s / 凋零 7 秒 |

---

## Compatibility / 兼容性

Two packages ship under the same release — pick the one that matches your game version. Their recipe and tag contents are identical; only the `pack.mcmeta` version declaration differs.
同一个 Release 里有两个包，按游戏版本二选一。两者的配方与标签内容完全一致，只有 `pack.mcmeta` 的版本声明不同。

| Minecraft Java Edition | File / 文件 | `pack.mcmeta` |
| --- | --- | --- |
| 1.21.4 – 1.21.11 | `[1.21.4-1.21.11]easy_stew.zip` | `pack_format 61` + `supported_formats 61–94` |
| 26.1 – 26.2 | `[26.1-26.2]easy_stew.zip` | `min_format 101` + `max_format [107,1]` |

Why two files / 为什么要分两个包：

- 1.21 uses singular data pack folders (`recipe/`, `tags/item/`), 1.21.2 simplified recipe ingredients to plain strings, and 1.21.4 added the eyeblossom flowers — so this package stops at 1.21.4.
- 1.21 起目录名改为单数（`recipe/`、`tags/item/`），1.21.2 起配方 ingredient 简化为字符串，1.21.4 加入眼眸花——所以这个包的下限是 1.21.4。
- 26.x switched to `[major, minor]` format numbers, which cannot be declared together with the old single-integer scheme in one file.
- 26.x 改用 `[主版本, 次版本]` 的版本号写法，无法与旧的单整数方案写进同一份 `pack.mcmeta`。

| Item / 项目 | Value / 内容 |
| --- | --- |
| Loader / 加载器 | None (datapack) / 无（数据包） |
| Works in / 可用于 | Singleplayer, LAN, dedicated servers, Realms / 单人、局域网、服务器、Realms |

The pack only overrides vanilla recipe files and the `#minecraft:mushrooms` item tag, nothing else — 17 recipes on 1.21.4 – 1.21.11, 18 on 26.x (golden dandelion added).
数据包只覆盖原版配方文件和 `#minecraft:mushrooms` 物品标签，不改动其他内容——1.21.4 – 1.21.11 为 17 条配方，26.x 为 18 条（多一条金蒲公英）。

---

## Installation / 安装

1. Check your game version, then download the matching `.zip` from [Releases](https://github.com/mc-XiaoRan/easy_stew/releases).
2. Drop it into `<world>/datapacks/` (singleplayer) or `<server>/world/datapacks/`.
3. Run `/reload` (or restart the server), then check `/datapack list`.

1. 先确认自己的游戏版本，再从 [Releases](https://github.com/mc-XiaoRan/easy_stew/releases) 下载对应的 `.zip`。
2. 放进 `<存档目录>/datapacks/`（单人）或 `<服务器>/world/datapacks/`。
3. 执行 `/reload`（或重启服务器），再用 `/datapack list` 确认已启用。

---

## Notes / 注意

- Stew crafted before v1.1 keeps its old stack limit (1) and will not merge with the new stacks.
- 1.1 之前合成的炖菜仍是原堆叠上限（1），不会与新堆叠合并。
- Because the pack overrides `/data/minecraft/recipe/`, it will conflict with other packs that edit the same recipes.
- 由于覆盖了 `/data/minecraft/recipe/`，会与其他修改同名配方的数据包冲突。

## Repository layout / 仓库结构

```
pack.mcmeta                     # pack metadata / 数据包元数据
pack.png                        # pack icon / 图标
data/minecraft/recipe/          # 17 recipes (1 stew + 16 suspicious stew)
data/minecraft/tags/item/       # #minecraft:mushrooms tag (red + brown)
```

## License / 许可

MIT — see [LICENSE](LICENSE).
MIT 许可证——见 [LICENSE](LICENSE)。
