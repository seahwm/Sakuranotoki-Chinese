# Sakuranotoki-Chinese

樱之刻简中汉化，仅作学习交流使用。

**目前翻译完成100%**。全长48684句话，日语字符共1288806，汉字字符约一百万。感谢大家的支持~

经过各位大佬的不懈努力和润色，个人感觉一定程度上可以媲美专业汉化组的成果。希望大家玩得开心。

## 关于初版人工校对

单单从能够在这个时候以这样的形式玩到《樱之刻》汉化版的角度来说，生在有GPT4的时代不得不说是一件幸事。作为一名刚通关《樱之诗》的玩家，在急不可耐想看到续作的心情下找到了这个版本的GPT4翻译。在开始游玩后，对GPT4的翻译能力感到惊讶的同时，也发现了诸多小瑕疵。秉着举手之劳的心态，玩的同时顺便借助谷歌、DeepL翻译等现代技术的力量，一边玩一边把肉眼可见的瑕疵优化了一遍，主要集中于以下几点：

- 人称优化。在日语对话中经常会将主语省去。可能是为了符合中文的表达习惯和语法，GPT4似乎喜欢在翻译中自行加入主语，然而由于理解上下文以及人物性别的困难性，经常出现“我”“你”互换、性别错乱的情况。我将我看到的这部分都改了一遍
- 人名、地名翻译统一。
- 考据相关优化。纷繁的引经据典是SCA-自作品魅力的一环，因此，我认为能够让读者高效地直接通过译文查询到作者用典的出处，对于欣赏这部作品来说是非常重要的。通过搜索引擎的帮助，我将遇到的外国人名、画作、书籍名称等翻译规范为了中国大陆互联网上最常用的形式。对于部分诗歌翻译，我引用了以下译者的版本：
    - 金枫 译 中原中也《被污浊了的悲伤》
    - b站用户“真紅様” 译 中原中也《春日狂想》
        - 为了保持和lukibluewell版本的统一性，仅使用了部分没在《樱之诗》中出现的段落
    - 其他lukibluewell在《樱之诗》中翻译的文本，包括但不限于那首回文诗
- 其他翻译优化，包括但不限于
    - 语序、表达方式调整，也就是通常说的“润色”
    - 使用ruby text（注音）的形式，标记出原文中的部分专有名词，如“刻”

由于我本人的能力所限，以上这些优化明显是有更大的提升空间的，甚至可能存在一些错误的地方。因为时间精力有限，可能之后难以像这两周一样高强度地继续进行进一步的优化了，期待能有更厉害的大佬将这个工作继续完善下去。其实在此之前我基本没有接触过汉化相关的工作，不过在大佬们的合作中粗糙地校对完初版之后，有了一种仿佛参与了《樱花们的足迹》的感觉。或许像这样由多人协力完成的汉化作品，本身就闪耀着《樱花们的足迹》般的光芒吧。

最后，感谢kono-dadada和tsukishima1321两位大佬的意见和各种支持。希望各位读者在力所能及的范围内支持正版，也感谢SCA-自为我们带来这样一部优秀的作品。
<div align="right">
  Poritani-Makoto

  2023/06/28
</div>

## 下载方法

前往 <https://github.com/tsukishima1321/Sakuranotoki-Chinese/releases> 下载最新release

或者[点击这里](https://github.com/kono-dada/Sakuranotoki-Chinese/archive/refs/heads/main.zip)下载最新的code的zip文件。

也可以直接下载release中的`script.zip`。

## 使用方法

把`script`和`sakuranotoki_l10n_cg`文件夹放置在游戏文件夹下，然后开始游戏即可。

## 翻译说明

使用GPT4网页版，在同一个session内发送15句一段的翻译请求，能有效保持上下文连贯性。翻译脚本已经开源到[VN-ChatGPT-Translator](https://github.com/kono-dada/VN-ChatGPT-Translator)

## 致谢

感谢一位b站上认识的网友[蝉时月夜](https://space.bilibili.com/13732795)提供了3个GPT plus账号，使翻译速度提升**3倍**。

## **如果你想对此翻译贡献自己的修改**：

如果在游玩的过程中遇到了不通顺或者可能错误的地方，你可以提交修改。

有两个文件夹和一个文件需要关注：

- `translated`文件夹以json格式储存了GPT4翻译后的对话。需要手动修改的部分基本全都在这个文件夹内。
- `untranslated`文件夹以json格式储存了原文作为参照。
- `05_11_2_format.ast`文件保存了经过手动调整的格式，因为这一节在游戏内有特殊的演出效果。如果你修改了此小节，请手动修改`05_11_2_format.ast`并将里面的内容复制到`script/05_11_2.ast`。

修改完成后，运行`.\to_ast.bat`生成新的ast脚本，然后直接pull request即可。

如果你找不到错误语句的位置，你可以通过运行`find_a_sentence.py`来查找某句话在哪个文件的哪一行。 **修改过后，请确保原文和译文有相同的行数**。

最后。希望全樱之刻玩家共同维护和完善这份汉化。
