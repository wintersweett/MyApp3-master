#baselibrary用来解耦，Module1与Module2既可以是单独的application，也可以是MainApp所依赖的library，
MyApp3首先是gradle.properties、build.gradle中的一些配置，
baselibrary 的接口用来解耦，真正的实现在module1和module2中，
ServiceFactory实现真正的解耦，Appconfig配置了有哪些业务module
MainApp与每个Module的自定义application，都要实现baselibrary中的IApp
