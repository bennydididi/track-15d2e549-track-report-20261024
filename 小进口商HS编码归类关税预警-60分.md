这个产品帮助从中国重复进货到美国的小进口商，在补货期间跟踪已确认的商品编码时，解决与自己商品有关的关税变化获知太晚、官方通知难以筛选的问题。

# 小进口商 HS 编码归类关税预警：只评“已有编码的关税变更提醒”

调研日：2026-10-24。HS 是商品海关分类体系；HTS 是美国使用的关税表及其商品编码。事实、厂商自述、研究判断和试验假设分开标注。

## 一分钟决策

| 钉死的研究对象 | 本次范围 |
|---|---|
| 谁 | 向美国重复进口、没有专职贸易合规人员、已有报关行确认编码的小进口商；先限中国原产商品。不是替客户归类的报关行。 |
| 场景 | 商品编码已确定，采购至到港期间需要知道政策是否影响下一批货。 |
| 输入 | 商品 CSV：内部商品编号、已确认的美国 HTS 编码、原产地、预计进口日期。缺资料先补齐。 |
| 输出 | 相关商品清单、变更前后税率（能够确定时）、生效日、官方文件链接和待确认条件；邮件提醒并保存记录。 |
| 只判一个用户任务 | **把官方关税变化匹配到我的既有商品，及时告诉我哪些需要复核。**不承诺预测未来政策或保证最终应纳税额。 |
| 相邻机会，只列表 | 商品描述→自动归类；发票→报关资料；编码→一次性税费/落地成本计算；反倾销/反补贴适用性判断；旧编码→新编码映射；历史报关退税审计。均不计主搜索量、付费证明或竞争评分。 |

| 三维决策 | 当前判断 | 决定性依据 |
|---|---|---|
| 有没有相关需求 | **有，但主动用户证据薄。** | 有进口卖家自述在货物受影响后才得知变更；官方也持续发布关税表版本。不能据此估计发生率。[用户原帖][r-monitor]、[USITC 版本库][archive] |
| 当前切口能否独立收费 | **待验证；已有直接收费供给，目标客户的付费 PMF 未证明。** | HTSAlert 将监控单独销售；同时存在免费监控。公开报价、免费用户、企业套件案例均不能替代小进口商的实际付款与续费。[HTSAlert][alert]、[免费 Radar][radar] |
| 是否优先靠 SEO | **暂不优先。保留小规模工具页试验，不做大规模内容站。** | 主任务词没有可确认的正数月搜；旧表的“0”有采集歧义；美国结果样本不满十条。查码、计算器流量不能移给提醒任务。[供应商接口][volapi]、[同任务搜索入口][google-monitor] |

**建议：继续低成本付费验证，暂不立项完整 SaaS。** 最有可能改变决定的未知是：客户用过免费监控后，是否还愿意为更可信、更及时的同任务提醒续费，而不是顺带购买归类、退税或咨询。下一步做同一批商品的免费产品对照与一个月付费试点；首付、复用、续费分别记录，阈值见后文。

下表逐项对照专员与现行筛选标准；分数均为研究判断，各项满分 5。专员旧五项与现行五项不同，不能硬移分。

| 现行五项 | 专员原分 | 核实后分 | 关键依据及边界 |
|---|---:|---:|---|
| ①需求真实 | 5（原“需求量”） | 4 | 主动监控投诉存在，但可靠全量频次未找到；归类工作量不计入这里。[原帖][r-monitor] |
| ②付费意愿 | 4 | 3 | 同任务产品有公开月费；目标小进口商的独立付费、续费人数未找到。[HTSAlert][alert]、[PortRobin][port] |
| ③好服务 | 未评分 | 2 | 用户虽非专家，却会用提醒做采购决策；误报、漏报和生效日出错都有后果。厂商自己将准确性视为核心。[监控方法][alert-about] |
| ④小团队做得动 | 4（原“小团队”） | 3 | 有独立开发者运营的同任务软件；官方版本可下载，但规则维护和异常复核不能省略。[运营者自述][alert-about]、[官方版本库][archive] |
| ⑤形态简单 | 未评分 | 3 | 输入可用表格，后台却要持续采集、匹配、去重、保留版本，不是一次提交出结果的表单。[同任务工作流][hero-monitor] |

