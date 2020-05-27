<p align="center"><img src="https://cdn.jsdelivr.net/gh/edward-martyr/rime-yahwe_zaonhe@add3661/images/logo.svg?sanitize=true" height="120"/></p>

# rime-yahwe_zaonhe：<ruby>吳語協會式上海話輸入法<rt><ruby>Ngnyu<rt>Wunyu</ruby> <ruby>Yahweseh<rt>Yihweseh</ruby> <ruby>Zaonhegho<rt>Zanhegho</ruby> <ruby>Syzehfah<rt>Syuzehfah</ruby></ruby>

[Plum 給出的吳語拼音方案](<https://github.com/rime/rime-wugniu>)是法吳的，並不一定適合所有的用戶。這個 repo 把  Plum  方案中的 `wugniu_lopha.dict.yaml` 的拼音全部轉化爲[吳語協會式拼音](<http://wu-chinese.com/romanization/>)（稍有改動，詳見下附知乎介紹鏈接），望能方便更多用戶、使用面更廣。簡介另見知乎上的介紹文章<https://zhuanlan.zhihu.com/p/62118563> 以及 <https://zhuanlan.zhihu.com/p/78791101>。

| Example 1                         | Example 2                         |
| --------------------------------- | --------------------------------- |
| ![示例1](https://cdn.jsdelivr.net/gh/edward-martyr/rime-yahwe_zaonhe@add3661/images/gifsample2.gif) | ![示例2](https://cdn.jsdelivr.net/gh/edward-martyr/rime-yahwe_zaonhe@add3661/images/gifsample1.gif) |

## <ruby>更新須知<rt>Kensin Siutsy</ruby>

`2020.03.15` 版本起不再使用 `h` 作爲 `'` 的替代（如用 `lhin` 表示吳語拼音 `'lin`），改用 `;` 替換 `'`（直接使用引號鍵的話導致引號難以輸入以及無法用其分詞），並以冒號鍵輸入冒號*及*分號。繼續使用舊版本的話請安裝 `yahwe_zaonhe_jieupaepen`。

## <ruby>安裝<rt>Oetsaon</ruby>

### <ruby>準備<rt>Tsenbe</ruby>

沒有安裝過 Rime 引擎的用戶先行安裝該輸入法引擎：<https://rime.im/download/>。

### <ruby>灋一<rt>Faehih</ruby>：<ruby>命令行<rt>Minlinghan</ruby>

#### <ruby>Mac<rt>麥柯</ruby>, <ruby>Linux<rt>黎納科水</ruby>

先安裝<ruby>東風破<rt>Tonfonphu</ruby>：

```bash
curl -fsSL https://git.io/rime-install | bash
```

再通過東風破安裝 `rime-yahwe_zaonhe`：

```bash
cd plum
bash rime-install edward-martyr/rime-yahwe_zaonhe
```

未安裝過 rime 基本包的用戶請再輸入一行：

```bash
bash rime-install :preset 
```

#### <ruby>Windows<rt>溫濤水</ruby>

調出`【小狼毫】方案選單設定` 的頁面，點擊「獲取更多輸入方案」，在跳出的窗口中輸入 `edward-martyr/rime-yahwe_zaonhe`。

#### <ruby>安卓<rt>Oetsoh</ruby>

見灋二。

### <ruby>灋二<rt>Faehnyi</ruby>：<ruby>直接複製<rt>Zehtsih Fohtsy</ruby>

電腦用戶將所有 `*.yaml` 文件複製到 Rime 用戶文件夾（MacOS下一般是 `~/Library/Rime/`）即可（熟悉的用戶可以忽略 `default.custom.yaml`）。

安卓 [Trime](<http://osfans.github.io/trime/>) 用戶也是將文件複製到 `sdcard/Rime` 文件夾下（每臺手機 sd 卡路徑可能不同）。

## <ruby>新派口音<rt>Shinpha Kheuin</ruby>

具體在 `yahwe.schema.yaml` 中有說明。

## <ruby>文件說明<rt>Venjie Sehmin</ruby>

- `*.dict.yaml` 皆爲字典文件，若不需要則可以在 `yahwe_zaonhe.dict.yaml` 中註釋掉。
- `yahwe_zaonhe.schema.yaml`：輸入方案設定，包括模糊音、簡寫等設置。

## <ruby>輸入習慣<rt>Syzeh Zihkuae</ruby>

在 `yahwe_zaonhe.schema.yaml` 中~~默認是不區分尖團的~~新版本詳見 `yahwe_zaonhe.schema.yaml` 設置不區分尖團，也有 `q=ch`、 `x=sh` 等方便部分用戶習慣的設置。另外設置了一些簡寫，如 ~~`ss=sy`~~、`tsh=tt`、~~`-VV=-Vh (V is any vowel, eg. nyoo=nioh)`~~，etc，熟悉的用戶都可以自定義。<sup id="a1">[[1]](#f1)</sup>

可以結合Emoji一起使用，參見<https://github.com/rime/rime-emoji>，將 `schema=xxx` 改爲 `yahwe_zaonhe` 即可。

<img src="https://cdn.jsdelivr.net/gh/edward-martyr/rime-yahwe_zaonhe@add3661/images/emoji.png" alt="示例" height="200"/>

支持四字成語：

<img src="https://cdn.jsdelivr.net/gh/edward-martyr/rime-yahwe_zaonhe@add3661/images/chengyu.png" alt="成語" height="200"/>

可通過 `luna_pinyin.poetry.dict.yaml` 支持詩句：

<img src="https://cdn.jsdelivr.net/gh/edward-martyr/rime-yahwe_zaonhe@add3661/images/poetry.png" alt="詩句" height="200"/>

## <ruby>試用<rt>Syyon</ruby>

用  `rime-yahwe_zaonhe` 也有別具一格的寫詩體驗：

```txt
草長鶯飛　路邊 
某種動物　塌下的五穀 
有鋤頭和花芳 
伊講 
要從布穀鳥的叫聲當中 
挑出三個 
錯別字 
因爲鋤頭講成了乳頭 
但是 
夢裏夢着的詩 
是啥言話就是啥 
翻譯不出 
不是訛轉了　燕子的詩 

—— だせい
```

自然就具備了一種 pastoralism。

 <hr /> 

<b id="f1">1．</b>該 repository 經過了多次更改，需要之前輸入特性的用戶請從 commits 下載歷史版本的 `yahwe.schema.yaml`，而只更新 `yahwe_zaonhe.dict.yaml`。[↩](#a1)
