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

## 本地工作目录（点击直达）

> 这些是 `file://` 链接，在 VS Code / Typora 的本地预览里可点开；在 GitHub 网页上无效。

| 目录 | 路径 |
| --- | --- |
| 主仓 Kite | [`D:\JLU_tools\Kite`](file:///D:/JLU_tools/Kite) |
| 评测台 | [`D:\JLU_tools\kite-bench`](file:///D:/JLU_tools/kite-bench) |
| 展示仓库 | [`D:\JLU_tools\kite-showcase`](file:///D:/JLU_tools/kite-showcase) |
| 周报仓库 | [`D:\JLU_tools\kite-weekly`](file:///D:/JLU_tools/kite-weekly) |
| 旧原型（可删） | [`D:\JLU_tools\kite-sim`](file:///D:/JLU_tools/kite-sim) |
| Unity 工程 | [`E:\GameStudio\My project`](file:///E:/GameStudio/My%20project) |
| 模型权重 | [`D:\JLU_tools\Kite\weights`](file:///D:/JLU_tools/Kite/weights) |
| 官方 SimplerEnv | [`D:\JLU_tools\official\SimplerEnv`](file:///D:/JLU_tools/official/SimplerEnv) |
| 板端工作区（ssh） | `ssh -p 2222 user@xh2` → `~/kite-work` |

常用产物：

| 产物 | 路径 |
| --- | --- |
| 模型抓取视频 | [`model_pick_demo.mp4`](file:///D:/JLU_tools/kite-bench/out/mujoco/model_pick_demo.mp4) |
| 抓取分阶段拼图 | [`pick_demo_cam.png`](file:///D:/JLU_tools/kite-bench/out/mujoco/pick_demo_cam.png) |
| 扰动基线表 | [`perturb-baseline.md`](file:///D:/JLU_tools/kite-bench/docs/perturb-baseline.md) |
| 微调权重 | [`head_v7.pt`](file:///D:/JLU_tools/kite-bench/out/head_v7.pt) |
| 示教数据（300 条） | [`out/episodes_v4`](file:///D:/JLU_tools/kite-bench/out/episodes_v4) |
