
## 怎么调试代码


### 一、 使用postman调试java REST接口

 1. 在chrome商店安装postman  [https://chrome.google.com/webstore/detail/tabbed-postman-rest-clien/coohjcphdfgbiolnekdpbcijmhambjff](https://chrome.google.com/webstore/detail/tabbed-postman-rest-clien/coohjcphdfgbiolnekdpbcijmhambjff)
<br>
 2. 先登录U2020环境，填充测试URL，在请求头 加三个键值对  
   - Cookie   :   从环境的某个请求上拷贝过来，不带{% em %}locale={% endem %}
   - Content-Type  :  application/json
   - roarand  :   从环境的某个请求上拷贝过来
<br>
 3. 填充请求体， 发送，查看响应体是否正确：
 
{% urlembed %}
../assets/media/02postman.html
{% endurlembed %}

### 二、 本地F5调试PMWebsite前端React

>   下面的例子是性能服务[PMWebsite](www.baidu.com)

 1. 根目录执行 mvn clean install -Dmaven.test.skip=true，下载好前端的依赖node_modules
 ```
mvn clean install -Dmaven.test.skip=true
 
 ```

 2. 修改 package.json 中的proxy为环境ip 
 

 3. 对request.js 加本地cookie
  ```javascript
 document.cookie = 'localLanguage=zh_CN;';
 document.cookie = 'locale=en-us;';
 document.cookie =
     'bspsession=x-6ns7g7k5by89umamqoandi1fft895fbvg8g784hfjs852kdc0bbt7wirqp3z45jv1gmo9fhdtecbk7mpuo6lfurzrwdifs6q5dqlvtqmvz2qikmnlihibyg9in3zg99f';
 document.cookie = 'user_time_a_lang=';
 document.cookie = 'roarand=543105708f91669c95d875463444110e42faa09b9a289c4c;';
  
  ```

 4. 替换cookie中的 bspsession
 
 5. npm run start
  ```
npm run start
  
  ```

 
 
{% urlembed %}
../assets/media/03ereact.html
{% endurlembed %}



&nbsp;

<br>


