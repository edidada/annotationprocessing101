Compile and deploy this project to your local maven repository with: 

```

mvn clean install

```

文件
target\classes\META-INF\services\javax.annotation.processing.Processor
内容是：

```
com.hannesdorfmann.annotationprocessing101.factory.processor.FactoryProcessor
com.hannesdorfmann.annotationprocessing101.factory.processor.MyAbstractProcessor
```

javac程序检测到后会调用注册的处理器来处理