专员原“AI 友好”4、“B 端”5不等于现标准的“好服务”和“形态简单”。需求来源及旧报告已随证据包保存；没有公开托管链接，不伪造网页来源。

## 判断依据

### 1. 真痛点是“谁负责持续盯住我的商品”，不是再生成一个编码

**支持：重复进口期间存在无人跟踪的空档。反证：部分卖家能靠手动检查、报关行或接受涨价解决，并不自然形成订阅。**

| 原声及用户 | 抱怨哪一步／现用办法 | 日期、热度与证据强弱 |
|---|---|---|
| FBA 版卖家自述：在货已受影响后“2 weeks after it already hit a shipment”才从 LinkedIn 得知。[原帖][r-monitor] | 政策→自己的商品→及时获知这一段失败；发帖询问手查 CBP、找报关行还是吸收成本。未提自己已购买软件。 | 当前页显示约 3 个月前；绝对发帖日、票数、评论总数**未找到**。可核主文，身份和损失未独立审计。支持需求存在，不证明常见或愿付费。 |
| 同帖从业回复推荐 CSMS 和盯自己的编码；另有回复选择涨价或接受成本。[原帖][r-monitor] | CSMS 是 CBP 的消息服务；官方材料确认可订阅邮件。有人已有可接受替代。[CBP 材料][csms-doc] | 同一线程，不另算独立需求。自称开发者并推广工具的回复不算客户证明。 |
| Alibaba 版监控帖回复：“The values don't change that often.”[原帖][r-manual] | 手动查编码和叠加税项；认为正常情况下变化不频繁。 | 页面约 5 个月前；精确日期、票数、评论总数**未找到**。主帖明确推广 RiskSim AI，排除主动投诉，仅保留回复反证。 |
| smallbusiness 版询问关税损失和跟踪方式。[原帖][r-research] | 是市场调研提问；回复建议按同一商品比较各批次成本，没有可核监控订阅付款。 | 搜索缓存标 2026-07-20、+7；当前页面不显示票数，评论总数**未找到**。排除主动投诉。[搜索所得原页][r-research] |
| AmazonFBA 版电子产品卖家拟做提醒工具，问用户愿付多少。[原帖][r-builder] | 自述损失后开始开发；提出的价格属于创业者试价。 | 搜索缓存标 2026-04-07、+2，已超本次半年窗口；排除主动投诉及付费证据。[原页][r-builder] |

本次上述与监控直接相关的 **4 个线程**中，只保留 **1 个非明确调研/推广的主动痛点线程**；“得知太晚”计 **1 次**，明确确认购买本任务 SaaS 的陈述计 **0 次**。这是人工选样计数，不是版块发生率，也不是“市场无人付款”。来源为上表四条原帖；排序表见证据包 `reddit-selected.json`。

Reddit 方法：核心从业版块选 `r/CustomsBroker`、`r/importexport`，FBA、Alibaba 仅补相关讨论。以 2026-04-24—2026-10-24 为窗口请求 Arctic Shift；两个核心版块各试两次、间隔 3 秒，均 DNS 失败；因此未取得半年全量，退回 `site:reddit.com`。没有可靠评论总数，不能按评论数排序；可见票数只用于两个非合格样本的降序展示，不用旧报告票数填空。[Arctic 接口][arctic]、[Reddit 入口][r-monitor]。详细请求与错误保存在 `arctic-attempts.json`。

### 2. 商业供给对口，但报价还不是独立收费成立

