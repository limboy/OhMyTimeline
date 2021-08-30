# OhMyTimeline

以可视化的方式展示生活中那些值得记录的场景，将那些杂糅在一起的点点滴滴通过不同的维度分解出来，就像三棱镜那样，或许会对自己的人生有不一样的认识哦。

只有一个文件，配置完后用浏览器打开该文件即可看到效果。

预览效果：https://limboy.me/life.html

![image](https://user-images.githubusercontent.com/35974/131289368-cfed8d39-6e4f-4280-b6be-1af153822ff4.jpg)

# 配置

用文本编辑器打开 `index.html` ，会在头部看到配置信息，以下是对这些配置项的说明

```yml
# 从哪一年开始展示
startYear: 1984

# 头像地址
avatar: https://limboy.me/logo.jpg

# 你的名字
name: Limboy

# 一个简短的说明
bio: get busy living or get busy dying

timeline:
  # 会展示在左边栏
  - title: 教育

    # 可选项位 line 或者 bar，前者是横线，后者是方块，通常用来展示数值，参考「收入」
    displayType: line

    items:
      # 开始的时间点，格式为 年.月，结束时间同
      - startDate: '1991.9'
        endDate: '1997.7'
        # 对当前这段时间的描述
        desc: 小学
      - startDate: '1997.9'
        endDate: '2000.7'
        desc: 中学
      - startDate: '2000.9'
        endDate: '2003.7'
        desc: 高中
      - startDate: '2003.9'
        endDate: '2007.7'
        desc: 大学（大连理工）

  - title: 收入
    displayType: bar
    # 对 Value 的说明，通常是单位，如 米 / 元
    valueDesc: (Percent)
    items:
      - startDate: '2008.5'
        endDate: '2009.4'
        desc: 时光网
        # 具体的数值，当 displayType 为 bar 时，必须要指定数值
        value: 0.05
      - startDate: '2010.4'
        endDate: '2011.7'
        desc: 凤凰网
        value: 0.1
      - startDate: '2011.7'
        endDate: '2012.4'
        value: 0.15
        desc: 知乎
      - startDate: '2013.6'
        endDate: '2014.11'
        value: 0.25
        desc: 花瓣
      - startDate: '2014.11'
        endDate: '2018.6'
        value: 0.4
        desc: 蘑菇街
      - startDate: '2019.6'
        endDate: '2021.7'
        value: 1
        desc: 字节跳动
```
