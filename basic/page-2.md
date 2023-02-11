# Decision Making

## Decision Making

if \[ expression ]; then xx elif \[]; then xx else xx fi

### 数值比较的类型

```shell
comparison    Evaluated to true when
$a -lt $b    $a < $b
$a -gt $b    $a > $b
$a -le $b    $a <= $b
$a -ge $b    $a >= $b
$a -eq $b    $a is equal to $b
$a -ne $b    $a is not equal to $b
```

### 字符串比较的类型

```shell
comparison    Evaluated to true when
"$a" = "$b"     $a is the same as $b
"$a" == "$b"    $a is the same as $b
"$a" != "$b"    $a is different from $b
-z "$a"         $a is empty
```

注意：在字符串变量周围使用""以避免特殊字符 \* 的扩展

### 逻辑与或

```shell
and 
if [ c1 -a c2 ]
if [ c1 ] && [ c2 ]

or
if [ c1 -o c2 ]
if [ c1 ] || [  c2 ]
```

### 与或运算符

#### |

管道运算符

```shell
command1 | command2
```

功能: 把第一个命令 command1 执行的结果作为 command2 的输入

#### &

不阻塞命令

```shell
./idea.sh     # 会阻塞当前终端进程
./idea.sh &   # 不会阻塞
```

#### &&

```shell
command1  && command2
```

功能： && 左边的命令（命令1）返回真(即返回0，成功被执行）后，&&右边的命令（命令2）才能够被执行；换句话说，“如果这个命令执行成功&&那么执行这个命令”。

#### ||

```shell
command1 || command2
```

功能： || 则与 && 相反。如果 || 左边的命令（command1）未执行成功，那么就执行 || 右边的命令（command2）；或者换句话说，“如果这个命令执行失败了||那么就执行这个命令”。

