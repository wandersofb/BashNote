# Decision Making & Loops

### Decision Making
if [ expression ]; then
    xx
elif []; then
    xx
else
    xx
fi

数值比较的类型
```shell
comparison    Evaluated to true when
$a -lt $b    $a < $b
$a -gt $b    $a > $b
$a -le $b    $a <= $b
$a -ge $b    $a >= $b
$a -eq $b    $a is equal to $b
$a -ne $b    $a is not equal to $b
```

字符串比较的类型
```shell
comparison    Evaluated to true when
"$a" = "$b"     $a is the same as $b
"$a" == "$b"    $a is the same as $b
"$a" != "$b"    $a is different from $b
-z "$a"         $a is empty
```
注意：在字符串变量周围使用""以避免特殊字符 * 的扩展


### Loops

