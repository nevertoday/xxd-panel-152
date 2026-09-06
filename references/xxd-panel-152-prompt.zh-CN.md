# Panel 152 runtime adapter

The canonical source brief is `references/original-prompt/zh-CN.md`. This adapter only records delivery variables; it never replaces the original aesthetic instructions.

- Modes: `top-bottom`, `left-right`, `design-only`, `wallpaper-pack`
- Ordinary comparison modes: strict 50:50 split; top-bottom keeps reality above, left-right keeps reality left.
- Text: `prompt`, `exact`, or `none`; resolve locale explicitly.
- Sizes: `auto`, `source`, common ratios, custom ratios, or exact pixels.
- Inputs: one image or an isolated directory batch.

将本适配器追加在完整、逐字的中文原文之后。`left-right` 只把原文上下坐标映射为左右，保留全部审美要求与严格 50:50；明确请求横向时，不得被原文的竖版上下措辞覆盖。`design-only`、`wallpaper-pack` 使用整幅设计区域，不展示原图。文字模式及目标语种只调整语言和准确内容，不改写原文图文编排原则。不得添加第三带、标题栏、底栏或内嵌面板，也不得二次风格化。
