### vim模式
- noremal模式  Esc进入normal模式（Ctrl + [）
- insert模式  i进入insert（o O a A）

### normal模式 -> 方向移动
- 上下左右移动 h j k l
- 页首 gg
- 页尾 G
- 行首 $
- 行尾 0
- 下一个词组开头 w & W
- 下一个词组末尾 e & E
- 向前移动到词组开头 e & E

### normal模式 -> 查找
- 当前行向后查找 f
- 当前行向前查找 F
- 查找一对类如([{ %
- 全局查找单词 / n下一个结果 N 上一个结果
- 查找当前光标的单词 *下一个 #上一个

### normal模式 -> 删除 替换 粘贴 复制
- 删除一个字母 x & X
- 替换一个字母 r
- 替换模式 R
- 复制 y
- 删除 d
- 粘贴 p
- 删除 dd 表示删除一行 dw删除一个词组 d$删除到行尾
- 复制 yy表示复制当前行
- 粘贴 删除命令x d都会放入到寄存器中，可以使用p进行粘贴

### normal模式 -> 重复 数字+指令
- 重复上一次命令 .
- 数字+指令 3dd

### 非ctrl指令
- C 删除至行尾并进入插入模式
- s 删除当前光标后并进行插入
- = 对齐（=G）
- ^ 行首和0的区别是忽略空格
- g_ 行尾非空格
- << 向左缩进
- >> 向右缩进
- cc S 整行删除并进行替换
- J 合并行
- v visual模式
- u U visual模式大小写替换
- ~ 当前光标下字母大小写替换
- c 表示删除并替换 cw c$

### normal ctrl指令
- c-f 向下翻一页
- c-b 向上翻一页
- c-d 向下翻半页
- c-u 向上翻半页
- c-a 计数加一

### vi yi ci di va ...
- i代表in 命令'vi(' 'vi"'
常用的
vi( vi[ vi< vi" vi' vi{ viw
va( va[ vi< va" va' va{
ci( ciw

### 替换
- :s/search/replace # 当前行匹配的第一个
- :s/search/replace/g # g表示全部匹配，这个命令会匹配当前行所有符合条件的
- :s/^/#/g # 可以使用正则表达式替换
- :s/Search/replace/i # 可以使用i表示区分大小写Search
- :10,20s/search/replace # 10 20表示第10行到第20行进行匹配
- :%s/search/replace # %s表示当前全部匹配

