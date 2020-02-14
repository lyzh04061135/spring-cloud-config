1、更新后需要手动调用post请求	http://localhost:9082/actuator/refresh	才能获取新的值！
2、如果需要自动刷新可以在git远程配置项目中添加webhook。

1、通过配置中心刷新调用post请求	http://localhost:9081/actuator/bus-refresh	才能获取新的值！
2、如果需要自动刷新可以在git远程配置项目中添加webhook。

1、去掉rabbitmq配置部分，去掉spring-cloud-starter-bus-amqp部分就是不通过配置中心，手动刷新模式
2、该目录是远程配置部分，需要配合本地项目spring-config使用。
3、git webhook地址 http://b612ed7b.ngrok.io/actuator/bus-refresh	ngrok.exe http 9081