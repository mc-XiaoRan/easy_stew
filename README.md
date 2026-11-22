# Easy Stew

![Minecraft Java Edition 1.21.5 - 1.21.11](https://img.shields.io/badge/Minecraft%20Java-1.21.5%20%E2%80%93%201.21.11-green)
![Environment](https://img.shields.io/badge/environment-datapack-orange)
![License MIT](https://img.shields.io/badge/license-MIT-blue)

Any two mushrooms can craft mushroom stew and suspicious stew.
任意两个蘑菇即可合成蘑菇煲和谜之炖菜。

[Modrinth](https://modrinth.com/datapack/easy_stew)

---

## What it changes / 功能说明

| Recipe / 配方 | Vanilla / 原版 | Easy Stew / 本数据包 |
| --- | --- | --- |
| Mushroom stew / 蘑菇煲 | 1 red + 1 brown mushroom + bowl | **any 2 mushrooms** + bowl |
| 蘑菇煲 | 棕蘑菇、红蘑菇各 1 个 + 碗 | **任意 2 个蘑菇** + 碗 |
| Suspicious stew / 谜之炖菜 | 1 red + 1 brown mushroom + bowl + flower | **any 2 mushrooms** + bowl + flower |
| 谜之炖菜 | 棕蘑菇、红蘑菇各 1 个 + 碗 + 花 | **任意 2 个蘑菇** + 碗 + 花 |

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

| Item / 项目 | Value / 内容 |
| --- | --- |
| Minecraft Java Edition / Minecraft Java 版 | 1.21.5 – 1.21.11 |
| Loader / 加载器 | None (datapack) / 无（数据包） |
| Works in / 可用于 | Singleplayer, LAN, dedicated servers, Realms / 单人、局域网、服务器、Realms |

The pack only overrides 17 vanilla recipe files and the `#minecraft:mushrooms` item tag, nothing else.
数据包只覆盖了 17 个原版配方文件和 `#minecraft:mushrooms` 物品标签，不改动其他内容。

---

## Installation / 安装

1. Download the release `.zip`.
2. Drop it into `<world>/datapacks/` (singleplayer) or `<server>/world/datapacks/`.
3. Run `/reload` (or restart the server), then check `/datapack list`.

1. 下载 Release 里的 `.zip`。
2. 放进 `<存档目录>/datapacks/`（单人）或 `<服务器>/world/datapacks/`。
3. 执行 `/reload`（或重启服务器），再用 `/datapack list` 确认已启用。

---

## Notes / 注意

- Because the pack overrides `/data/minecraft/recipe/`, it will conflict with other packs that edit the same recipes.
- 由于覆盖了 `/data/minecraft/recipe/`，会与其他修改同名配方的数据包冲突。

## Repository layout / 仓库结构

```
pack.mcmeta                     # pack metadata, format 71 / [94,1]
pack.png                        # pack icon
data/minecraft/recipe/          # 17 recipes (1 stew + 16 suspicious stew)
data/minecraft/tags/item/       # #minecraft:mushrooms tag (red + brown)
```

## License / 许可

MIT — see [LICENSE](LICENSE).
MIT 许可证——见 [LICENSE](LICENSE)。
