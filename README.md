## Gradle
No **build.gradle** na raiz do seu projeto, adicionar o maven dentro da closure **allprojects** conforme abaixo:
```
allprojects {  
  repositories {  
    maven {
      url "https://github.com/dev-cervantes/maven/raw/main"
    } 
	... 
  }  
}
```
No **build.gradle** do app, adicionar a dependência dentro da closure **dependencies** conforme abaixo:

```
dependencies {    
  implementation 'com.cielo.lio:order-manager:1.7.0'  
}
```

Realizar o build do projeto.