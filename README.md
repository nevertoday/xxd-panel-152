<div align="center">

# XXD Panel 152｜色场基座纸艺志

把普通照片重新导演成可独立使用的艺术海报；保留主体记忆点，让材质、构图与留白共同工作。

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## 样张展示

本项目已发布 8 张实际样片，图片文件位于 `assets/examples/`。

| sample-05 | sample-07 | sample-09 | sample-11 |
| --- | --- | --- | --- |
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| sample-07 | sample-08 |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |
| sample-09 | sample-10 |
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| sample-11 | sample-12 |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 适用场景与解决的问题

适合个人摄影整理、独立出版、展览练习和生活方式视觉创作。原图构图普通、背景杂乱或主体偏小，也可以通过删减、重组、裁切和尺度变化重新建立重点，而不是把照片套上滤镜。

下半部分提取照片中最具识别性的**主体、轮廓、结构、姿态与叙事关系**，重新做美术判断，重构为**色场基座式纸艺拼贴插画**。不要完整复制照片，也不要逐物转绘；主动删除绝大多数背景和无关细节，只保留最能代表原物的视觉记忆点，通过剪纸轮廓、纸片层叠、几何概括和少量纹理重新组织，使人一眼识别它与上方照片的对应关系。

## 原始提示词 · 五种语言

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中文文件逐字保留用户原始提示词，是运行时唯一的创作与审美权威。其余四语为完整、忠实的阅读译文，不参与改写生成指令。

## 快速判断：Panel 152 适合你吗？

既要保留源图身份，也要重新构图；既要材质特征，也要主动留白。可选准确文字、智能文案或无文字；支持单图、递归目录批量以及下方四种交付模式。

## 它如何把照片变成成品

理解主体与关系 → 按原文提炼视觉语言 → 删除无关细节 → 重组尺度、位置与留白 → 生成少量贴图文案 → 检查比例、文字与成品

## 成品中最容易识别的特点

整体呈现**剪纸拼贴、上下色域分割、全宽纯色基座、局部背景色块、大面积负空间与编辑式排版**共同构成的高级视觉效果。避免完整场景转绘、复杂背景、写实透视、渐变、厚重阴影、画面填满、卡通感、3D感和模板化拼贴。

## 四种输出模式

- `top-bottom`：整张画布只有上下两个全宽区域，现实照片在上、设计在下，严格各占 50%。
- `left-right`：整张画布只有左右两个全高区域，现实照片在左、设计在右，严格各占 50%，不会旋转成上下结构。
- `design-only`：整张画布只呈现 Panel 152 的设计转译，照片只作为不可见参考。
- `wallpaper-pack`：按手机、iPad、桌面和手表分别生成完整设计壁纸，可选 `linked` 连贯套装或 `independent` 四张独立。

支持多选模式与比例（`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5` 或准确像素），以及模型生成文字、准确文字和无文字。传入目录会递归扫描图片，每张源图独立处理，共用一次交付设置；最终 PNG 平铺放入一个新任务目录。

## 开始使用

```bash
git clone https://github.com/nevertoday/xxd-panel-152.git
npx skills add https://github.com/nevertoday/xxd-panel-152 --skill xxd-panel-152
```

安装后重新启动 Agent 会话，然后调用 `$xxd-panel-152`。也可以按需追加 `--global --agent codex --yes` 做用户级安装。

常用调用示例：

```text
/xxd-panel-152 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale zh-CN
/xxd-panel-152 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-152 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-152 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

完整运行契约见 [SKILL.md](SKILL.md)；运行适配器见 [英文](references/xxd-panel-152-prompt.en.md) 与 [中文](references/xxd-panel-152-prompt.zh-CN.md)。

<!-- xxd-readme-ads:start -->
## 关于 XXD

XXD 是小小东品牌名的缩写，本项目由小小东创建并维护： [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## 广告信息｜XXD 付费服务与会员

> **广告与商业信息声明：** 以下二维码、会员与付费服务链接属于小小东的广告信息。是否扫码或购买完全自愿，不影响本开源项目的访问与使用。


<!-- xxd-panel-command-system:start -->

将军 Skills 已包含在 699 元/年的统一会员权益中，无需单独购买。

| 层级 | Skill | 负责什么 |
|---|---|---|
| **将军级** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 识别当前可用的编号 Skills；按图片、主题和用途推荐；按编号点将；组织同图多风格试稿；为图片文件夹批量分配并逐项派发。 |
| **士兵级** | `xxd-panel-NNN` | 每个编号只执行自己独立的原始提示词与审美，把将军派发的单个任务完成为成品。 |

<!-- xxd-panel-command-system:end -->

### 知识星球＋成员提示词库＋Skills 所有将军会员 · 699 元/年

[知识星球](https://wx.zsxq.com/group/15554814142882)、[小小东成员提示词库](https://vip.xiaoxiaodong.ai/)与 Skills 所有将军会员是同一份会员权益：**一次年费同时开通三项权益，无需重复付费。**

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) · [Member Prompt Library](https://vip.xiaoxiaodong.ai/)

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD WeChat" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## 许可证

本项目（包括 Skill、提示词、脚本、文档及随附样张）采用 **PolyForm Noncommercial License 1.0.0**。完整法律条文请见 [LICENSE](LICENSE)，官方页面见 <https://polyformproject.org/licenses/noncommercial/1.0.0>。

许可范围说明：

- 个人可以用于学习、研究、实验、测试、兴趣项目和私人娱乐；慈善机构、教育机构、公共研究/安全/卫生机构、环保组织及政府机构也可以使用。
- 在**非商业目的**下，你可以使用、复制、修改、制作衍生作品并分享；分享时必须同时提供本许可证（或上面的链接）以及作者提供的所有 `Required Notice:` 声明。
- 不允许用于商业产品或服务、收费交付、出售访问权或许可，或任何预期会带来商业应用的用途。需要商业使用时，请先向版权方另行取得书面许可。
- 本协议只授予其中明确写出的著作权许可和有限的专利许可，不授予商标、品牌名称或其他未明确授予的权利，也不能把你的许可再转授给他人。
- 如果收到书面违约通知，须在 32 天内纠正并采取实际补救措施，否则许可会立即终止；就专利侵权提出书面主张也会终止专利许可。
- 内容按“现状”提供，在法律允许的范围内不作任何担保，使用风险和可能的损失由使用者自行承担。
