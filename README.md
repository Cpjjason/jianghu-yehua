# 江湖夜话 ·《活侠传》AI 对话模组

在《活侠传》里，和唐门的人、崖底的叶云裳、雪山上的师父坐下来聊天。想说什么，直接打字；她们用原版的对话框、立绘和表情回你。

- 唐门地图上多了「夜话」，门里的人都能找来聊。
- 剧情里每次歇脚都能聊：崖底、雪山、崆峒的自由时间。
- 送礼看各人喜好，不合心意的当面退回；讨教武学、炼丹会真的加。
- 她记得你们之间的事，过几旬再去，还提得起。
- 有免费游玩的选项，不用自己找 Key；也可以用自己的 DeepSeek / OpenRouter / Kimi 等 Key。

**[下载最新版 →](https://github.com/Cpjjason/jianghu-yehua/releases/latest)**（下载 `JianghuYehua_v*.zip`）

## 安装

1. **找到游戏文件夹**：Steam 库里右键《活侠传》→ 管理 → 浏览本地文件。会打开一个文件夹，里面有 `Mortal.exe`。
2. **把压缩包里的东西全部解压进去**。解压完，`Mortal.exe` 旁边应该多出 `BepInEx` 文件夹、`winhttp.dll`、`doorstop_config.ini`、`.doorstop_version`。
   - 如果多了一层文件夹，把它里面的东西拿出来，和 `Mortal.exe` 放在一起（用「解压到当前文件夹」就不会多这一层）。
   - 已经装过 BepInEx 6 的：只把 `BepInEx\plugins\MortalTalk` 拷过去就行。
3. **正常启动游戏**。第一次启动会慢几秒。进到唐门地图，右上角「储存」左边多了「夜话」按钮，就装好了。
4. **第一次点「夜话」会打开设置，二选一**：
   - 用自己的 Key：服务商默认 DeepSeek（也能选 OpenRouter / Kimi 等），粘贴 API Key，点「测试连接」，显示「连上了」就能聊。Key 只存在你电脑上，只发给你选的服务商。
   - 不想找 Key，想免费玩：服务商选最上面的「Yumina」，点「登录 / 注册」，浏览器里注册或登录后点「允许」，游戏会自己连上。

压缩包里也有一份 `安装说明.txt`。

## 装不上？

- **地图上没出现「夜话」**：看看 `winhttp.dll` 是不是和 `Mortal.exe` 在同一个文件夹。有的杀毒软件会删掉它，把游戏文件夹加进白名单后重新解压。
- **和别的 mod 一起用**：别的 mod 也是 BepInEx 6 的就没问题；用 BepInEx 5 的 mod 不能共存。
- **游戏更新后失效**：等新版本，模组的设置页会提示「有新版本」。目前适配的游戏版本：1.0.6000.5。

## 卸载

删掉 `BepInEx\plugins\MortalTalk` 文件夹。连 BepInEx 也不要了：再删 `BepInEx` 文件夹、`winhttp.dll`、`doorstop_config.ini`、`.doorstop_version`。

## 隐私

你和角色说的话、以及这段对话需要的游戏状态（好感、时间、人物信息），会发给你在设置里选的服务商生成回复：用自己的 Key 时只发给那个服务商，选 Yumina 时发给 Yumina，别的地方都不发。夜话的记忆存在本机 `BepInEx\config\JianghuYehua\`。

## 开源组件

BepInEx 6（LGPL-2.1）· Jint（BSD-2-Clause）· Acornima（BSD-3-Clause）· Newtonsoft.Json（MIT）。由 Yumina 引擎驱动。

---

### English

**Jianghu Yehua** is an AI conversation mod for *Legend of Mortal*: sit down with anyone in the Tang Sect (and at the story's rest points) and type whatever you want to say; they answer in the game's own dialogue boxes, portraits and expressions, remember what you've shared, react to gifts by taste, and can really teach you skills.

Install: extract the release zip into the game folder (next to `Mortal.exe`), start the game, and press 「夜话」 on the map. Use your own API key (DeepSeek / OpenRouter / Kimi …) or pick **Yumina** in the provider list to play for free without a key. UI languages: Simplified Chinese, Traditional Chinese, Korean.
