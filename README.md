# 学习spring-boot 的示例代码

# 一、工具：
> idea 、tomcat、jdk1.8以上

# 二、操作步骤：

新建项目：New Project ——》 Spring Initializr （选择SDK）——》填写 项目基本信息 ——》选择Web——》下一步——》完成


新建一个控制器类：HelloController

编写代码如下：
	
	 // package com.example.testdemo.controller;
	import org.springframework.web.bind.annotation.GetMapping;
	import org.springframework.web.bind.annotation.RestController;
	
	@RestController
	public class HelloController {
	
	    @GetMapping("/hello")
	    public String hello() {
	        return "3333";
	    }
	}


启动Tomcat

运行DemoApplication

浏览器中输入：http://localhost:8080/hello