**有竞品支持需求存在；当前缺的是“小进口商只为持续提醒付款并续费”的证据。免费方案已对口，但本轮未实测其覆盖和满意度，不能据此宣布收费机会不存在。**

以下均为官网自述，未实测准确性或交付时效；只比较监控部分。

| 同任务玩家 | 公开供给／价格 | 能证明什么，不能证明什么 |
|---|---|---|
| HTSAlert | 已知编码每日监控、变化邮件；免费监控 5 个编码，Starter **$19/月**、Pro **$49/月**、Broker **$129/月**；Pro 含 CSV 记录导出。[官网][alert] | 切口本身已有独立售卖形态，运营者自称独立开发者。[方法页][alert-about] 付费客户数、营收、续费、融资、可靠流量数据均**未找到**。 |
| HTS Hero Tariff Tracker | 编码＋原产地监控；当前首页 **$12/月起**，最多 10 组；监控页列 30 组 **$29/月**。[首页][hero]、[监控页][hero-monitor] | 同任务价格成立。监控页称被数百报关行、货代和制造商信任，未说明付费及小进口商占比。营收、续费和可靠流量**未找到**。旧定价页缓存显示 **$49/月起**，与现页冲突，不能混成统一现价。[旧价页][hero-old] |
| PortRobin Pro | **$29/月**，监控最多 100 个编码＋原产地组合；归类和成本工具同时打包。[定价][port] | 证明监控被放进付费层；不能拆出监控收入或证明用户仅为提醒购买。客户数、营收、续费、融资、可靠流量**未找到**。 |
| Quickcode | 进口商方案 **$2,099/月起**，最多 25,000 个被监控商品，同时包含其他合规功能。[定价][quick-price] | 企业级同任务交付可见；Field Fastener 是厂商具名综合案例，未披露监控单项合同及目标小客户付款。不能用它通过当前切口 PMF 门槛。[案例][quick-case] |
| CustomsGenius Trade Radar | 按导入报关记录的编码与原产地筛选政策；页面明确 **feed 和 digest 免费且独立，无需信用卡**。[产品页][radar] | 免费替代直接命中筛选提醒任务。实际覆盖、漏报率及用户满意度**未找到**。是必须对照的产品，不是自动否决票。 |

同任务搜索还出现 [USTariffRates 观察列表][us-alerts]、[TariffClassify 编码变化邮件][classify-alerts]、[ImportCostCalculator 类目变化邮件][import-alerts]；价格与使用效果未核实的部分不加付费分。它们说明仅做“填编码、收邮件”并非空白。

**可切缝隙目前只是待验证假设：** 用更容易整理的既有商品表导入、明确区分“公告已发／税表已更新／条件尚未确定”，在同一提醒里给出可追溯原文和版本。用户讨论支持“消息到自己商品之间缺人负责”，官方版本库支持保留依据；但竞争产品已覆盖不少这些功能，**未找到竞品用户明确愿为上述差异迁移付费的证据**。[用户线程][r-monitor]、[版本库][archive]、[现有工作流][hero-monitor]

### 3. SEO 暂无足够证据排第一，仍可低成本试

**先承接“我要监控我的编码”，不能用“我要查一个编码／算一次关税”的词代替。** 以下是本次美国主任务的全部核心表达；月量来源为用户提供的 PXAny 快照，非 Google 官方保证值。数据对应原快照采集日 2026-10-24，供应商未给出可核统计窗口。[供应商量接口][volapi]

