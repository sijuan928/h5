# 泉州南音 H5

源码仓库：sijuan928/h5，生产分支 main。
固定网址：https://majestic-profiterole-540cdc.netlify.app
Netlify 自动部署 main；发布目录为根目录，无构建步骤。

## 本版

v0.2.3：仅优化响应式 CSS；阅读区最大 1040px，正文最大 680px，小屏自然撑高，图片完整显示，保留文案、结构、素材、字体、配色及交互逻辑。

v0.2.2：第五章三位人物替换为小组提供的照片，保留原图、水印和完整画面。v0.2.1 文案替换见 COPY.md。原版基础为 黛青水墨、六章叙事、乐器卡片/抽屉、互动工乂谱、时代切换、三个选择结局。纯 HTML、CSS 与原生 JavaScript。声音由 Web Audio 合成，不加载音频文件，不自动播放。

部署前：本地检查交互、移动尺寸、无控制台错误、资源完整；同步修改 app.js 的 VERSION、index.html 版本/资源查询串与 version.json。部署后：检查固定网址的版本与资源、真实交互，未经验证不声明发布成功。
无 Service Worker。首页/脚本/样式重验证，版本文件 no-store；页面每分钟及返回前台时检查更新，显示刷新提示，不强制打断用户阅读。

## 内容与素材

以用户上传《03-交付指令包》和《02-视觉设计与素材拆分》顶部 v3 修订为视觉依据。取消朱砂与副标题斜杠，使用新版黛青色板。用户已确认允许按官方资料校正事实性表述。

校正：基本谱字使用乂、工、六、思、一；三弦为拨奏、圆角琴箱，不能写成敲鼓；二弦共鸣体不笼统写作竹筒；来源用历代南迁与融合，不固定唯一发端年代；课堂传承用官方资料；删除未核验方言音注，宫商角徵羽/简谱作入门示意，非固定绝对音高。四乐器“骨、肉、线、点”为文学比喻。

图像由内置 imagegen 生成，压缩为 WebP，透明图保留 alpha。场景为创作插画，非历史照片；乐器插画不作精确形制图。音频为五声音阶合成示意，不当作真实南音或历史录音。页面有真实演奏资料入口和来源对话框。

来源：
- https://ich.unesco.org/en/RL/nanyin-00199
- https://www.ihchina.cn/project_details/12600
- https://www.quanzhou.gov.cn/lyb/mfms/mjqy/201510/t20151029_181676.htm
- https://data.fjdsfzw.org.cn/upload/Annals/2011/鲤城区志/epub/ops/1529.htm
- https://jyj.quanzhou.gov.cn/zwgk/zfxxgk/gdgk/rdty/rddbjy/202504/t20250413_3157902.htm
- https://www.hqu.edu.cn/info/1071/709813.htm

字体自托管：Noto Serif SC、LXGW WenKai、Cormorant Garamond；OFL 许可证随 assets/licenses 保存。已按页面实际文字子集化，新文案出现缺字时需更新字体子集。

## 适配取舍

长说明放抽屉或 details，优先保证字体、48px 点击区域与可滚动访问。小屏或横屏允许章节自然增加高度，避免为固定一屏而裁掉内容；首尾采用完整竖屏，尊重 safe-area 和 prefers-reduced-motion。所有文案为 HTML 文本，所有交互按钮为 HTML/CSS/SVG，图中不含界面文字。
