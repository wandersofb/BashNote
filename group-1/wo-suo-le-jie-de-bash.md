# Variable

shell 变量被创建一次就会被赋值，使用 “=” 赋予。 变量可以包含数字、字符和字符串，其命名是区分大小写的并且可以包含下划线（underscore）“\_”。 注意 “=” 左右不允许空格。

## Tips

* \ 是用来转义特殊的符号
* ${} 是用来避免歧义
* "" 是用来保存变量里的空格

```shell
greeting='Hello        world!'
echo $greeting" now with spaces: $greeting"
Hello world! now with spaces: Hello        world!
```

* 变量可以用命令输出的值进行分配。这被称为替换。替换可以通过用\`\`来封装命令（即所谓的反标）或用$()来完成。注意，当脚本运行时，它将运行$()括号内的命令并捕获其输出。

```shell
FILELIST=`ls`
FileWithTimeStamp=/tmp/my-dir/file_$(/bin/date +%Y-%m-%d).txt
```