| 美国核心词 | 原快照 | 最终可采信状态 | SERP 与页面承接 |
|---|---|---|---|
| tariff monitoring software | 标 0 | **未返回，原 0 待核** | Google 美国样本 9 条；软件、厂商内容、宏观追踪混合。页面提供导入并监控功能。[对口产品入口][hero-monitor] |
| tariff change alerts | 标 0 | **未返回，原 0 待核** | 样本 9 条，包含官方公告、提醒产品和新闻。页面交付按商品筛选的提醒。[同任务入口][radar] |
| tariff alerts by hts code | 标 0 | **未返回，原 0 待核** | 样本 9 条，部分为查码或说明文；可承接观察列表。[直接结果页][us-alerts] |
| import duty change notifications | 标 0 | **未返回，原 0 待核** | 样本 9 条，含提醒工具、内容及非工具页。可承接邮件通知。[直接结果页][classify-alerts] |
| tariff alerts for small importers | 标 0；原未查 SERP | **未返回，原 0 待核** | 已补公开网页搜索，核读 3 个同任务入口：HTSAlert、HTS Hero、GingerControl。不是固定美国 Google 前十，不报告排名。[入口一][alert-about]、[入口二][hero-monitor]、[入口三][ginger] |

上述每组原样本只有 **9 条**，不称“看完整前十”；第五词补查不提供完整排名结论。现有数据不能算可获点击、付费转化或流量回本，相关数值均**未找到**。搜索意图与功能本轮已核，量缺失不等于需求不真实。

**搜索量审计影响结论：** 原采集器对 `avgMonthlySearches` 缺失也写 0；原始 `metrics` 响应没有保留，无法确认“真 0”与“缺字段”。所以主任务词全部按“未返回／待核”处理，不说搜索量为零。本轮尝试重查 API，DNS 失败。高量相邻词没有进入当前切口的量或获客判断。[接口来源][volapi]；代码与网络日志随包保存。

域名年龄仅观察：原快照记录 CustomsGenius 注册于 **2025-11-13**、USTariffRates 于 **2026-02-26**、ImportCostCalculator 于 **2026-01-26**；均有页面出现在相关样本。独立 RDAP 复核 DNS 失败，注册时间仍是供应商待复核值。[RDAP：CustomsGenius][rdap-cg]、[USTariffRates][rdap-us]、[ImportCostCalculator][rdap-ic]。这只能提示“有年轻域名值得继续查”，不能说明新站容易排名；其中还有免费产品和内容页，付费转化未知。

### 4. 远程交付可行，持续正确维护才是负担

**小团队可以做窄监控试点；不能把它按简单表单估工。** USITC 提供版本及部分 CSV/XLS/JSON 文件，CBP 提供消息渠道，数据底座存在。[版本库][archive]、[CBP 材料][csms-doc] HTSAlert 的公开流程包括参考编码校验、异常变化拦截、分别保存检测日和法律生效日，说明可靠交付需要持续维护。[方法页][alert-about]

本次只销售远程软件：CSV 导入、账户订阅、邮件和导出均可在线完成。归类、申报代理和逐票应税判断不纳入交付。CBP 的 H350722 涉及外国在线平台的 AI 归类等服务及执照问题；**不能从“软件／用户确认”直接推导业务豁免**。实际流程边界的专业核查结果**未找到**，上线前必须落实，否则小团队执行分继续下调。[CBP 裁定检索原文][ruling]

【判断】AI 越强，通知抽取、关联候选商品、解释变化会更省工；客户购买的是持续跟踪与证据记录，价值不会因能聊天而消失。另一方面，基础匹配和摘要更容易复制，AI 也可能误读条件。主优势须来自可核来源、完整版本和稳定运营，不能用“AI 自动归类”替本切口加分。[同任务运营方法][alert-about]

市场边界：Census 的 2024 年统计列出美国可识别进口企业 **240,535 家**，其中中小企业 **234,023 家**。这只是行业背景，包含不同规模和贸易模式；“从中国重复补货、有确定编码、缺监控且愿买软件”的目标企业数**未找到**，不拿大盘乘占有率推收入。[官方报告第 4 页及表 6d][census]

