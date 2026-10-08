# 算力负载洞察 · Compute Workload Insight

将场景约束、技术路线与模型机制推导为算力负载、Infra优化和计算系统需求，生成或审阅中文阅读型洞察材料。按请求交付框架、文案、PPT或HTML，不默认扩展为整套材料。

**分析链条：** 场景需求与约束 → 技术路线与执行机制 → 负载变量变化 → 计算、访存、通信和调度影响 → 优化及代价 → 有条件的系统需求。

## 前置推导与总结示例

![原标准专题总结页](assets/standard-topic-preview.png)

[下载四页完整HTML](assets/complete-example.html) · [原可编辑总结页PPT](assets/standard-topic-example.pptx) · [单独使用三页前置HTML](assets/prelude-examples.html)

本次示例按 **P2技术路线 → P3执行机制 → P6优化机制 → C原标准专题总结** 组织。前三页使用独立设计的路线图、抽象机械臂场景、生成回路、缓存和时序图，围绕主视觉配置分析、变量与结论；最后保留原skill生成的C型单页及其红白版式。三页前置例和原单页也可独立使用。

HTML下载后可离线翻页和放大。前三页是HTML文字与SVG图示，第四页是原生成总结页的忠实预览；可编辑文字、表格及来源备注保留在随附PPT中。下载PPT时与HTML放在同一目录，页面内的PPT链接即可使用。生成页预览不是保密PDF原图，交付不包含内部截图或原稿回看。

原总结页中的日期、数字、证据状态与预测按原示例保留；本次仅整合模板，不代表重新核验，也不能由前三页通用机制图推定具体案例已被验证。详见[模板使用说明](references/template-guide.md)与[示例索引](references/source-gallery.md)。

## 页型结构

| 基础页型 A—E | 前置推导页型 P1—P6 |
|---|---|
| A 研究工作流 | P1 场景需求与性能约束 |
| B 全景路线矩阵 | P2 技术路线比较与演进 |
| C 标准专题洞察 | P3 业务流程与模型机制 |
| D 定量建模 | P4 规模变量与趋势证据 |
| E Agent系统专题 | P5 部署架构与资源分工 |
| | P6 优化技术与瓶颈变化 |

按缺失论证选择页面，不要求每次使用全部页型。前置页交付后续建模需要的变量、约束与适用条件。缺少数据时采用有边界的定性分析，不补造性能曲线或硬件阈值。

## 安装与使用

将仓库克隆到个人技能目录下的`compute-workload-insight`文件夹。默认目录为`~/.codex/skills/`；如果设置了`CODEX_HOME`，则使用其`skills/`目录。已有同名技能时先备份，再选择性更新。

> 使用 $compute-workload-insight，在已有定量页之前补充技术路线、执行机制和优化瓶颈变化三页，写清每页交给后续模型的变量与适用条件。保留有论证作用的机制图与输入输出样例。

也可只要求分析框架、页面文案、定量建模或审阅已有页。PPT制作需要所在环境具备演示文稿制作和渲染能力；HTML示例可直接离线查看。

## 仓库内容与来源

- `SKILL.md`、`agents/openai.yaml`：技能入口、使用边界和界面提示。
- `references/`：分析字段、页型、前置推导、视觉规则、验收清单及来源索引。
- `assets/diagrams/`：10张原创通用机制SVG，便于编辑和复用。
- `assets/`：四页完整HTML、独立三页前置HTML、逐页预览及原可编辑标准专题PPT。
- [初创企业投资推荐技能](skills/startup-investment-recommendation/SKILL.md)：支持框架、文案、离线HTML与证据审阅。[三页虚构HTML示例](skills/startup-investment-recommendation/assets/investment-example.html) · [预览](skills/startup-investment-recommendation/assets/investment-example-preview.png)。该技能目录仅含通用方法与原创虚构示例，不含原始投资模板。

本仓库为私有。当前示例资源见[可分享示例索引](references/source-gallery.md)。前三页为通用机制说明，不对应内部产品、配置或实验结果，图中节点数量、时序长度与曲线没有实际量纲；原总结页保留既有案例及其证据边界；新专题仍需重新确定数据来源和证据状态。对明确保密的材料，使用原创抽象图或已获准引用的公开资料，不以换色、去标识或描边代替内容检查。

当前版本不包含内部参考图片、完整工作区、构建临时文件、API密钥、模型权重或原始PDF文件。
