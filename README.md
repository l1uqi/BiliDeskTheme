

# 仿B站桌面客户端白天/夜间 切换效果

上班摸鱼逛掘金看到这篇[使用全新的View Transitions API，实现B站PC客户端的深色主题切换效果](https://juejin.cn/post/7207810396420325413) 感觉挺有意思的, 在不使用文章的方式实现了一下。

## 预览
http://hello7cat.com/BiliDeskTheme/
 
## 实现
1. 底部背景, 其余页面z-index 大于背景。
2. requestAnimationFrame 是底部背景圆变大/ 变小从而实现效果
3. 文字及背景色采用mix-blend-mode来实现


## B站效果
![](https://raw.githubusercontent.com/l1uqi/PicGo/main/blog/1.gif)

## 实现效果
![](https://raw.githubusercontent.com/l1uqi/PicGo/main/blog/2.gif)
### 慢速
![](https://raw.githubusercontent.com/l1uqi/PicGo/main/blog/3.gif)




## 问题


- [mix-blend-mode会继承, 子元素无法移除](https://stackoverflow.com/questions/31629541/remove-mix-blend-mode-from-child-element)