【试验经济假设，非预测】试价 **$29/月、最多 30 个编码＋原产地组合**，参考同任务公开价，仍需付款验证。[价格参照][port] 若每账户每月支持 20 分钟，按内部工时 $30/小时记 $10，再假设数据及邮件 $3、收款等 $2，则单位贡献为 **$29−$10−$3−$2＝$14/月**；100 个付费账户月收入 $2,900、单位贡献合计 $1,400，尚未扣固定监控维护、获客、专业复核、税和创始人工资。所有成本、账户数是试验设定，实际值**未找到**。若要求三个月回收获客费，可承受 CAC 仅 **$14×3＝$42**；所以不能先铺内容再等收入。

### 5. 最小验证：先证明付费，再分别证明复用、续费和 SEO

以下全部是**拟执行阈值，不是已完成结果**。本轮只调查与制备报告，没有联系用户、收款、注册竞品账户或测试真实提醒。

| 验证项 | 最小动作／通过条件 | 停止或调整条件 |
|---|---|---|
| 可交付性 | 用官方历史通知与专业复核建立 20 个变更／不变更对照案例；检查适用商品、条件、生效日和来源。再将同一小目录与免费 Radar、HTSAlert 对照。 | 严重漏报、把不确定条件写成确定税率，先暂停对外自动发送并修复；若依赖大量逐票人工才能交付，停止当前 SaaS 方案。 |
| **首付** | 14 天内约访 10 家符合画像的进口商，让其看自己商品的真实样例与免费替代；至少 3 家预付一个月 $29，并说清为“监控提醒”购买的差异。 | 未达门槛先改画像或价值；若客户普遍只为归类、退税或人工咨询付款，则当前切口未通过，不挪相邻收入补证。 |
| **复用** | 首月记录各账户是否维持有效商品目录、核看提醒并完成复核／采购动作；至少 2 家在另一补货节点继续使用同一监控任务。无真实变化时记录目录复核，不制造假通知。 | 只用第一次导入／演示，后续无经营动作；或支持时间持续超过上述成本假设，重新评估。套餐内再次使用只算复用，不算再付款。 |
| **续费** | 到第二、第三个账期再看实际成功扣款；至少 2/3 的首付客户各续两个账期，单列退款、失联、拒续原因。 | 没到扣款周期就写“未验证”；免费延长、自动续费开关和口头承诺都不算。小样本通过也只支持继续试点。 |
| SEO | 首付和交付通过后，先上线承接上述 5 个同任务表达的一个工具落地页，配少量有依据的用法页；观察 8 周 Search Console 意图、真实目录导入和付款来源。 | 若查询始终只要免费查码/计算器，就不扩内容量；未被索引或无曝光先查技术与数据，不能直接判需求不存在。没有付费来源前不按排名推收入。 |

免费工具若在目标客户实际对照中已经足够、客户也满意，且没有愿付费的同任务差异，应停止这个收费切口；本轮尚未取得这样的满意度证据。**成熟 PMF 的前置门槛目前未过，建议级别为“验证”，不是“推荐开发”。**

## 附录：评分、审计与词表

### A. 综合评分与旧结论修正

【内部研究判断】按现行五项等权折算：**(4＋3＋2＋3＋3)÷25×100＝60/100**。只评本次监控任务。该总分没有单独的 SEO 权重，不能冒充 SEO 优先级；三维决策优先。

| 旧依据 | 本次处理 |
|---|---|
| 专员 22/25；旧深挖 65.5/100 | 范围与评分维度不同，不能直接作同口径升降。原文件随证据包保留。 |
| 15,000 件商品归类缓慢 | 原话可核，讨论的是批量归类，排出当前任务。[原帖][r-classify] |
| 顾问高小时费证明本切口付费 | 价格讨论可核，但买的是清关／归类咨询，不计监控付费。[原帖][r-consult] |
| smallbusiness “painful／surprise bill at the port” | 本次仍**未找到**所引两句；当前是调研主文，不能当主动投诉。[原帖][r-small] |
| “Pick one code…document why…”旧报告称未找到 | 本次在评论中找到，但该帖涉及英国混合商品归类；不计美国监控需求，且不采纳为合规建议。[原帖][r-mixed] |
| Incoclyse 证明小进口商软件需求 | 帖内开发者自述及资料准备讨论，不证明监控付费。[原帖][r-invoice] |
| 年轻域名／查码高量支持容易做 SEO | 均撤出该结论。原 SERP 甚至将 `hs code software` 返回为编程网站，`customs duty calculator` 返回为通用计算器；这些结果无效于当前任务。原始页与最终表分开保存。 |

