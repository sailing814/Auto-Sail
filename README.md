<div align="center">
  <img src="https://ccvaults.com/thumbnails/20.%20Blocks/33.%20Workplaces/Chest.png" alt="Auto Sail" width="150"/>

  <h1>Auto Sail</h1>
</div>

## **介绍**

配合 Baritone 自动挖矿模组使用的辅助工具，此模组能够实现背包装满后回家存放，并再次返回矿区。可在死亡后自动重生并返回矿区。

## **教程**
<div align="center">
[![Auto Sail](https://i0.hdslb.com/bfs/archive/a3770ccf9bcaa47b8d6cc7c380190e0188f1ff29.jpg@308w_174h)](https://www.bilibili.com/video/BV1gHcszuEji/)
</div>

## **版本更新**

- **v1.0 版本**：背包装满后回家存放；
- **v1.1 版本**：新增死亡后自动重生并返回矿区；
- **v1.2 版本**：新增 add 可执行多条指令；
- **v1.3 版本**：新增可记忆指令，退出游戏依然保存先前设置的指令；新增可自定义延迟，可自定义指令与指令之间的间隔时间，以秒为单位；
- **v1.4 版本**：新增检测处于指令延迟倒计时中玩家的异常移动，移动将重新执行上一条自定义指令；
- **v1.5 版本**：新增自定义背包放入延迟指令`/autosail delay %秒`；新增背包放入切换，全部放入或保留一个原物品`/autosail dumpall`。

## **命令**

- `/autosail add1 <指令1> %秒 <指令2> ...` - 设置包满回家指令；
- `/autosail add2 <指令1> %秒 <指令2> ...` - 设置返回矿区指令；
- `/autosail add3 <指令1> %秒 <指令2> ...` - 设置自动挖矿指令；
- `/autosail toggle` - 开启 / 关闭（背包装满回家存放）；
- `/autosail dumpall` - 全部放入/保留一个；
- `/autosail delay %秒` - 设置放入物品的间隔时间；
- `/autosail respawn` - 开启 / 关闭（死亡自动重生并返回）；
- `/autosail list` - 查看保存的配置。

---
