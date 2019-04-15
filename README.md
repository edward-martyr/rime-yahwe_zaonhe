<p align="center"><img align="center" src="./images/logo.svg?sanitize=true" alt="logo" height="100"/></p>

# rime-yahwe：吳語協會式上海話輸入法

[Plum 給出的吳語拼音方案](<https://github.com/rime/rime-wugniu>)是法吳的，並不一定適合所有的用戶。這個repo把 Plum 方案中的 `wugniu_lopha.dict.yaml` 的拼音全部轉化爲[吳語協會式拼音](<http://wu-chinese.com/romanization/>)（稍有改動，詳見下附知乎介紹鏈接），又結合了搜狗詞庫等，望能方便更多用戶、使用面更廣。簡介另見知乎上的介紹文章<https://zhuanlan.zhihu.com/p/62118563>。

| Example 1                         | Example 2                         |
| --------------------------------- | --------------------------------- |
| ![示例1](./images/gifsample2.gif) | ![示例2](./images/gifsample1.gif) |

## 安裝

### 準備

沒有安裝過 Rime 引擎的用戶先行安裝該輸入法引擎：<https://rime.im/download/>。

### 命令行

#### Mac，Linux

先安裝東風破：

```bash
curl -fsSL https://git.io/rime-install | bash
```

再通過東風破安裝 `rime-yahwe`：

```bash
cd plum
bash rime-install edward-martyr/Rime-Yahwe
```

#### Windows

調出`【小狼毫】方案選單設定` 的頁面，點擊「獲取更多輸入方案」，在跳出的窗口中輸入 `edward-martyr/Rime-Yahwe`。

#### 安卓

見下。

### 直接複製

電腦用戶將所有 `./rime-yahwe/*.yaml` 文件複製到 Rime 用戶文件夾（MacOS下一般是 `~/Library/Rime/`）即可（熟悉的用戶可以忽略 `default.custom.yaml`）。

安卓 Trime 用戶也是將文件複製到 `sdcard/Rime` 文件夾下（每臺手機 sd 卡路徑可能不同）。

## 文件說明

`default.custom.yaml`：包含朙月拼音和吳語協會式兩種的定義。熟悉的用戶可以使用自己定義的文檔。

`*.dict.yaml` 皆爲字典文件。

`yahwe.schema.yaml`：輸入方案設定，包括模糊音、簡寫等設置。

## 輸入習慣

在 `yahwe.schema.yaml` 中默認是不區分尖團的，也有 `q=ch`、 `x=sh` 等方便部分用戶習慣的設置。另外設置了一些簡寫，如 `ss=sy`、`tsh=tt`、`VV=Vh (V is any vowel, eg. nyoo=nyoh)`，在實際使用中可用可不用，熟悉的用戶都可以自定義。

可以結合Emoji一起使用，參見<https://github.com/rime/rime-emoji>，將 `schema=xxx` 改爲 `yahwe` 即可。

<img src="./images/emoji.png" alt="示例" height="200"/>

支持四字成語：

<img src="./images/chengyu.png" alt="成語" height="200"/>

支持俗語（注意「射」的寫法，可爲 `dza`，蘇滬嘉小片以外口音，區分度高，也可爲 `za`，符合上海話習慣）：

<img src="./images/idiom.png" alt="俗語" height="200"/>

通過 `luna_pinyin.poetry.dict.yaml` 支持詩句：

<img src="./images/poetry.png" alt="詩句" height="200"/>