### B. 搜索量四态与完整国家覆盖

原始 **578 条市场×词记录**来自用户给定的快照：**124 条返回正数、367 条标“供应商返回0”、87 条未返回、0 条未查询**。由于上述采集器问题，367 条“0”均待核；最终口径为 **124 条正数、0 条可确认供应商数值0、454 条未返回/待核、0 条未查询**。这是本次文件审计，不是供应商声称“全部未返回”，也不是这些词没有需求。新增公开网页补查表达未查询月量，单独记“未查询”，不并入原 578 条。[量数据接口来源][volapi]

| 市场／语言 | 原记录数 | 原正数 | 原标0待核 | 原未返回 | 同类监控表达（观察，不计美国主评分） |
|---|---:|---:|---:|---:|---|
| US／英语 | 61 | 23 | 38 | 0 | 上文五个主任务词，仅这五词进入主判断 |
| UK／英语 | 61 | 22 | 39 | 0 | tariff change alerts；当地税制未纳入当前交付 |
| CA／英语 | 61 | 23 | 38 | 0 | tariff monitoring software；当地税制未纳入当前交付 |
| AU／英语 | 61 | 20 | 41 | 0 | import duty change notifications；当地税制未纳入当前交付 |
| DE／德语 | 48 | 12 | 31 | 5 | Änderungen Zolltarifnummer überwachen；兼有编码变更歧义 |
| FR／法语 | 48 | 1 | 41 | 6 | alertes modifications tarifaires douanières |
| ES／西语 | 48 | 3 | 45 | 0 | alertas de cambios arancelarios |
| IT／意语 | 48 | 6 | 42 | 0 | monitoraggio variazioni dazi doganali |
| NL／荷语 | 48 | 8 | 34 | 6 | wijzigingen invoerrechten volgen |
| JP／日语 | 47 | 1 | 2 | 44 | 関税率 変更 通知；本词原状态就是“未返回” |
| KR／韩语 | 47 | 5 | 16 | 26 | 관세율 변경 알림 |

上表是**采集完整性审计**，不加总为主任务搜索量。其余词按输入输出移入相邻任务，不重新打其他赛道分。完整逐词原值、最终状态、排除理由、样本链接在附件 `final-judgments.json` 和 `serp.md`；供应商数据需要认证，本轮没有可公开核验每条月量的网页，公开数值复核入口**未找到**。[供应商接口][volapi]

SERP 共取得 **129 组**原始结果，其中 **116 组 9 条、12 组 8 条、1 组 10 条**；本次主任务已有的四组均为 9 条。不能把全体 129 组、其他国家或相邻计算器的结果算成当前竞争样本。低量核心词仍检查意图和产品；其余外围词沿用单市场 >200 的原采集门槛，排除词不补查。

### C. 最终口径与缺失证据

