# login

## 获取验证码
http://localhost:48080/admin-api/system/captcha/get-image
```json
{
  "code": 0,
  "data": {
    "enable": true,
    "uuid": "b1213fb6714f4c88ba634ed5e55d11d6",
    "img": "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"
  },
  "msg": ""
}
```
### CaptchaController
使用hutool生成验证码
```java
 CircleCaptcha captcha = CaptchaUtil.createCircleCaptcha(captchaProperties.getWidth(), captchaProperties.getHeight());
```
uuid 使用hutool uuid 
```java
String uuid = IdUtil.fastSimpleUUID();
```
redis 存储格式
```text
captcha_code:2d2d035caacf48b9b1322374268ff327: tvfh2
```

### 验证码验证流程
1. 进入登录页刷新验证码, 存储到redis中，并设置有效时间
2. 登录校验验证码，并删除验证码

## 前端路由逻辑
`src/permission.js`
1. 判断是否有token
2. 没有token，判断白名单，通过，否则进入登录页
3. 有token 
    3.1 是登录页 跳转到home页
    3.2 判断角色是否为空，为空(登录后)获取登录详情(权限信息，数据字典，菜单信息)，否则直接进入页面。

## 登录

### 获取租户id  
http://localhost:48080/admin-api/system/tenant/get-id-by-name
```json
{"code":0,"data":1,"msg":""}
```

### login
http://localhost:48080/admin-api/system/auth/login
```json
{
  "code": 0,
  "data": {
    "userId": 1,
    "accessToken": "41a5e0b0719b4c1da3c67e90f9df6698",
    "refreshToken": "0693866594a845bc82117ae6f365b727",
    "expiresTime": 1660524995860
  },
  "msg": ""
}
```

### 获取权限信息 
http://localhost:48080/admin-api/system/auth/get-permission-info
```json
{
  "code": 0,
  "data": {
    "user": {
      "id": 1,
      "nickname": "芋道源码",
      "avatar": "http://test.yudao.iocoder.cn/a4224a33cf8d509f97aabc5d1ef67ba81959ec471f021f30e361faf7378962ba.jpg"
    },
    "roles": ["common", "super_admin"],
    "permissions": [
      "",
      "infra:config:create",
      "system:sms-template:update",
      "system:menu:query",
      "infra:file-config:query",
      "infra:config:export"
    ]
  },
  "msg": ""
}
```
AuthController#getPermissionInfo()

### 获取数据字典 
http://localhost:48080/admin-api/system/dict-data/list-all-simple
```json
{
  "code": 0,
  "data": [
    {
      "dictType": "bpm_model_category",
      "value": "1",
      "label": "默认",
      "colorType": "primary",
      "cssClass": ""
    },
    {
      "dictType": "bpm_model_category",
      "value": "2",
      "label": "OA",
      "colorType": "success",
      "cssClass": ""
    },
    {
      "dictType": "bpm_model_form_type",
      "value": "10",
      "label": "流程表单",
      "colorType": "",
      "cssClass": ""
    },
    {
      "dictType": "bpm_model_form_type",
      "value": "20",
      "label": "业务表单",
      "colorType": "",
      "cssClass": ""
    }
  ],
  "msg": ""
}
```
DictDataController#getSimpleDictDatas

### 获取菜单列表
http://localhost:48080/admin-api/system/auth/list-menus 
```json
{
  "code": 0,
  "data": [
    {
      "id": 1254,
      "parentId": 0,
      "name": "作者动态",
      "path": "https://www.iocoder.cn",
      "component": null,
      "icon": "ep:bell-filled",
      "visible": true,
      "keepAlive": true,
      "children": null
    },
    {
      "id": 1,
      "parentId": 0,
      "name": "系统管理",
      "path": "/system",
      "component": null,
      "icon": "ep:tools",
      "visible": true,
      "keepAlive": true,
      "children": [
        {
          "id": 1224,
          "parentId": 1,
          "name": "租户管理",
          "path": "tenant",
          "component": null,
          "icon": "ep:cherry",
          "visible": true,
          "keepAlive": true,
          "children": [
            {
              "id": 1138,
              "parentId": 1224,
              "name": "租户列表",
              "path": "list",
              "component": "system/tenant/index",
              "icon": "peoples",
              "visible": true,
              "keepAlive": true,
              "children": null
            }
           ]
        }
      ]
    }
  ], 
  "msg":""
}
```
AuthController#getMenus