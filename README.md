# kite-weekly

> Kite 项目的团队周报归档。一周一份，只写"能被追问"的东西。

## 周报索引

| 周 | 主题 | 报告 |
| --- | --- | --- |
| 2026-10-20 ~ 10-26 | 仿真闭环打通：模型抓取 8/8、输入扰动基线、三仓分工 | [2026-10-26](2026/10/2026-10-26.md) |

## 写法约定

1. **数字必须有出处**：成功率写分子分母（`8/8`），延迟写测试条件（设备、步数）
2. **区分仿真与真机**：没上真机就写"仿真"，不要用"已实现抓取"这种模糊说法
3. **交付物给链接**：代码进仓库、视频给路径、数据给目录，别只写"已完成"
4. **失败也写**：没做成的部分写清结论和下一步，比藏着强
5. **一页以内**：超过一屏没人看；细节放链接

## 模板

新建周报时复制 [`TEMPLATE.md`](TEMPLATE.md)，放到 `YYYY/MM/YYYY-MM-DD.md`，并更新上面的索引表。

## 相关仓库

| 仓库 | 内容 |
| --- | --- |
| [`Kite`](https://github.com/Kite-Robotics-Special-Interest-Group/Kite) | 端侧模型与运行时（私有） |
| [`kite-bench`](https://github.com/Kite-Robotics-Special-Interest-Group/kite-bench) | 仿真、数据、训练、鲁棒性评测 |
| [`kite-showcase`](https://github.com/Kite-Robotics-Special-Interest-Group/kite-showcase) | Unity 场景、视频渲染、对外素材规范 |

## 本地工作目录

> 仓库里的内容都能在 GitHub 上点开（见上表）；下面这些是**只存在于本机**的目录，用等宽文本列出，避免 `file://` 链接在网页上失效。

| 目录 | 路径 |
| --- | --- |
| 主仓 Kite | `D:\JLU_tools\Kite` |
| 评测台 | `D:\JLU_tools\kite-bench` |
| 展示仓库 | `D:\JLU_tools\kite-showcase` |
| 周报仓库 | `D:\JLU_tools\kite-weekly` |
| 旧原型（可删） | `D:\JLU_tools\kite-sim` |
| Unity 工程 | `E:\GameStudio\My project` |
| 模型权重（不进 Git） | `D:\JLU_tools\Kite\weights` |
| 官方 SimplerEnv | `D:\JLU_tools\official\SimplerEnv` |
| 板端工作区 | `ssh -p 2222 user@xh2` → `~/kite-work` |

## 常用产物

| 产物 | 位置 | 是否入库 |
| --- | --- | --- |
| 扰动基线表 | [`docs/perturb-baseline.md`](https://github.com/Kite-Robotics-Special-Interest-Group/kite-bench/blob/main/docs/perturb-baseline.md) | ✅ 在 kite-bench |
| Unity 教程 | [`docs/unity-setup.md`](https://github.com/Kite-Robotics-Special-Interest-Group/kite-showcase/blob/main/docs/unity-setup.md) | ✅ 在 kite-showcase |
| 视频录制规范 | [`docs/video.md`](https://github.com/Kite-Robotics-Special-Interest-Group/kite-showcase/blob/main/docs/video.md) | ✅ 在 kite-showcase |
| 模型抓取视频 | `kite-bench/out/mujoco/model_pick_demo.mp4` | ❌ 本地生成 |
| 抓取分阶段拼图 | `kite-bench/out/mujoco/pick_demo_cam.png` | ❌ 本地生成 |
| 微调权重 | `kite-bench/out/head_v7.pt` | ❌ 本地（网盘分发） |
| 示教数据（300 条） | `kite-bench/out/episodes_v4/` | ❌ 本地 |
