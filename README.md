# rime-yahwe：吳語協會式上海話輸入法

Plum給出的吳語拼音方案是法吳的，並不一定適合所有的用戶。這個repo把 `wugniu_lopha.dict.yaml` 的拼音全部轉化爲[吳語協會式拼音](<http://wu-chinese.com/romanization/>)（稍有改動），又結合了搜狗詞庫等，望能方便更多用戶、使用面更廣。簡介另見<https://zhuanlan.zhihu.com/p/62118563>。

| Example 1                         | Example 2                         |
| --------------------------------- | --------------------------------- |
| ![示例1](./images/gifsample2.gif) | ![示例2](./images/gifsample1.gif) |

## 安裝

將所有`*.yaml`文件複製到Rime用戶文件夾（MacOS下一般是`~/Library/Rime/`）即可。

## 文件說明

`default.custom.yaml`：包含朙月拼音和吳語協會式兩種的定義。熟悉的用戶可以使用自己定義的文檔。

`*.dict.yaml` 都是字典文件。

`yahwe.schema.yaml` 輸入方案設定，包括模糊音、簡寫等設置。

## 輸入習慣

在 `yahwe.schema.yaml` 中默認是不區分尖團的，也有 `q=ch`、 `x=sh` 等方便部分用戶習慣的設置。另外設置了一些簡寫，如 `ss=sy`、`tsh=tt`，在實際使用中可用可不用，熟悉的用戶都可以自定義。

可以結合Emoji一起使用，參見<https://github.com/rime/rime-emoji>，將 `schema=xxx` 改爲 `yahwe` 即可。

<img src="https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/example.png" alt="示例" height="200"/>

支持四字成語：

<img src="https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/chengyu.png" alt="成語" height="200"/>

支持俗語（注意「射」的寫法，可爲dza，蘇滬嘉小片以外口音，區分度高，也可爲za，符合上海話習慣）：

<img src="https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/idiom.png" alt="俗語" height="200"/>

通過`luna_pinyin.poetry.dict.yaml`支持詩句：

<img src="https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/poetry.png" alt="詩句" height="200"/>