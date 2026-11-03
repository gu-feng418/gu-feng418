<!-- 数据来源：GitHub 公开接口（已认证）抓取于 2026-11-03；账号信息与仓库字段来自 /users 与 /repos，PR 计数来自 search is:pr author:gu-feng418 is:merged。人工补充项由本人确认后写入。 -->

<div align="center">

# Hi, I'm 九日 👋

**AI Agent & MCP 基础设施 · 开发者工具 · 33 个上游 PR 已合并**

<p><i>先把协议、规则和索引做成可验证的基建，再谈快不快。</i></p>

<p><i>Protocols, rules and indexes — verified before called fast.</i></p>

<p>
  <a href="https://github.com/gu-feng418">GitHub</a> · <a href="mailto:2730232528@qq.com">Email</a>
</p>

</div>

## 📊 By the Numbers <sub>数据速览</sub>

| Merged PRs | Upstream projects | Own Go tools |
| :---: | :---: | :---: |
| **33** | **9** | **2** |

<i>统计口径：GitHub 公开接口，作者维度已合并 PR 总数 / 有合并记录的上游仓库数 / 非 fork 公开仓库数 · 截至 2026-11-03</i>

## 🚀 Selected Contributions <sub>代表贡献</sub>

| Upstream project | PRs merged | What I did |
| :--- | :---: | :--- |
| [OpsiMate/OpsiMate](https://github.com/OpsiMate/OpsiMate) | **11** | 补齐客户端与服务端的测试缺口：版本徽章判定逻辑、告警分组 hook 的存储与展开、服务端 loadConfig 默认值与邮件降级，把原先没有回归保护的分支变成可执行断言 |
| [OpsiMate/documentation](https://github.com/OpsiMate/documentation) | **6** | 重写并补全产品文档：AI (Beta) 的 Bedrock 密钥配置与 AI 搜索、告警根因分析 API、按当前告警队列重写告警管理页 |
| [gombit-dev/gombit](https://github.com/gombit-dev/gombit) | **5** | 修复 client/server 契约问题：unwrap 兼容 openapi-fetch 报出的成功响应（含无 body 情况）、缺失的嵌套字段按自身路径定位、CLI jobs inspect 打印队列真实持有的载荷 |
| [foro-sh/pii-mcp](https://github.com/foro-sh/pii-mcp) | **3** | 给 PII 检测 MCP 补能力与门禁：新增英国邮编检测器、把 eval/parity.py 接进原生 wheel 任务、让 release-please PR 上的 Cargo.lock 保持同步 |
| [devlikeapro/waha](https://github.com/devlikeapro/waha) | **3** | 修复 WhatsApp API 网关问题：S3 媒体元数据改为百分号编码而不是剥离非 ASCII、NOWEB 会话 lids 计数不再取列、用 fromObject 重新加载 app state sync key |
| [uber/kraken](https://github.com/uber/kraken) | **2** | 修文档与配置：贡献者初始化改用 go mod download、nginx gzip_types 去掉未使用的 csv 条目 |

> 另有 3 个已合并 PR：modelcontextprotocol/go-sdk 里把无冒号的 SSE 行读成空值字段、mark3labs/mcp-go 里上报因非法 x-mcp-header 注解被排除的工具、alibaba/open-code-review 里加一条「扩展名从允许表消失就失败」的回归测试。

## 🔭 What I Focus On <sub>专注方向</sub>

| Direction | What I work on |
| :--- | :--- |
| MCP & Agent Tooling | 读协议实现而不是绕开它：修 MCP SDK 的 SSE 解析边界、给 mcp-go 补非法注解诊断、给 PII 检测 MCP 补检测器与 CI 门禁 |
| Code Review & Static Analysis | 把隐式约定变成可执行断言：rulefit 审计「路径 → 规则」映射里的死模式、遮蔽规则与不可达文档，open-code-review 上给允许表加回归锁 |
| Reliability & Diagnostics | 面向真实数据与 Windows 场景修问题：全盘索引定位工具 xunji、S3 元数据编码、会话状态重载、配置默认值的回归覆盖 |

## 🧰 Projects <sub>项目清单</sub>

| Area | Project | What it is |
| :--- | :--- | :--- |
| Windows tooling | [xunji](https://github.com/gu-feng418/xunji) | 全盘定位 Windows 应用 / 文件 / 快捷方式：注册表 + MS-SHLLINK 二进制解析 + 流式全盘索引，Go 零依赖单二进制，自带本地 Web UI |
| Static analysis | [rulefit](https://github.com/gu-feng418/rulefit) | 审计代码评审工具的路径 → 规则配置：遮蔽规则、死模式、不可达规则文档、未路由扩展名，每条结论带可复现 witness，支持 SARIF 输出 |

## 🛠️ Tech Stack <sub>技术栈</sub>

<img src="https://skillicons.dev/icons?i=go" alt="Go" width="40" height="40"> <img src="https://skillicons.dev/icons?i=py" alt="Python" width="40" height="40"> <img src="https://skillicons.dev/icons?i=ts" alt="TypeScript" width="40" height="40"> <img src="https://skillicons.dev/icons?i=js" alt="JavaScript" width="40" height="40"> <img src="https://skillicons.dev/icons?i=docker" alt="Docker" width="40" height="40"> <img src="https://skillicons.dev/icons?i=linux" alt="Linux" width="40" height="40"> <img src="https://skillicons.dev/icons?i=git" alt="Git" width="40" height="40"> <img src="https://skillicons.dev/icons?i=githubactions" alt="Githubactions" width="40" height="40">

## 🤝 Community & More <sub>社区与日常</sub>

- 33 个已合并上游 PR：OpsiMate(11)、documentation(6)、gombit(5)、pii-mcp(3)、waha(3)、kraken(2)，其余 3 个在 MCP SDK 与 open-code-review
- 修问题的偏好：先写能复现的用例再改实现；测试 PR 也按正式贡献写，覆盖判定逻辑而不是只覆盖格式化
- 代码之外：给开源仓库补 issue、盯 CI 与规则配置的静默漂移

## 📫 Get in Touch <sub>联系我</sub>

<p align="center">
  <a href="https://github.com/gu-feng418"><strong>GitHub</strong></a> · <a href="mailto:2730232528@qq.com"><strong>Email</strong></a>
</p>

<p align="center"><i>Open to talks about MCP tooling, code review infrastructure and developer diagnostics.</i></p>
