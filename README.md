snailseg
========

Chinese Words Segment Library in Python 简单的中文分词库

Usage
========
* 将snailseg目录放置于当前目录或者site-packages目录
* import snailseg

代码示例

	import snailseg
	words = snailseg.cut("南京市长江大桥")
	for w in words:
		print w



Algorithm
=========
* 算法是统计单字在词语中出现位置的概率大小，选择最大可能的分词方案

Performance
=========
* 700 KB/Second
* test env: Intel(R) Core(TM) i7-2600 CPU @ 3.4GHz

Example
=========
* https://github.com/fxsjy/snailseg/blob/master/test.py

Sentences:
	cuttest("这是一个伸手不见五指的黑夜。我叫孙悟空，我爱北京，我爱Python和C++。")
	cuttest("我不喜欢日本和服")
	cuttest("雷猴回归人间")
	cuttest("工信处女干事每月经过下属科室都要亲口交代24口交换机等技术性器件的安装工作")
	cuttest("我需要廉租房")
	cuttest("永和服装饰品有限公司")
	cuttest("我爱北京天安门")
	cuttest("abc")
	cuttest("隐马尔可夫")
	cuttest("雷猴是个好网站")
	cuttest("“Microsoft”一词由“MICROcomputer（微型计算机）”和“SOFTware（软件）”两部分组成")
	cuttest("草泥马和欺实马是今年的流行词汇")
	cuttest("伊藤洋华堂总府店")
	cuttest("中国科学院计算技术研究所")
	cuttest("罗密欧与朱丽叶  Hahaha")
	cuttest("新生小鼠中肌红蛋白含量较成年鼠高吗？")
	cuttest("南京市长江大桥")
	cuttest("乒乓球拍卖完了")
	cuttest("大")
	cuttest("")

Efect:
	这是 / 一个 / 伸手 / 不见 / 五指 / 的 / 黑夜 / 我 / 叫 / 孙悟空 / 我爱 / 北京 /
	我爱 / Python / 和 / C++ /
	我 / 不 / 喜欢 / 日本 / 和服 /
	雷 / 猴 / 回归 / 人间 /
	工信处 / 女 / 干事 / 每月 / 经过 / 下属 / 科室 / 都 / 要 / 亲口 / 交代 / 24 / 口
	 / 交换机 / 等 / 技术性 / 器件 / 的 / 安装 / 工作 /
	我 / 需要 / 廉租 / 房 /
	永和 / 服装 / 饰品 / 有限 / 公司 /
	我爱 / 北京 / 天安 / 门 /
	abc /
	隐 / 马尔 / 可夫 /
	雷 / 猴 / 是 / 个 / 好网 / 站 /
	Microsoft / 一 / 词 / 由 / MICROcomputer / 微型 / 计算机 / 和 / SOFTware / 软件
	/ 两部 / 分组 / 成 /
	草泥马 / 和 / 欺 / 实 / 马 / 是 / 今年 / 的 / 流行 / 词汇 /
	伊藤 / 洋华堂 / 总府 / 店 /
	中国 / 科学院 / 计算 / 技术 / 研究 / 所 /
	罗密 / 欧 / 与 / 朱丽 / 叶 / Hahaha /
	新生 / 小鼠 / 中 / 肌 / 红蛋 / 白 / 含量 / 较 / 成年 / 鼠 / 高 / 吗 /
	南京市 / 长江 / 大桥 /
	乒乓 / 球拍 / 卖 / 完了 /
	大 /
	