# 原谅帽 <img src="https://github.com/4148/greenhat/blob/master/greenhat.png" alt="greenhat image" width="10%" height="10%"/>
原谅帽是一个修改过去的'n`天提交来快速装饰你的GitHub贡献日历。 它使用`GIT_AUTHOR_DATE`和`GIT_COMMITTER_DATE`环境变量来使提交出现在过去。 请注意，原谅帽将破坏您的存储库的提交历史记录。


### 如何去使用
将 `greenhat.py` 放到你的git仓库. 确保你的[远程仓库链接被设置](https://help.github.com/articles/adding-a-remote/), 并且有一个[公钥](https://help.github.com/articles/generating-ssh-keys/). 然后使用py命令执行脚本, 使用整数指定今天之前的“n”天数来生成提交。 例如. E.g.,

	python greenhat.py <n>

生成所有提交可能需要一段时间。 如果“原谅帽”在完成之前停止，您可以通过在今天之前指定一个日期来恢复您最后一次停止的位置，如下所示：

	python greenhat.py <n> <date>

`n`是你想要生成提交的剩余天数，'date`是`yyyy-mm-dd`形式的日期字符串（例如，2013-04-05）。

#### 案例

下图是一个之后 `python greenhat.py 365`后的结果:

<img src="https://github.com/4148/greenhat/blob/master/example.png" alt="example image"/>

运行了整整八个小时. 很漂亮吧?
满足你的虚荣心吧!

### 协议
原谅帽 is distributed under the GNU General Public License v3.0 (GPLv3).
