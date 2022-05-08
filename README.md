Java Run Jersey2 in Jetty as Jar Demo
====================================

这里面有一个天坑：
1. jersey是jax的一个实现
2. jax2中的包名是`javax.ws.rs`
3. jersey2支持jax2
4. jax3包名变成了`jakarta.ws.rs`
5. jersey3支持jax3

所以如果要使用jersey2，必须使用`javax.ws.rs`。

另外，jetty当前最新版`11`不知道改了什么，代码有变，所以就用jetty10了

```
mvn clean package
java -jar target/demo.jar
```