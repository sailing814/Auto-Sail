<div align="center">
  <img src="./images/Chest.png" alt="Auto Sail" width="150"/>

  <h1>Auto Sail</h1>
</div>

<br>
<br>

## **介绍**

配合 Baritone 自动挖矿模组使用的辅助工具，此模组能够实现背包装满后回家存放，并再次返回矿区。可在死亡后自动重生并返回矿区。

<br>
<br>

## **教程**
<div align="center">
  
[![Auto Sail](./images/A.jpg)](https://www.bilibili.com/video/BV1kZfeBmEWb/)
<p>点击上方封面图观看演示视频</p>

</div>

<br>
<br>

## **Wiki**

- `/autosail help` - 获取AutoSail指令教程。
- `/autosail respawn`死亡自动重生后固定执行`add2`和`add3`中的指令；在`v1.6`版本移除了重生后固定输出的`#stop`指令。
- `/autosail toggle`检测背包装满后固定执行`add1`和`add2`和`add4`中的指令；在`v1.6`版本移除了背包满后固定输出的`#stop`指令。
- `%秒`可以设置小数点。
- Tick必须为`<整数>`；`20 Tick`为一秒；最大设置为`100 Tick`。
- `/autosail whitelist <cmd>`开启白名单需要添加白名单物品，但打开后再清空白名单，你将获得一个什么都嫌弃的背包！
- `/autosail movecheck toggle`在`%秒`中检测到玩家移动将重新执行上一条指令并继续进行`%秒`倒计时，`%秒`前面没有指令将再次进入`%秒`倒计时；如果你的传送会被移动打断(怪物攻击、水流、误触等)，可以尝试开启它，但它不一定每次都管用。
- `/autosail invmode`背包检测模式为`占满格子`则只要背包中每个格子上都有物品就会检测为满；背包检测模式为`堆叠满`则需背包中所有格子的物品全部堆叠上限才能检测为满(模组或插件改的部分物品可能无法检测是否堆叠满)。
- `/autosail dumpall`存放箱子的模式为`全部放入`则背包不会保留物品，将全部放入箱子；存放箱子的模式为`保留一个`则背包内会保留一个原来的物品，不会全部放入箱子。
- `/autosail whitelist add <id1> <id2>...`按键盘F3+H设置为`高级提示框：显示`把鼠标放在物品上即可看到`物品ID`；支持模组物品！
- `/autosail list`存储的配置文件保存在游戏的`config`文件夹中，名为`autosail.json`。

<br>
<br>

## **命令**

- `/autosail help` - 获取AutoSail指令教程；
- `/autosail add1 %秒 <指令1> %秒 <指令2> ...` - 设置包满回家指令；
- `/autosail add2 %秒 <指令1> %秒 <指令2> ...` - 设置返回矿区指令；
- `/autosail add3 %秒 <指令1> %秒 <指令2> ...` - 设置自动挖矿指令；
- `/autosail toggle` - 开启/关闭(背包装满回家存放)"；
- `/autosail respawn` - 开启/关闭(死亡自动重生并返回)"；
- `/autosail invmode` - 切换背包检测模式(占满格子/堆叠满)"；
- `/autosail whitelist toggle` - 开启/关闭白名单过滤"；
- `/autosail whitelist add <id1> <id2>...` - 添加白名单物品"；
- `/autosail whitelist clear` - 清空白名单"；
- `/autosail whitelist frequency <整数>` - 设置白名单丢弃频率(Tick)"；
- `/autosail movecheck toggle` - 开启/关闭移动检测"；
- `/autosail movecheck frequency <整数>` - 设置检测频率(Tick)"；
- `/autosail dumpall` - 全部放入/保留一个"；
- `/autosail delay %秒` - 设置放入物品的间隔时间"；
- `/autosail reset` - 重置所有配置到默认状态"；
- `/autosail list` - 查看保存的配置和状态"。

<br>
<br>

## **版本更新**

- **v1.0 版本**：
  - 背包装满后回家存放；
- **v1.1 版本**：
  -  新增死亡后自动重生并返回矿区；
- **v1.2 版本**：
  - 新增`add`可执行多条指令；
- **v1.3 版本**：
  - 新增可记忆指令，退出游戏依然保存先前设置的指令；
  - 新增可自定义延迟，可自定义指令与指令之间的间隔时间，以秒为单位；
- **v1.4 版本**：
  - 新增检测处于指令延迟倒计时中玩家的异常移动，移动将重新执行上一条自定义指令；
- **v1.5 版本**：
  - 新增自定义背包放入延迟指令`/autosail delay %秒`；
  - 新增背包放入切换，全部放入或保留一个原物品`/autosail dumpall`；
- **v1.6 版本**：
  - 缩短固定指令延迟，并移除固定指令延迟聊天框输出显示；
  - 移除背包满后和死亡自动重生中后固定输出的`#stop`指令；
  - 优化自定义指令，可在`<指令1>`前添加延迟，例`/autosail add1 %秒 <指令1> %秒 <指令2> ...`；
  - 新增移动检测开关`/autosail movecheck toggle`；
  - 新增自定义移动频率检测指令`/autosail movecheck frequency <整数Tick>`；
  - 新增重置指令`/autosail reset`可将所有数据重置为默认状态；
- **v1.7 版本**：
  - 新增背包检测模式`/autosail invmode`可切换占满格子检测或堆叠满检测；
  - 新增白名单功能`/autosail whitelist`可添加或清空白名单，非白名单的物品将自动扔出背包；
  - 新增自定义白名单扔出频率`/autosail whitelist frequency <整数>`。

<br>
<br>
<br>
<br>

# 反馈与支持
如果你在使用过程中遇到问题、需要帮助或有任何建议，欢迎通过以下渠道联系我们。你的反馈可能将推动Auto Sail改进！

## 加入交流群
- **QQ群**：欢迎加入我们的QQ交流群，与开发者和其他用户直接交流。
  - 群号：`1067558374`
  - 或点击链接快速加入：[点击加入QQ群](https://qm.qq.com/q/RcnG8PGgcS)
  - 扫码加入：
<div align="center">
  <img src="./images/qq.jpg" alt="QQ群二维码" width="200" />
</div>

<br>
<br>

## 赞助支持
如果这个项目对您有帮助，欢迎赞助支持项目的持续开发和维护。
- **爱发电**：[点击支持](https://afdian.com/a/AutoSail)
- **微信赞助**：
<div align="center">
  <div style="display: inline-block; margin: 0 20px;">
    <img src="./images/wx.png" alt="微信赞助" width="150"/><br>
    <small>微信赞助</small>
  </div>
</div>

<br>
<br>

## 其他反馈方式
- **电子邮件**：发送邮件至 `3145372042@qq.com`

<br>
<br>

**感谢你的使用与支持！**

---
