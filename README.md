# Kessoku 演示视频

本仓库存放《Kessoku 工地安全识别报警平台》的仿真演示片段。主项目仓库是私有的；
这里单独公开，为的是让四页简报里那条「在线播放」在答辩 / 路演现场能直接点开。
简报当前引用的是 `mujoco-policies.mp4`（七策略对照整幅），其余三段留作素材备查。

| 文件 | 分辨率 | 说明 |
|---|---|---|
| `fleet-formation-demo-clean.mp4` | 960×542 | 四台 Unitree Go2 地面编队 + 三架 Skydio X2 低空掠过、塔吊回转；原片顶部的说明文字条已整行裁掉 |
| `go2-trot-probe-clean.mp4` | 960×544 | Go2 策略驱动步态（直行 / 左转 / 右转），X2 走串级 PD；顶部文字条已裁掉 |
| `mujoco-policies.mp4` | 3840×576 | 派单策略对照完整版：4 列 × 2 行共 8 格，其中 7 格是七个策略（信息增益 / 拍卖 / 就近 / 共识 / 随机 / 学习式 / 轮询），1 格空白；每格左为平台 2D 真值俯视、右为 MuJoCo 3D 跟随视野 |
| `irsim-our_dwa.mp4` | 690×518 | irsim 里的第三方基线 `our_dwa`，用于对照避障表现 |

## 来源与许可

- 仿真环境：MuJoCo（Apache-2.0）与 irsim。
- 整机模型：Unitree Go2（BSD-3-Clause）、Skydio X2（Apache-2.0），均取自 MuJoCo Menagerie。
- 画面由本项目仿真脚本录制，**不是实拍**；片中出现的指标均来自同一次仿真运行。

## 用法

GitHub 的 raw 对二进制会触发下载；要在浏览器里直接播，用 jsDelivr 的 GitHub 源：
`https://cdn.jsdelivr.net/gh/ZYAONS/kessoku-demo-videos@master/<文件名>`

这些视频仅用于竞赛答辩与路演说明。
