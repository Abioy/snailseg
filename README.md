snailseg
========

Chinese Words Segment Library in Python 简单的中文分词库

Usage
========
* 将snailseg目录放置于当前目录或者site-packages目录
* import snailseg
* 代码示例

	import snailseg
	words = snailseg.cut("南京市长江大桥")
	for w in words:
		print w



Algorithm
=========
* 算法是统计单字在词语中出现位置的概率大小，选择最大可能的分词方案

Example
=========

https://github.com/fxsjy/snailseg/blob/master/test.py

