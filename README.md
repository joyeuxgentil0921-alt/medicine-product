# 用药助手 · 老人端产品原型

面向老年人的用药管理交互设计，包含「今日」「计划」「我的」三个主要模块。本仓库集中展示最新导出的原型图、HTML 交互演示和使用教程视频。

## 体验入口

- **HTML 交互演示**：发布 GitHub Pages 后，可通过网站首页直接体验，无需登录 Figma 或 GitHub。下载到本地后，直接用浏览器打开 [index.html](index.html)。在 GitHub 仓库内点击 HTML 文件只会显示源码。
- **[Figma 交互原型](https://www.figma.com/proto/RF1My8Yh2994z0DMbGgtXi/%E8%80%81%E4%BA%BA%E7%AB%AF?node-id=329-328&t=DBbZBDRZophZvJDR-1)**：体验原生设计交互。使用作者提供的最新分享链接，匿名访问权限尚待验证；若出现申请访问，请按 [分享与发布说明](docs/分享与发布说明.md)调整 Figma 原型权限。
- **[素材总览](materials.html)**：发布 Pages 后可浏览全部原型图，并观看教程。
- **[新版操作演示视频 MP4](videos/tutorial.mp4)**：约 16.26 MiB、60 秒。由最新的「操作演示.mov」重新封装，发布包只保留这一份视频。

项目仓库：[https://github.com/joyeuxgentil0921-alt/medicine-product](https://github.com/joyeuxgentil0921-alt/medicine-product)。

Pages 网站：仓库已确认公开，当前尚未启用 Pages；启用后的预期地址为 `https://joyeuxgentil0921-alt.github.io/medicine-product/`，请以仓库 Settings → Pages 显示的地址为准。

## 主要页面

| 今日用药 | 用药计划 | 我的 |
| --- | --- | --- |
| <img src="prototypes/screens/02%E4%BB%8A%E6%97%A5.png" width="220" alt="今日用药原型"> | <img src="prototypes/screens/04%E8%AE%A1%E5%88%92_filled.png" width="220" alt="用药计划原型"> | <img src="prototypes/screens/05%E6%88%91%E7%9A%84.png" width="220" alt="我的原型"> |

- **今日**：查看用药任务、确认用药或漏服、查看用药记录。
- **计划**：管理用药计划，输入或选择药品，设置每次剂量和每日频次，调整用药时间。
- **我的**：查看与管理常用药、联系人和个人设置。

HTML 演示与 Figma 原型分别维护，交互细节以对应演示的实际行为为准。示例用药和联系方式仅用于产品展示。

## 文件目录

```text
.
├── index.html                   # 可独立运行的 HTML 演示，也是 Pages 首页
├── materials.html               # 全部原型与视频的网页总览
├── prototypes/
│   ├── screens/                 # 20 张完整页面与弹窗原图
│   └── components/              # 16 张主组件及中间状态原图
├── videos/
│   └── tutorial.mp4             # 新版操作演示，约 16.26 MiB
├── docs/分享与发布说明.md
├── manifest.json                # 原始文件大小及 SHA-256 校验清单
└── .nojekyll
```

## 发布到 GitHub Pages

1. 将本目录内容上传到公开仓库的根目录，确保 `index.html` 直接位于仓库根目录。
2. 打开仓库 **Settings → Pages**。
3. 在 **Build and deployment → Source** 选择 **Deploy from a branch**。
4. 分支选择 **main**，文件夹选择 **/(root)**，点击 **Save**。
5. 等待 Pages 部署完成，复制 **Visit site** 对应的网址，放到本 README 的体验入口和仓库的 Website 字段。

普通项目仓库的地址格式为 `https://你的用户名.github.io/仓库名/`，以 GitHub 实际显示的地址为准。首页是 HTML 演示，`materials.html` 是原型图和视频总览。

本包所有单文件均小于 25 MiB，可使用 GitHub 网页的 Add file → Upload files 上传，也可使用 GitHub Desktop 或 Git。请上传解压后的文件和文件夹，不要只把 ZIP 上传到仓库，Pages 需要展开后的文件。详细步骤见 [分享与发布说明](docs/分享与发布说明.md)。

## 原型图索引

### 完整页面与弹窗

- [01今日用药_用药记录](prototypes/screens/01%E4%BB%8A%E6%97%A5%E7%94%A8%E8%8D%AF_%E7%94%A8%E8%8D%AF%E8%AE%B0%E5%BD%95.png)
- [02今日](prototypes/screens/02%E4%BB%8A%E6%97%A5.png)
- [03计划_empty](prototypes/screens/03%E8%AE%A1%E5%88%92_empty.png)
- [04计划_filled](prototypes/screens/04%E8%AE%A1%E5%88%92_filled.png)
- [05我的](prototypes/screens/05%E6%88%91%E7%9A%84.png)
- [06我的_我的联系人](prototypes/screens/06%E6%88%91%E7%9A%84_%E6%88%91%E7%9A%84%E8%81%94%E7%B3%BB%E4%BA%BA.png)
- [07我的_联系人详情](prototypes/screens/07%E6%88%91%E7%9A%84_%E8%81%94%E7%B3%BB%E4%BA%BA%E8%AF%A6%E6%83%85.png)
- [08_我的_我的常用药](prototypes/screens/08_%E6%88%91%E7%9A%84_%E6%88%91%E7%9A%84%E5%B8%B8%E7%94%A8%E8%8D%AF.png)
- [二次确认模块](prototypes/screens/%E4%BA%8C%E6%AC%A1%E7%A1%AE%E8%AE%A4%E6%A8%A1%E5%9D%97.png)
- [删除联系人确认面板](prototypes/screens/%E5%88%A0%E9%99%A4%E8%81%94%E7%B3%BB%E4%BA%BA%E7%A1%AE%E8%AE%A4%E9%9D%A2%E6%9D%BF.png)
- [底部导航栏](prototypes/screens/%E5%BA%95%E9%83%A8%E5%AF%BC%E8%88%AA%E6%A0%8F.png)
- [我的_添加常用药面板](prototypes/screens/%E6%88%91%E7%9A%84_%E6%B7%BB%E5%8A%A0%E5%B8%B8%E7%94%A8%E8%8D%AF%E9%9D%A2%E6%9D%BF.png)
- [我的：添加联系人](prototypes/screens/%E6%88%91%E7%9A%84%EF%BC%9A%E6%B7%BB%E5%8A%A0%E8%81%94%E7%B3%BB%E4%BA%BA.png)
- [添加计划](prototypes/screens/%E6%B7%BB%E5%8A%A0%E8%AE%A1%E5%88%92.png)
- [用药计划模块](prototypes/screens/%E7%94%A8%E8%8D%AF%E8%AE%A1%E5%88%92%E6%A8%A1%E5%9D%97.png)
- [确认漏服面板](prototypes/screens/%E7%A1%AE%E8%AE%A4%E6%BC%8F%E6%9C%8D%E9%9D%A2%E6%9D%BF.png)
- [第一次用药模块](prototypes/screens/%E7%AC%AC%E4%B8%80%E6%AC%A1%E7%94%A8%E8%8D%AF%E6%A8%A1%E5%9D%97.png)
- [联系电话](prototypes/screens/%E8%81%94%E7%B3%BB%E7%94%B5%E8%AF%9D.png)
- [输入用户名面板](prototypes/screens/%E8%BE%93%E5%85%A5%E7%94%A8%E6%88%B7%E5%90%8D%E9%9D%A2%E6%9D%BF.png)
- [选择拨打电话](prototypes/screens/%E9%80%89%E6%8B%A9%E6%8B%A8%E6%89%93%E7%94%B5%E8%AF%9D.png)

### 组件与中间状态

- [Component 1](prototypes/components/Component%201.png)
- [Component 2](prototypes/components/Component%202.png)
- [Component 3](prototypes/components/Component%203.png)
- [Vector](prototypes/components/Vector.png)
- [user](prototypes/components/user.png)
- [常用药面板](prototypes/components/%E5%B8%B8%E7%94%A8%E8%8D%AF%E9%9D%A2%E6%9D%BF.png)
- [提醒按钮](prototypes/components/%E6%8F%90%E9%86%92%E6%8C%89%E9%92%AE.png)
- [朗读button](prototypes/components/%E6%9C%97%E8%AF%BBbutton.png)
- [用药确认button](prototypes/components/%E7%94%A8%E8%8D%AF%E7%A1%AE%E8%AE%A4button.png)
- [联系人](prototypes/components/%E8%81%94%E7%B3%BB%E4%BA%BA.png)
- [联系人名片](prototypes/components/%E8%81%94%E7%B3%BB%E4%BA%BA%E5%90%8D%E7%89%87.png)
- [输入剂量1](prototypes/components/%E8%BE%93%E5%85%A5%E5%89%82%E9%87%8F1.png)
- [输入剂量2](prototypes/components/%E8%BE%93%E5%85%A5%E5%89%82%E9%87%8F2.png)
- [输入药品1](prototypes/components/%E8%BE%93%E5%85%A5%E8%8D%AF%E5%93%811.png)
- [输入药品2](prototypes/components/%E8%BE%93%E5%85%A5%E8%8D%AF%E5%93%812.png)
- [闪烁](prototypes/components/%E9%97%AA%E7%83%81.png)

