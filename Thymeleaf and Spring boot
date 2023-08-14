pom.xml

```java
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency>
```

Controller

```java
@GetMapping("/hello")
// 將Model 作為Controller 的引數，由Spring 框架自動創建並作為參數傳入
public String sayHello(Model theModel) {

	// 讓html view可以調用Model 的變數
  theModel.addAttribute("theDate", new java.util.Date());

	// 要導入的html
  return "helloworld";
}
```

增加一個頁面，在src/main/resources/templates資料夾底下增加一個helloworld.html

helloword.html

```java
<!DOCTYPE html>
//首先要將thymeleaf 的命名空間導入
<html xmlns:th="http://www.thymeleaf.org">
<head>
    <meta charset="UTF-8">
    <title>Thymeleaf Demo</title>
</head>
<body>
    <p th:text="'Time on th server is' +${theDate}"/>
</body>
</html>
```
