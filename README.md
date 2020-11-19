# fetch-auth-code

## 解决本地开发调试时，redirect_uri 回调公网的不便
<br /> 

### 登录开放平台，将授权回调地址配置为以下地址

<br /> 

```
www.mockdata.cn
```
<br /> 


![授权回调](https://raw.githubusercontent.com/wyh-code/fetch-auth-code/master/mockdata.png)
<br /> 
<br /> 

* * *
<br /> 

### 下载依赖     

```js
npm install fetch-auth-code --save-dev
```

### 项目引入
```
import fetchAuthCode from './fetchAuthCode.js';
```


### 使用
```js
const data = await fetchAuthCode({
  id: 'xx',
  appid: 'xxx'
})

console.log(data, '===data')
//{ code: '051wQKFa1UmB0A0LoGFa1j7YlK2wQKFe', state: 'undefined-1605887483942.0002' }
```

参数说明        
https://developers.weixin.qq.com/doc/oplatform/Website_App/WeChat_Login/Wechat_Login.html

![参数说明](https://raw.githubusercontent.com/wyh-code/fetch-auth-code/master/params.png)