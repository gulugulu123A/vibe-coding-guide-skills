[English](./README_EN.md) | 中文

---

# Vibe Coding 新手上路指南 skills

> 从零搭一个个人网站，学会和 AI 高效协作。

## 这是什么

一本以**搭建个人网站**为完整实践案例的 Vibe Coding 协作手册。你跟着做完一个网站的同时，会自然理解：

- 怎么跟 AI 说清楚你要什么
- 怎么把一个项目拆成 AI 能消化的步骤
- 怎么在 AI 写出 bug 时不崩溃
- 怎么判断自己现在在什么水平、下一步该练什么

**不教具体技术，教的是方法。** 换一个框架、换一个 AI 工具，这套方法依然有效。

## 适合谁

- 第一次用 AI 做项目，不知道从哪下手
- 用过 AI 但感觉"时好时坏"，说不上为什么
- 想把自己和 AI 的协作方式系统化

## 怎么用

按顺序走完 7 个里程碑，每个里程碑包含：

| 板块 | 说明 |
|---|---|
| **要做什么** | 这一步的目标和产出 |
| **对话模板** | 可以直接复制给 AI 的提示词 |
| **确认清单** | 做完这一步要验证的事 |
| **停下来想想** | 这一步你学到了什么，对应什么底层能力 |

## 安装与使用

### 方法 1：安装为 Skill（推荐，可自动激活）

直接复制下面这句发给 Claude Code：

```
帮我安装一个 skill，地址是 https://github.com/gulugulu123A/vibe-coding-guide-skills ，装好之后引导我从里程碑 0 开始。
```

Claude Code 会自动 clone 到 skills 目录。之后每次启动时，只要你的需求跟搭网站相关，Claude Code 会识别 `SKILL.md` 中的元数据并自动激活。

### 方法 2：终端手动安装

```bash
# 克隆到 Claude Code 的 skills 目录
git clone https://github.com/gulugulu123A/vibe-coding-guide-skills.git ~/.claude/skills/vibe-coding-guide-skills
```

重启 Claude Code 后生效。也可以手动激活：

```
/skill vibe-coding-guide-skills
```

### 方法 3：不用 Skill，直接当文档用

```bash
git clone https://github.com/gulugulu123A/vibe-coding-guide-skills.git
cd vibe-coding-guide-skills
```

用你喜欢的 AI 工具打开这个目录，告诉它：

> 参考这个目录里的文档，引导我从里程碑 0 开始搭一个个人网站。

## 目录

- [里程碑 0：开工之前先问自己三个问题](./references/00-check.md)
- [里程碑 1：先把页面跑起来](./references/01-mvp.md)
- [里程碑 2：梳理内容结构](./references/02-blueprint.md)
- [里程碑 3：逐模块交付](./references/03-modules.md)
- [里程碑 4：视觉打磨的迭代方法](./references/04-polish.md)
- [里程碑 5：调试排查心法](./references/05-debug.md)
- [里程碑 6：收尾与沉淀](./references/06-ship.md)
- [终章：回头看——你在 Vibe Coding 地图上的位置](./references/07-reflect.md)

## 核心理念

> 技能可以被 AI 补上，但协作方法不行。Vibe Coding 的本质不是"让 AI 写代码"，而是"你知道怎么让 AI 写出你想要的东西"。

这本指南融合了三个底层框架：

1. **六个底层特质**（好奇心、靠谱、事实洁癖、多元化思维、忍受不确定性、低 ego 高自驱）——决定你在 AI 时代能不能走得远
2. **十个使用等级**（Lv.0 旁观者 → Lv.10 一人军团）——帮你看清自己在哪、下一步往哪走
3. **内容创作三步法**（获取信息 → 找角度 → 创作）——做网站和写文章一样，角度比执行更重要

## 推荐搭配的 Skill

以下是实际搭建过程中验证过的优质 Skill，按使用阶段推荐。每个都是独立的开源项目，**可选安装，非本项目依赖**。

### `frontend-design`
- **功能**：生成高质量、有辨识度的前端界面，避免通用 AI 审美
- **优点**：产出风格独特，不会千篇一律；内置多种设计语言参考
- **缺点**：生成代码量较大，需要筛选；简单项目可能用力过猛

### `ui-ux-pro-max`
- **功能**：50+ 设计风格、161 套配色、57 组字体搭配、99 条 UX 准则
- **优点**：相当于随身设计顾问，不用自己查配色和字体；覆盖 10 个技术栈
- **缺点**：规则较多，初次使用需要花时间了解；部分风格偏欧美审美

### `gsap-core` + `gsap-react`
- **功能**：专业级 JS 动画引擎，滚动驱动动画、弹性缓动、时间线编排
- **优点**：CSS 做不了的效果它能做（staggered reveal、3D tilt、spring 弹窗）；性能优秀
- **缺点**：有学习曲线；需要额外注册 ScrollTrigger 等插件；部分高级插件需付费

### `shadcn/ui`
- **功能**：源码级开源组件库，按钮/弹窗/表单/菜单等开箱即用
- **优点**：代码直接进项目而非 node_modules，完全掌控；社区活跃
- **缺点**：仅支持 React/Vue；初始配置需引入 Tailwind CSS

### `neat-freak`
- **功能**：会话结束后自动审查项目文档、同步 CLAUDE.md、清理过时记忆
- **优点**：防止文档腐烂，确保下次对话 AI 能正确接上；OCD 级的整理标准
- **缺点**：整理过程较耗时；可能需要多轮交互确认

## 鸣谢

感谢以下开源项目和社区：

- **[frontend-design](https://github.com/anthropics/claude-code/tree/main/plugins/frontend-design)** — 前端设计 Skill
- **[ui-ux-pro-max](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)** — UI/UX 设计智能 Skill
- **[GSAP](https://github.com/greensock/gsap-skills)** — 专业级 JavaScript 动画引擎
- **[shadcn/ui](https://ui.shadcn.com)** — 开源组件库
- **[neat-freak](https://github.com/KKKKhazix/khazix-skills/tree/main/neat-freak)** — 文档与记忆整理 Skill
- **微信公众号[数字生命卡兹克]** — 本指南的底层方法论来源于卡兹克关于 AI 时代六个特质、十级使用等级和内容创作三步法的深度分享

## 开源

MIT License，欢迎 Fork、修改、翻译成其他语言，或者用你自己的项目案例重写一遍。
