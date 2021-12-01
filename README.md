# www.muluba.cc

网站分类目录目录吧网址提交API

## 基础地址：

`https://www.muluba.cc/api/`

## 申请：

邮箱联系：superbcondom###gmail.com

## 获取分类Id：

*提交时请准确填写分类Id，查到随意填写的删除所有已提交内容或重定向到同类型任意链接。*

GET:

`https://www.muluba.cc/api/?appid={appid}&action=category`

响应过长，不做展示。

## 提交URL：

post:
`https://www.muluba.cc/api/?appid={appid}&action=submit&cate={分类Id}`

post内容为提交的url的json数组，如["www.muluba.cc", "whois.muluba.cc"]

内页建议带上http/https协议，首页可以不用带。

响应内容：
```
{
    "success": 1,
    "msg": "",
    "jobId": jobId
}
```

jobId可用于任务状态查询

## 查询提交状态：

GET：
`https://www.muluba.cc/api/?appid={appid}&action=job&jobId={jobId}`

响应内容：
```
{
    "success": 1,
    "msg": "",
    "status": 1
}
```

字段说明：

status:0 代表未处理或正在处理
status:1 代表已经处理

注意：请勿滥用API，所有提交内容均已关联APPId和用户，违规提交将清理掉所有已提交内容。

具体申请可以登录[目录吧](https://www.muluba.cc) 查看文档说明
