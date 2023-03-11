<h1 align="center">qinglong-sign</h1>

<div align="center">
    青龙面板脚本整合库
</div>

## ✨ 内容

- 网易云音乐合伙人自动评分 ✔

## 🔨 使用

#### 打开Web界面
输入账户和密码，依次单击`订阅管理 / 新建订阅`，名称随意，链接为本repo链接，定时可以自定义，推荐`0 8 * * *`

#### 安装依赖
在`控制面板 / 依赖管理 / Python3` 处添加依赖
`PyExecJS`
`pycryptodome`
`requests`

#### 配置文件
在青龙面板容器的`/ql/data/config`目录下新建`sg_config.json`,内容如下：
```JSON
{
  "MUSIC_COPARTNER": [
    {
      "cookie": "_ntes_nuid=xxx; _ns=xxx; _ntes_nnid=xxx; UM_distinctid=xxx; NMTID=xxx; WNMCID=xxx; WEVNSM=xxx; __csrf=xxx; MUSIC_U=xxx; ntes_kaola_ad=xxx; _iuqxldmzr_=xxx; JSESSIONID-WYYY=xxx;"
    },
    {
      "cookie": "多账号 url 填写，请参考上面，url 以实际获取为准（遇到特殊字符如双引号\\\" 请加反斜杠转义）"
    }
  ]
}
```
Cookie值可能不相同，尽量把有的都填上即可

#### TODO:通知配置


## ⚙ 配置变量说明

| 配置名称            | 说明          | 获取位置                            |
|:----------------|:------------|:--------------------------------|
| MUSIC_COPARTNER | 网易云音乐cookie | [网易云音乐](https://music.163.com/) |


## 致谢

[Sitoi](https://github.com/Sitoi)

[yuxian158](https://github.com/yuxian158/)

[weixin_44530979](https://blog.csdn.net/weixin_44530979)

[KotoriMinami](https://github.com/KotoriMinami)
