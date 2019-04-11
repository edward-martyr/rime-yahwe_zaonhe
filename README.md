# rime-yahwe：吳語協會式上海話輸入法

Plum給出的吳語拼音方案是法吳的，並不一定適合所有的用戶。這個repo把`wugniu_lopha.dict.yaml`的拼音全部轉化爲[吳語協會式拼音](<http://wu-chinese.com/romanization/>)（稍有改動），又結合了搜狗詞庫等，望能方便更多用戶、使用面更廣。

## 安裝

將所有`*.yaml`文件複製到Rime用戶文件夾（MacOS下一般是`~/Library/Rime/`）即可。

## 使用

可以結合Emoji一起使用，參見<https://github.com/rime/rime-emoji>，將`schema=xxx`改爲`yahwe`即可。

![示例](https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/example.png)

支持四字成語：

![成語](https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/chengyu.png)

支持俗語（注意「射」的寫法，可爲dza，太湖片以外口音，區分度高，也可爲za，符合太湖片習慣）：

![俗語](https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/idiom.png)

通過`luna_pinyin.poetry.dict.yaml`支持詩句：

![詩歌](https://github.com/edward-martyr/Rime-Yahwe/blob/master/images/poetry.png)