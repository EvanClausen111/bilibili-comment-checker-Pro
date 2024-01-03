# bilibili-comment-checker-Pro
B站评论区自动标注成分油猴脚本，识别各个成分的BU们<br />
**本项目是 [bilibili-comment-checker](https://github.com/trychen/bilibili-comment-checker) 的Fork，感谢[Trychen](https://github.com/trychen)大佬的项目**<br/>
## 目前可以检测：
* 原神
* 崩坏：星穹铁道
* 崩坏3
* 王者荣耀
* 明日方舟
* 我的世界
* A-SOUL
* VTB（关注了嘉然、永雏塔菲、东雪莲）
* 互动抽奖
---
## 效果
![使用效果](https://files.catbox.moe/91mv7d.png)
![使用效果](https://files.catbox.moe/ja751i.png)
---
* 支持视频、动态等页面的显示和识别
* 支持添加自定义的识别
* 添加查询按钮，避免频繁访问接口被封号

## Credit
本脚本动态信息获取代码来源自[原神玩家指示器作者 laupuz xu](https://greasyfork.org/zh-CN/scripts/450720-原神玩家指示器)


## 安装
* [从 Greasy Fork 安装](https://greasyfork.org/zh-CN/scripts/451164-b站成分检测器)
* [从 Github Raw 安装](https://raw.githubusercontent.com/trychen/bilibili-comment-checker/main/bilibili-comment-checker.user.js)

## 配置
基础配置:
```javascript
    // 在这里配置要检查的成分
    const checkers = [
        {
            displayName: "原神",
            displayIcon: "https://i2.hdslb.com/bfs/face/d2a95376140fb1e5efbcbed70ef62891a3e5284f.jpg@240w_240h_1c_1s.jpg",
            keywords: ["互动抽奖 #原神", "米哈游", "#米哈游#", "#miHoYo#"],
            followings: [401742377] // 原神官方号的 UID
        },
        {
            displayName: "王者荣耀",
            displayIcon: "https://i2.hdslb.com/bfs/face/effbafff589a27f02148d15bca7e97031a31d772.jpg@240w_240h_1c_1s.jpg",
            keywords: ["互动抽奖 #王者荣耀"]
        }
    ]
```

可以自行添加内容， `keywords` 表示要识别的关键字，`followings` 表示检查有没有关注特定的用户uid。

## 声明
脚本仅供学习参考，请勿用于侵害他人权益。


