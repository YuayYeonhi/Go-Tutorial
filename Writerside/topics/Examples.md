# Examples

## My first GO program
我们来编写第一个 Go 程序 hello.go（Go 语言源文件的扩展是 .go），代码如下：
<compare first-title="hello.go" second-title="go run">
<code-block lang="go">
package main
import "fmt"
func main() {
    fmt.Println("Hello, World!")
}
</code-block>
<code-block lang="shell">
$ go run hello.go 
Hello, World!
</code-block>
</compare>
在这个程序中：

- `package main` 定义了包的名称。`main` 包是一个特殊的包，它定义了一个独立可执行的程序，而不是一个库。
- `import "fmt"` 导入了 `fmt` 包，它包含了格式化输出的函数。
- `func main()` 定义了程序的入口点。`main` 函数在程序启动后会被自动调用。
- `fmt.Println("Hello, World!")` 调用了 `fmt` 包的 `Println` 函数，将 "Hello, World!" 打印到标准输出。

除了使用 `go run` 命令执行 Go 语言代码，我们还可以使用 `go build` 命令来生成二进制文件：
<code-block lang="shell">
$ go build hello.go 
$ ls
hello   hello.go
$ ./hello 
Hello, World!
</code-block>

