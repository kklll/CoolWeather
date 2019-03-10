# CoolWeather
酷欧天气App  

![pic](https://github.com/kklll/CoolWeather/blob/master/pic_.png)

#### 开发基本思想
- 设计APP来进行天气预报的显示，天气预报的信息来源于和风天气。通过请求和风天气的API来得到天气数据，此APP主要是将得到的数据展示出来。


#### 开发心得

- 初次进行安卓开发，很多东西都不太了解，以下内容如有谬误，希望大家指正。


- 郭霖的酷欧天气开发使用了四个依赖：LitePal，OkHttp，glide，GSON   
 这四个库分别用来进行数据库操作，发送http请求，展示图片，解析JSON数据。  
 
 1：加入依赖：
```
dependencies {
    implementation fileTree(dir: 'libs', include: ['*.jar'])
    implementation 'com.android.support:appcompat-v7:28.0.0'
    implementation 'com.android.support.constraint:constraint-layout:1.1.3'
    testImplementation 'junit:junit:4.12'
    androidTestImplementation 'com.android.support.test:runner:1.0.2'
    androidTestImplementation 'com.android.support.test.espresso:espresso-core:3.0.2'
    implementation 'org.litepal.android:core:1.4.1'
    implementation 'com.squareup.okhttp3:okhttp:3.4.1'
    implementation 'com.google.code.gson:gson:2.7'
    implementation 'com.github.bumptech.glide:glide:3.7.0'
    implementation 'org.jetbrains:annotations-java5:15.0'

}
``` 
![pic](https://github.com/kklll/CoolWeather/blob/master/pic.png)

此为目录结构：


- 其中db主要是对数据库的一些操作。
+ db中存放的类即省市县的类，通过get，set方法实现更号的封装。

- gson来解析从服务器上获得的数据以及一些Java类。

- utility对请求进行封装。


（具体代码就不粘贴了，自行寻找。）