- 唯一最终判定表为 `final-judgments.json`；`serp.json` 已同步同一内容，`serp.md` 由它生成。旧标签保留在 `raw_*` 字段与 `evidence/original-serp.*`，不再用于最终汇总。原 `kw/core.txt` 含多个任务，仅作为历史输入；当前五个核心词另存 `evidence/final-core.txt`。
- 域名注册时间来自原供应商 RDAP 快照，本轮复核未成功；不以四舍五入的年龄判断是否刚好满一年。DR 未用于主结论。可靠自然流量、搜索转化率、直接产品的可审计营收及续费，均**未找到**。
- Arctic Shift 无全量；Reddit 当前精确日期、票数、评论总数缺失已逐项标明。网站页面与搜索缓存可能处于不同版本，HTS Hero 定价冲突已保留，不掩盖。
- 证据包含原报告、SOP、筛选标准、Reddit 方法、原/最终 SERP、原关键词、公开网页摘录、采集代码、重试日志、试验参数与计时。公开报告托管链接：**未找到（本轮未发布）**；核心事实均提供上文可访问的官方／产品／原帖入口。

### D. 用时

<!-- TIMING -->

[r-monitor]: https://www.reddit.com/r/FulfillmentByAmazon/comments/1uscjoe/how_are_you_guys_actually_keeping_up_with_tariff/
[r-manual]: https://www.reddit.com/r/Alibaba/comments/1tr9wko/anyone_here_actually_tracking_tariffhscode/
[r-research]: https://www.reddit.com/r/smallbusiness/comments/1v1ixzf/importersdropshippers_has_a_tariff_or_duty_change/
[r-builder]: https://www.reddit.com/r/AmazonFBA/comments/1sf8s21/how_are_you_tracking_tariff_changes_on_your/
[r-classify]: https://www.reddit.com/r/CustomsBroker/comments/1pdgve2/importers_requesting_classifications_in_advance/
[r-consult]: https://www.reddit.com/r/CustomsBroker/comments/1q25i9k/how_much_cost_a_customs_broker_hts_classification/
[r-small]: https://www.reddit.com/r/smallbusiness/comments/1svt2lz/how_are_you_currently_handling_hts_codes_tariff/
[r-mixed]: https://www.reddit.com/r/CustomsBroker/comments/1p5f1z1/struggling_with_hs_codes_for_mixed_imports_anyone/
[r-invoice]: https://www.reddit.com/r/importexport/comments/1pn5usz/small_importers_what_do_you_usually_prepare/
[archive]: https://www.usitc.gov/harmonized_tariff_information/hts/archive/list
[csms-doc]: https://www.cbp.gov/sites/default/files/documents/ACE101_June_4_Presentation_Slides.pdf
[arctic]: https://arctic-shift.photon-reddit.com/api/posts/search?subreddit=CustomsBroker&after=2026-04-24&before=2026-10-25&limit=100
[volapi]: https://api.pxany.com/v1/keyword-volumes
[google-monitor]: https://www.google.com/search?q=tariff+alerts+by+hts+code&gl=us&hl=en
[alert]: https://htsalert.com/
[alert-about]: https://htsalert.com/about
[hero]: https://htshero.com/
[hero-monitor]: https://htshero.com/tariff-monitor
[hero-old]: https://htshero.com/pricing-calculator
[port]: https://www.portrobin.com/pricing
[quick-price]: https://quickcode.ai/pricing/
[quick-case]: https://quickcode.ai/case-study-field-fastener-transforms-classifications-tariff-accuracy/
[radar]: https://www.customsgenius.com/radar
[us-alerts]: https://ustariffrates.com/alerts
[classify-alerts]: https://tariffclassify.ai/tariff-rate-alerts
[import-alerts]: https://www.importcostcalculator.com/tariff-alerts.html
[ginger]: https://gingercontrol.com/products/compliance-radar
[ruling]: https://rulings.cbp.gov/api/getdoc/hq/2026/H350722.pdf
[census]: https://www.census.gov/foreign-trade/Press-Release/edb/edbrel2024.pdf
[rdap-cg]: https://rdap.verisign.com/com/v1/domain/CUSTOMSGENIUS.COM
[rdap-us]: https://rdap.verisign.com/com/v1/domain/USTARIFFRATES.COM
[rdap-ic]: https://rdap.verisign.com/com/v1/domain/IMPORTCOSTCALCULATOR.COM
