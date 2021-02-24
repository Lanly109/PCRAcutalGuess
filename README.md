# PCRActualGuess for HoshinoBot

基于[HoshinoBot v2](https://github.com/Ice-Cirno/HoshinoBot)的猜角色现实图片的小游戏，代码改自[cygames猜语音](https://github.com/GWYOG/HoshinoBotVoiceGuessPlugin)

本项目仓库地址：[https://github.com/Lanly109/PCRAcutalGuess](https://github.com/Lanly109/PCRAcutalGuess)

## 安装方式

1. clone或者下载此仓库的代码

2. 将pcractualguess文件夹放入`hoshino/modules/`文件夹中

3. 打开`hoshino/config/`文件夹中的`__bot__.py`文件，在`MODULES_ON`中加入一行`'pcractualguess',`

4. 重启bot

5. 发送`猜现实`开始游戏。

注：

1. 首次开始游戏时，插件会从[干炸里脊资源站](https://redive.estertion.win)上下载现实图片资源包，直到数量达到代码中设置的`DOWNLOAD_THRESHOLD`。下载的图片会放入`res/img/priconne/unit/actual`文件夹下，其中`res`为Hoshinobot的资源文件夹。

2. 此插件兼容贵族决斗(位于`hoshino/modules/priconne/pcr_duel`)的金币系统，如无需该功能，请注释第`17`行和第`138-147`行代码。

3. 每次获胜可获得150金币，上限6次，如有需要可更改`PRICE`和`MAX_NUM`的值。

4. 每日上限次数**没有作可持久化**，即重启bot后已获得金币次数将重置。