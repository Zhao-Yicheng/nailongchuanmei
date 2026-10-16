# 奶龙传媒学院 🐉

> 奶龙正在护送你前往奶龙传媒学院

奶龙传媒学院校区选择页 —— 1:1 复刻「[中国奶龙大学.com](https://xn--fiqs8srwb9iv6f6w9n.com/)」的开场动画与全屏扇形校区转盘，并改名为「奶龙传媒学院」。

🌐 **已上线**：[奶龙传媒学院.com](https://xn--dpqu5wnyaiyf17sktl.com/)

仓库每次更新后网站会自动同步部署。

![预览](assets/og.jpg)

## 特性

- **开场动画**：旋转文字环 + 进度条，点击或任意按键可跳过
- **全屏扇形校区转盘**：缓慢公转、截图反向自转保持静止、悬停高亮、选中后放大跳转
- **渐进加载**：模糊占位图（LQIP 内联，零额外请求）→ 清晰 WebP 淡入，首屏约 300KB
- **细节**：深色模式、`prefers-reduced-motion` 降级、无 JS 静态兜底
- **零依赖**：纯 HTML/CSS/JS，无构建步骤，打开即用
- **SEO**：robots.txt 允许爬虫、sitemap.xml、PWA manifest

## 目录

```
index.html                单页主体（所有逻辑都在这）
assets/                   站点素材（ring/core/og/favicon、压缩后的校区图）
resource/                 校区原图、QQ 群图
robots.txt sitemap.xml manifest.json   SEO 与 PWA 基础设施
```

## 自定义

改校区只需编辑 `index.html` 顶部的 `CAMPUSES` 数组（支持 2 / 3 / 4 / 5 个，几何自动重算）：

```js
const CAMPUSES = [
  { name: "媒体工程学院", img: "assets/campus-mtgc.webp", href: "https://mtgc.cuz.edu.cn/" },
  { name: "总校官网",     img: "assets/campus-cuz.webp",  href: "https://www.cuz.edu.cn/" },
  // { name: "新校区",    img: "assets/campus-xxx.webp", href: "https://..." },
];
```

想换校名改 `UNIV` 常量，换素材直接覆盖 `assets/` 中同名文件。

## 贡献

欢迎浙传的奶龙爱好者们一起来做贡献 —— **前端代码**（动画、性能、可访问性）与**艺术设计**（校徽 logo、校区图、周边视觉）都非常需要！

<div align="center">
<img src="resource/QQ.jpg" alt="QQ 群二维码" width="240">
<p>奶龙交流 QQ 群（扫码加入）</p>
</div>

## 待办

- [ ] **logo**：目前暂用原站校徽，等待奶龙传媒学院专属设计
- [ ] **代码**：动画细节、性能与可访问性打磨

## 致谢

- 原站：[中国奶龙大学.com](https://xn--fiqs8srwb9iv6f6w9n.com/)，本页在其基础上 1:1 复刻改造
- 校徽取自群友「微微一奶很龙龙」
- 与大连理工大学、浙江传媒学院均无任何官方关联，仅供娱乐
