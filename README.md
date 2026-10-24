# Softglow Cursors

轻柔、半透明、带微光的 macOS 指针主题。**v0.3 设计预览版，尚非完整指针包。**

![双配色预览](first-study.png)

## 下载

- [淡蓝色 MaCursor 主题](Softglow-blue-trial01.cursor)
- [烟灰色 MaCursor 主题](Softglow-graphite-trial01.cursor)
- [完整源文件与目录结构 ZIP](softglow-cursors-v0.3-source.zip)：包含 Swift 生成与校验脚本、可编辑 SVG、透明 PNG、多分辨率图片、动画条带和主题文件。

目前是通过浏览器上传的私有预览快照；源码目录保存在 ZIP 内，之后再整理为可在线浏览的 Git 目录结构。

## 安装与恢复

安装 [MaCursor](https://github.com/writronic/MaCursor)，下载 `.cursor` 文件，通过「文件 → 导入主题」导入，然后选中并点击「应用」。回退时选原主题或点击「恢复」。

若切换窗口后主题被覆盖，将系统自定义指针颜色重设为默认，再重新应用。大小可以在系统设置 → 无障碍 → 显示 → 指针中调整。

![等待动画样稿](wait-rocking.gif)

## 当前包含

箭头、文字选择、链接手形、张手、握手，横向/纵向/两个对角方向缩放，以及等待/忙碌摇摆动画。29 个底层标识在 MaCursor 中显示 27 个条目，不等于 27 种独立造型。

普通状态静止；仅应用请求等待状态时播放动画，不代表网页或 AI 的真实运行进度。

## 已知限制

- 复制、别名、移动、禁止、帮助、准星等仍未完成，参见 [覆盖清单](COVERAGE.md)。未实现状态使用系统默认，不混用第三方主题。
- 同轴边缘共用双向缩放图形。
- 浅背景蓝色清晰度、手形比例、小目标点击准确性需要继续实测。
- 已在作者的一台 Mac 上通过 MaCursor 加载试用，尚无跨设备兼容保证。
- 文件校验通过：图片解码、透明通道、热点边界、动画条带尺寸和两个对角方向的图像区别。但边界合法不等于点击精度已经充分验证。
- 应用自行绘制的指针可能不受系统主题影响。

## 署名与许可

景文发起并指导，使用 AI 辅助设计与编码。不是 OpenAI 官方项目，不含从 OpenAI 安装包提取的图片，也不包含之前已移除的混合主题试验品。

- 原创图片、SVG、预览与主题内原创图形：[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)，署名 "Softglow Cursors by Jingwen and contributors"，修改时注明变化。详见 [LICENSE-ARTWORK.md](LICENSE-ARTWORK.md)。
- 脚本：MIT，见 [LICENSE-CODE](LICENSE-CODE)。
- 其他说明：[ATTRIBUTION.md](ATTRIBUTION.md)。

暂不作为正式完整版本发布；欢迎先做本地试用和改进。
