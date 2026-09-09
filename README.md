<p align="center">
  <img src="docs/banner.svg" alt="paper-submission-4ss" width="100%">
</p>

# Paper 投稿整备 4SS（submission 模块独立版）

中文社会科学论文投稿文件整备模块。用于将 Markdown 成稿导出为 Word，按用户模板或内置社会学研究范式模板检查格式，整理正文引用与文后参考文献，生成投稿清单、cover letter 与 response letter。

本包由 `paper-master-4ss/scripts/export_standalone.py` 从总控包 `paper-master-4ss/modules/submission/` 自动导出：

- 包内相对路径相对本包根目录解析；
- `master/` 与 `references/` 中的协议/治理文件是导出时拷贝的快照；
- 跨模块路径 `paper-master-4ss/modules/<x>/...` 相对同级安装的总控包解析；
- 更新方式：修改总控包对应模块后运行
  `python3 paper-master-4ss/scripts/export_standalone.py submission` 重新导出，勿直接编辑本包。

## 它做什么

把接近完成的 Markdown 成稿转成投稿包：Word 导出、格式对照、正文引用与文后参考文献整理、投稿清单、cover letter 与 response letter。

不负责大规模重写正文；论证或语言问题写入检查报告并回流 write。

## 使用

将本目录安装为宿主 skill（与 `paper-master-4ss` 总控包同级）。入口见 `SKILL.md`。Word 导出依赖 pandoc；模板与体例见 `templates/` 与 `references/`。
