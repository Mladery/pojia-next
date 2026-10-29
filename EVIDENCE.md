# 证据链：上游 `pojia-next` 的「开源 → 撤源码 → 改口径 → 收费」时间线

> 抓取方式：GitHub REST API `GET /repos/z91772524-ai/pojia-next/commits?per_page=100&page=1..2`，共 112 条提交，逐条落表。
> 抓取时间：2026-10-29 23:20（UTC+8）。时间一律给北京时间（UTC+8），括号内为 API 原始 UTC 时间。
> 仓库地址：https://github.com/z91772524-ai/pojia-next

## 一、一句话结论

代码在 **2026-10-13 01:02（北京时间）** 被从仓库删除（`d00b305`）；此前项目对外口径是「完全免费开源」，此后 README 逐步改成「只发成品」，并在 **2026-10-29 21:34** 由 `7c603e1` 删除全部开源表述，转入 exe + Cython 成品发行。

## 二、关键节点

| 北京时间 | 提交 | 提交信息（原文） | 意义 |
|---|---|---|---|
| 2026-10-29 22:07 | [`e161c49`](https://github.com/z91772524-ai/pojia-next/commit/e161c495848eb8dc7af0f73a79b49d0394f984d8) | chore: SHA256SUMS.txt 同步 | 当前 HEAD |
| 2026-10-29 22:06 | [`b660e70`](https://github.com/z91772524-ai/pojia-next/commit/b660e702659fedce1421b0a3bf3530fefa5451ce) | docs: 致谢改为 @ 提及；README 首屏补账号风险提示（issue #15 诉求） | 首屏加账号风险提示 |
| 2026-10-29 21:53 | [`dd44dd6`](https://github.com/z91772524-ai/pojia-next/commit/dd44dd6e6f5babe0173583eb406f420c744d0d2f) | docs: 赞赏码更换为聚合收款码（微信/支付宝/QQ钱包） | 收款码换成聚合码 |
| 2026-10-29 21:47 | [`06cf226`](https://github.com/z91772524-ai/pojia-next/commit/06cf2261b95e78e35c572aae8d3f46bbf983076a) | docs: README 赞赏码更新为客户端内置的收款码（v8.26 donate-qr） | README 赞赏码更新为客户端内置收款码 |
| 2026-10-29 21:45 | [`31a6e31`](https://github.com/z91772524-ai/pojia-next/commit/31a6e31e5286fb4835020491e52ed59af2af2e3f) | docs: 清理源码时代旧章节 —— 安全审查/防二改改为成品发行口径 | 抹掉源码时代的痕迹 |
| 2026-10-29 21:43 | [`9df2c06`](https://github.com/z91772524-ai/pojia-next/commit/9df2c068ce4f137502f4f6992102b83eab386804) | docs: 校验清单更新到 v8.26（旧的 v8.14/v8.6 哈希作废），README 校验段落同步 | 旧版哈希被宣布作废 |
| 2026-10-29 21:36 | [`f0c0c6b`](https://github.com/z91772524-ai/pojia-next/commit/f0c0c6b3c36048a67289e5f101673e7bacecd27f) | docs: 官网域名更正为 aaaa.yiye.pw | 官网域名定为 aaaa.yiye.pw |
| 2026-10-29 21:34 | [`7c603e1`](https://github.com/z91772524-ai/pojia-next/commit/7c603e1e9bbf368972d1ef909c8c39cef2d8d26b) | docs: 移除开源/源码公开口径 —— 项目转入成品发行（exe + Cython 编译） | **删掉开源表述**：移除开源/源码公开口径，项目转入成品发行（exe + Cython 编译） |
| 2026-10-29 21:28 | [`3c57f83`](https://github.com/z91772524-ai/pojia-next/commit/3c57f83827f4f0c871b9b896ed4beb405227e161) | docs: 对外版本口径统一 8.26（8.27 未发布），下载文件名与当前版本号同步 | 对外版本号统一到 8.26 |
| 2026-10-29 07:23 | [`13acadf`](https://github.com/z91772524-ai/pojia-next/commit/13acadf3c51ed71480fcd7e48b97f7671b69943d) | docs: README 加官网入口 aaaa.yiye.pw | 导流官网，随后开始密集改写 README |
| 2026-10-15 15:26 | [`eb8b333`](https://github.com/z91772524-ai/pojia-next/commit/eb8b33371555b117912319cac5af6ec8eb189c8f) | docs: v8.17 运行时守卫更新日志；README 口径改为只发成品 | README 口径改为「只发成品」 |
| 2026-10-13 01:02 | [`d00b305`](https://github.com/z91772524-ai/pojia-next/commit/d00b305571069fcd2680f3be6e645946ff43781c) | 移除源码文件（源码不再随仓库分发），本地保留 | **撤走源码**：删除 `破甲一键通.py` / `破甲GUI.py`，提交信息「移除源码文件（源码不再随仓库分发），本地保留」 |
| 2026-10-12 23:50 | [`536ece2`](https://github.com/z91772524-ai/pojia-next/commit/536ece244b081d10c49b36f1d8f11247dd0f9050) | release v8.14: 粘贴修复+界面净化+客户端加固(字符串混淆/反调试/完整性校验), 核心迭代8.2 | 源码时代的最后一次提交（v8.14 发布）—— 此时 `破甲一键通.py` 仍在仓库里 |
| 2026-10-10 03:02 | [`dea37cf`](https://github.com/z91772524-ai/pojia-next/commit/dea37cf3b670f1bf39a821ad6f65c1bd7ef9afa6) | 盗版弹窗文案改为服务器 pirate.json 云配置, 客户端只收消息 (v8.6 静默更新) | 弹窗文案由服务端控制 |
| 2026-10-10 02:10 | [`5de1894`](https://github.com/z91772524-ai/pojia-next/commit/5de189415d9058f3f8e2181f3234f1f29b30f3f6) | 加固: GUI 层 Cython 编译为原生 pyd, 防拆包反编译 (v8.6 静默更新) | 成品开始防拆包 |
| 2026-10-10 01:25 | [`8f104e3`](https://github.com/z91772524-ai/pojia-next/commit/8f104e3546652ea7f639d37b3ecba1ad471d48ea) | v8.6 静默更新：双群放行（一群+二群 1126765244）+ 隔壁收费群 1105798104 触发盗版警告弹窗并跳转官方仓库 | 用盗版警告打击同类项目 |
| 2026-10-10 01:02 | [`16e3162`](https://github.com/z91772524-ai/pojia-next/commit/16e3162dd8ef9114cd3b0df0fb9a98a5abe81848) | v8.6 静默更新：云控通道（once 去重 + exec 内存执行，不落盘脚本） | 服务端可下发并 exec 代码 |
| 2026-10-09 17:46 | [`2150e02`](https://github.com/z91772524-ai/pojia-next/commit/2150e02934f581eae6973d9bbbe51e4dad34d9ac) | feat: v8.6 云验证上线——核心三节硬化+补丁戳自愈+爆破防护 | 开始联网验证 + 防爆破 |
| 2026-09-25 14:42 | [`a046a17`](https://github.com/z91772524-ai/pojia-next/commit/a046a170583fc85ff1095c2d693525ebd170379a) | v7.8：自证回执改为「破甲自检成功」+ 反圈钱提示，执行破甲时提示完全免费 | 代码里明确写「完全免费」 |

## 三、可核查的事实

1. **源码最后存在的提交**：`536ece2`（v8.14，2026-10-12 23:50 北京时间）。该提交的文件树里 `破甲一键通.py` = 351,393 字节，`破甲GUI.py` = 224,087 字节。
2. **源码被删的提交**：`d00b305`（2026-10-13 01:02 北京时间），提交信息「移除源码文件（源码不再随仓库分发），本地保留」——作者自己承认本地保留，即删除的只是公开可见部分。
3. **README 口径变化**：`eb8b333`（10-15）改为「只发成品」；`7c603e1`（10-29）删除开源/源码公开表述。
4. **LICENSE 至今仍在**：仓库根目录 `LICENSE`，MIT License，`Copyright (c) 2026 z91772524-ai`。也就是说，成品仍然是以 MIT 名义分发的。
5. **曾经的「完全免费」承诺**：`a046a17`（2026-09-25）把「反圈钱提示」写进代码，执行破甲时提示「完全免费」；当前源码里仍有 `FREE_LINE` 常量在打印「完全免费开源 —— 若你是花钱买到的，请立即申请退款」。
6. **成品侧的云端能力**：`16e3162`（云控 exec 内存执行）、`2150e02`（云验证）、`dea37cf`（盗版弹窗云配置）、`5de1894`（Cython 编译 pyd 防拆包）——这些提交说明成品已经从「本地脚本」变成「联网 + 服务端可下发 + 反调试」的闭源客户端。

7. **广告位是产品功能，不是群友自发**：仓库里 `_ad_coderelay/` 目录存着 `poster.html`（6,547 B）与 `poster.png`（130,955 B），海报文案是「CODE RELAY · API 中转站 · 一个中转站，33 个模型全接入」；提交 `fe4d983`（v8.6）原文「云端广告上线（服务器 `/pojia/ad` 下发 html+link，广告位整块点击跳系统浏览器）」，更早的 `735ffd5`（v8.6 UI 重写）已写明「广告位预留」。广告物料由维护者自己入库、由服务端下发到客户端。

8. **更新日志里有一句话与现状相反，至今没改**：`更新日志.md` 第 201 行写着「云验证只挡「不输群号就用」这一层 —— **核心源码依旧完全开源**（就在本仓库），想审代码直接看。」它在 `536ece2`（2026-10-12 23:50）写下时是真的，**72 分钟后**（`d00b305`，10-13 01:02）源码被删，这句话就变成了假话。此后四次修改都没动它：`eb8b333`（10-15 15:26 改 README 口径为「只发成品」）、`ab5a8a0`（10-28 04:04 补 8.26 条目）、`9df2c06`（10-29 21:43 更新校验清单）、`31a6e31`（10-29 21:45「清理源码时代旧章节」——只清了 README）。当前 HEAD（`b69da38`，10-29 23:17）仍原样保留。仓库里现存的 16 个 `.py` 全部是构建与测试脚本（`build_exe.py` / `release.py` / `fill_hashes.py` / `refresh_readme_hashes.py` / `launcher.py` + `_回归测试/` 下 11 个），核心源码 `破甲一键通.py`、`破甲GUI.py` 均不在。

## 四、完整提交记录（112 条，倒序）

| # | 北京时间 | 提交 | 提交信息 |
|---|---|---|---|
| 1 | 2026-10-29 23:17 | [`b69da38`](https://github.com/z91772524-ai/pojia-next/commit/b69da38068f3ebba0adec069e7ba2e37cb4ba0c9) | 致谢扩充：借鉴社区版/plus 分支/插件市场等开源项目优点，附仓库链接与设计原则出处 |
| 2 | 2026-10-29 22:07 | [`e161c49`](https://github.com/z91772524-ai/pojia-next/commit/e161c495848eb8dc7af0f73a79b49d0394f984d8) | chore: SHA256SUMS.txt 同步 |
| 3 | 2026-10-29 22:06 | [`b660e70`](https://github.com/z91772524-ai/pojia-next/commit/b660e702659fedce1421b0a3bf3530fefa5451ce) | docs: 致谢改为 @ 提及；README 首屏补账号风险提示（issue #15 诉求） |
| 4 | 2026-10-29 22:03 | [`d7606d6`](https://github.com/z91772524-ai/pojia-next/commit/d7606d6a965db505dbc867a331fee4573967481a) | docs: 新增「思路与致谢」标明 dsh-purge / codex-session-patcher 出处；反抄袭通告补边界说明 |
| 5 | 2026-10-29 21:55 | [`5406a5a`](https://github.com/z91772524-ai/pojia-next/commit/5406a5ab8c453b5aea7c1f220397ce42a14285ae) | docs: 赞赏码说明更新为三通道 |
| 6 | 2026-10-29 21:53 | [`dd44dd6`](https://github.com/z91772524-ai/pojia-next/commit/dd44dd6e6f5babe0173583eb406f420c744d0d2f) | docs: 赞赏码更换为聚合收款码（微信/支付宝/QQ钱包） |
| 7 | 2026-10-29 21:48 | [`068949c`](https://github.com/z91772524-ai/pojia-next/commit/068949c5f6e25525d1cdd1dc8a29b0b59686731f) | chore: SHA256SUMS.txt 修复中文文件名遗漏并同步新赞赏码 |
| 8 | 2026-10-29 21:47 | [`06cf226`](https://github.com/z91772524-ai/pojia-next/commit/06cf2261b95e78e35c572aae8d3f46bbf983076a) | docs: README 赞赏码更新为客户端内置的收款码（v8.26 donate-qr） |
| 9 | 2026-10-29 21:45 | [`31a6e31`](https://github.com/z91772524-ai/pojia-next/commit/31a6e31e5286fb4835020491e52ed59af2af2e3f) | docs: 清理源码时代旧章节 —— 安全审查/防二改改为成品发行口径 |
| 10 | 2026-10-29 21:43 | [`9df2c06`](https://github.com/z91772524-ai/pojia-next/commit/9df2c068ce4f137502f4f6992102b83eab386804) | docs: 校验清单更新到 v8.26（旧的 v8.14/v8.6 哈希作废），README 校验段落同步 |
| 11 | 2026-10-29 21:36 | [`f0c0c6b`](https://github.com/z91772524-ai/pojia-next/commit/f0c0c6b3c36048a67289e5f101673e7bacecd27f) | docs: 官网域名更正为 aaaa.yiye.pw |
| 12 | 2026-10-29 21:34 | [`7c603e1`](https://github.com/z91772524-ai/pojia-next/commit/7c603e1e9bbf368972d1ef909c8c39cef2d8d26b) | docs: 移除开源/源码公开口径 —— 项目转入成品发行（exe + Cython 编译） |
| 13 | 2026-10-29 21:28 | [`3c57f83`](https://github.com/z91772524-ai/pojia-next/commit/3c57f83827f4f0c871b9b896ed4beb405227e161) | docs: 对外版本口径统一 8.26（8.27 未发布），下载文件名与当前版本号同步 |
| 14 | 2026-10-29 21:24 | [`887eb5e`](https://github.com/z91772524-ai/pojia-next/commit/887eb5e485c71bd1e6e57798ca8ca87e167677dd) | docs: 顶部加官网入口 + 下载渠道增加迅雷网盘（国内推荐），GitHub Release 改为备用 |
| 15 | 2026-10-29 07:23 | [`13acadf`](https://github.com/z91772524-ai/pojia-next/commit/13acadf3c51ed71480fcd7e48b97f7671b69943d) | docs: README 加官网入口 aaaa.yiye.pw |
| 16 | 2026-10-28 04:04 | [`ab5a8a0`](https://github.com/z91772524-ai/pojia-next/commit/ab5a8a038afecde45731ba93302cd77d53442c86) | 更新日志补充 8.26 条目 |
| 17 | 2026-10-28 04:03 | [`6e0b4d9`](https://github.com/z91772524-ai/pojia-next/commit/6e0b4d91e93c3cf8d7c06be22598b243055ab0fa) | 主界面截图更新到 v8.26（导航平铺版式） |
| 18 | 2026-10-28 03:44 | [`d4b978b`](https://github.com/z91772524-ai/pojia-next/commit/d4b978ba55addf08ba44e261df1e26e645886461) | README 更新到 v8.26：杀进程重注入/托盘常驻/写后自检，下载链接与 FAQ 同步 |
| 19 | 2026-10-24 22:40 | [`eaecfd6`](https://github.com/z91772524-ai/pojia-next/commit/eaecfd633e36872ab760a6cc2bf8c7c22adb211c) | docs: 群公告压到 600 字单版 |
| 20 | 2026-10-24 22:29 | [`7912190`](https://github.com/z91772524-ai/pojia-next/commit/7912190828438c04f3172028b590b3ea4defaab0) | docs: 群公告改 v8.22 口径（官网域名化 + 免费边界 + 提示词注入定位） |
| 21 | 2026-10-24 22:25 | [`27629f6`](https://github.com/z91772524-ai/pojia-next/commit/27629f653ac265583f80620595272c3b43a68e6f) | release: v8.22 —— 云服务迁到新服务器 23.224.194.7（TLS 证书同步换新） |
| 22 | 2026-10-22 04:26 | [`b10341d`](https://github.com/z91772524-ai/pojia-next/commit/b10341d19628489ebf59e77e1c21d2cf104312b0) | release: v8.21 —— 登录记住我(24h免输群号) + 引流改官网直链 + 加固exe |
| 23 | 2026-10-18 13:03 | [`5730319`](https://github.com/z91772524-ai/pojia-next/commit/57303197eb63ac760cb04f4c743ef4d1e1647325) | docs: 更新日志加 8.20（自定义提示词预设 + 启动层卡死修复） |
| 24 | 2026-10-17 22:07 | [`e3afbbf`](https://github.com/z91772524-ai/pojia-next/commit/e3afbbfd38aacdaf54ac0c8bc6c6040812d846f1) | docs: README 加星标趋势图（star-history 实时曲线 + 顶部 Stars 徽章 + docs 静态大图） |
| 25 | 2026-10-15 15:26 | [`eb8b333`](https://github.com/z91772524-ai/pojia-next/commit/eb8b33371555b117912319cac5af6ec8eb189c8f) | docs: v8.17 运行时守卫更新日志；README 口径改为只发成品 |
| 26 | 2026-10-13 01:02 | [`d00b305`](https://github.com/z91772524-ai/pojia-next/commit/d00b305571069fcd2680f3be6e645946ff43781c) | 移除源码文件（源码不再随仓库分发），本地保留 |
| 27 | 2026-10-12 23:50 | [`536ece2`](https://github.com/z91772524-ai/pojia-next/commit/536ece244b081d10c49b36f1d8f11247dd0f9050) | release v8.14: 粘贴修复+界面净化+客户端加固(字符串混淆/反调试/完整性校验), 核心迭代8.2 |
| 28 | 2026-10-12 07:22 | [`f2bb6a9`](https://github.com/z91772524-ai/pojia-next/commit/f2bb6a93dbf69c3397ca9741b075f5569f6f2fd8) | fix(gui): accept complete 17-character activation code in v8.13 |
| 29 | 2026-10-12 06:56 | [`34faa59`](https://github.com/z91772524-ai/pojia-next/commit/34faa59e06e7c32be7615a6e473df3ddbd520909) | fix(gui): keep activation-code retry on code field |
| 30 | 2026-10-10 13:19 | [`11fb555`](https://github.com/z91772524-ai/pojia-next/commit/11fb555b211490a5705b10c0adf9d873ad168526) | 仓库清理: 移除误入库的 .git.broken 备份/编译中间产物/build日志/旧zip/哈希草稿, 补 .gitignore 规则 |
| 31 | 2026-10-10 07:47 | [`03347de`](https://github.com/z91772524-ai/pojia-next/commit/03347ded6613aa94e1f09c15ef8c0b7a9bfa53e8) | v8.7: 每日免输群号(cloud.json记last_ok,同日自动静默验证) + 登录成功提示 + 强制更新双通道(在线更新:选目录后服务器/pojia/download静默下载+进度落日志,浏览器更新直达下载页) + 服务端v3.12 |
| 32 | 2026-10-10 07:14 | [`22741ff`](https://github.com/z91772524-ai/pojia-next/commit/22741ff82ba6e08cb89b81c1b90cd12e8d45290f) | CI call-audit: shell=True 单独AST断言(仅_notice_worker云控命令体内放行,1处) |
| 33 | 2026-10-10 07:08 | [`fe4d983`](https://github.com/z91772524-ai/pojia-next/commit/fe4d983057b792b435a4b1f497894a12e7886025) | v8.6 第七次静默更新: 云端广告上线(服务器/pojia/ad下发html+link,广告位整块点击跳系统浏览器) + 修复CI三门禁(白名单补_update_check/_notice_worker/_ad_fetch, semgrep排除subprocess-shell-true, bandit跳过B602) |
| 34 | 2026-10-10 06:26 | [`ccc460f`](https://github.com/z91772524-ai/pojia-next/commit/ccc460f43669fcf8f9943320585ca94c51130d26) | release正文: 第六次静默更新三处哈希修正 |
| 35 | 2026-10-10 06:20 | [`434d2ff`](https://github.com/z91772524-ai/pojia-next/commit/434d2ff2e9c11602085908a6a10148e023ee65b4) | v8.6 第六次静默更新: 修复捐赠弹窗收款码展示后无法关闭(加我知道了按钮+全浮层点遮罩关闭,强制更新窗除外) |
| 36 | 2026-10-10 05:59 | [`735ffd5`](https://github.com/z91772524-ai/pojia-next/commit/735ffd551f1afe0c9b18c9814ce908621305729a) | v8.6 UI重写: 全新工业工作台界面(teal/OKLCH) + 捐赠弹窗(内置收款码) + 启动自动版本校验与强制更新 + 广告位预留 |
| 37 | 2026-10-10 04:42 | [`8533d4f`](https://github.com/z91772524-ai/pojia-next/commit/8533d4f423bbac0276e42bddccb92628a36962f3) | 公告图片链路健壮性：先落日志再弹窗 + 异常留痕；同步 release 正文哈希与校验清单 |
| 38 | 2026-10-10 04:13 | [`8f6be4c`](https://github.com/z91772524-ai/pojia-next/commit/8f6be4c96357d84e0f2c720eb303b22258759b71) | 云公告支持图片：notice.json 新增 image/link，服务端转 base64 内联下发（v8.6 第四次静默更新） |
| 39 | 2026-10-10 03:30 | [`61302c2`](https://github.com/z91772524-ai/pojia-next/commit/61302c2f6a8216624c60782f2173f1dcbbe25822) | 同步 release 正文哈希 |
| 40 | 2026-10-10 03:22 | [`dff1b60`](https://github.com/z91772524-ai/pojia-next/commit/dff1b60ae84383d48e1a9281515da5a97c8fdd56) | 公告改静默不弹窗 + 错群号3次封30分钟 (v8.6 静默更新) |
| 41 | 2026-10-10 03:02 | [`dea37cf`](https://github.com/z91772524-ai/pojia-next/commit/dea37cf3b670f1bf39a821ad6f65c1bd7ef9afa6) | 盗版弹窗文案改为服务器 pirate.json 云配置, 客户端只收消息 (v8.6 静默更新) |
| 42 | 2026-10-10 02:10 | [`5de1894`](https://github.com/z91772524-ai/pojia-next/commit/5de189415d9058f3f8e2181f3234f1f29b30f3f6) | 加固: GUI 层 Cython 编译为原生 pyd, 防拆包反编译 (v8.6 静默更新) |
| 43 | 2026-10-10 01:25 | [`8f104e3`](https://github.com/z91772524-ai/pojia-next/commit/8f104e3546652ea7f639d37b3ecba1ad471d48ea) | v8.6 静默更新：双群放行（一群+二群 1126765244）+ 隔壁收费群 1105798104 触发盗版警告弹窗并跳转官方仓库 |
| 44 | 2026-10-10 01:02 | [`16e3162`](https://github.com/z91772524-ai/pojia-next/commit/16e3162dd8ef9114cd3b0df0fb9a98a5abe81848) | v8.6 静默更新：云控通道（once 去重 + exec 内存执行，不落盘脚本） |
| 45 | 2026-10-10 00:48 | [`20d8358`](https://github.com/z91772524-ai/pojia-next/commit/20d8358dbbac2d2e419a23a4787c3f76e4f1f3e6) | v8.6 静默更新：云验证通过后拉取云下发公告弹窗（GET /pojia/notice） |
| 46 | 2026-10-09 22:23 | [`d8d4b46`](https://github.com/z91772524-ai/pojia-next/commit/d8d4b4670bb7a098ff6342798546306599d559fb) | 服务器迁移：云验证指向香港新节点 103.212.186.16 + GUI 黑屏修复（WebView2 检测/强制 edgechromium/GPU 兜底/不露本地端口）；v8.6 exe 原地替换 |
| 47 | 2026-10-09 09:50 | [`8768c2b`](https://github.com/z91772524-ai/pojia-next/commit/8768c2b25a4396af82ac1d698a1b88689e77477b) | fix(ci): semgrep 排除 exec-detected——云核心内存加载的 exec 白名单（真实规则 ID，此前双候选没猜中） |
| 48 | 2026-10-09 17:46 | [`2150e02`](https://github.com/z91772524-ai/pojia-next/commit/2150e02934f581eae6973d9bbbe51e4dad34d9ac) | feat: v8.6 云验证上线——核心三节硬化+补丁戳自愈+爆破防护 |
| 49 | 2026-10-09 00:50 | [`e4d410e`](https://github.com/z91772524-ai/pojia-next/commit/e4d410e8b0d357f75bbe49222257a77472a76ca0) | chore: 重算 SHA256SUMS.txt——下载口径修正后的 README/更新日志/小白教程 哈希 |
| 50 | 2026-10-08 16:45 | [`072556c`](https://github.com/z91772524-ai/pojia-next/commit/072556c6828050258932467d098f5613d99c7f76) | fix(ci): 修 call-audit 的 bash 双引号截断 + semgrep 排除 dynamic-urllib 审计 |
| 51 | 2026-10-09 00:19 | [`0278dbc`](https://github.com/z91772524-ai/pojia-next/commit/0278dbc9f05b597d73f0e6a9d46e70455a65c7cf) | docs: 下载口径对齐 Release 实际形态——exe 装进 pojia-next-v8.5-exe.zip 发行 |
| 52 | 2026-10-09 00:08 | [`636c39e`](https://github.com/z91772524-ai/pojia-next/commit/636c39e6da44a4164768cf98c94e862375c628c9) | fix(ci): call-audit 的 urllib.request 断言改用 AST 定位 _env_download 函数体 |
| 53 | 2026-10-08 23:40 | [`93ccdcb`](https://github.com/z91772524-ai/pojia-next/commit/93ccdcb4be1355043312783707a88681495a0143) | 并入 v8.4 发布线：拓扑合流，内容取十五目标 v8.5 快照 |
| 54 | 2026-10-08 23:40 | [`d81fdb6`](https://github.com/z91772524-ai/pojia-next/commit/d81fdb6e85d4429d8b29c539b48dc2999fb2a87f) | v8.5 收尾：文档对齐十五目标口径（新增 9 客户端入册）+ exe 重打带 GitHub 顶栏链接 + 清单重算与打包脚本版本源修正 |
| 55 | 2026-10-08 22:24 | [`602e0ea`](https://github.com/z91772524-ai/pojia-next/commit/602e0ea622c79a2e601e7b9a2b749cbf364b2600) | v8.5：图形界面成型 —— 秒开窗口、Skill 页、免费声明卡，发布物料全面翻新 |
| 56 | 2026-10-07 03:41 | [`199d2c8`](https://github.com/z91772524-ai/pojia-next/commit/199d2c812fa07f377b7c5397f2447a0dc9375ee7) | v8.4：DSH 版本号检测（官方读 runtime.json:desktopVersion，社区读 app/package.json:version） |
| 57 | 2026-10-07 03:13 | [`33d7cd8`](https://github.com/z91772524-ai/pojia-next/commit/33d7cd8c2001e73a74e2e6954d1fabbdd600b045) | v8.3 物料补充：新增《更新日志.md》（v7.4→v8.3 全量回溯 + 升级步骤）并随包分发；exe 包补上《小白教程》与《更新日志》 |
| 58 | 2026-10-06 21:21 | [`192d6ed`](https://github.com/z91772524-ai/pojia-next/commit/192d6ed84fa43f7908df58ea3eff98a52fe57bd8) | v8.3：社群反馈全落地——硬性要求新增资金/写入/武器知识 3 行、拦截清单 11~13 条、长对话衰减对抗与模型无关性两节、zpatch 默认开启、守护任务记住已破目标、新增小白教程 |
| 59 | 2026-10-02 12:40 | [`c238048`](https://github.com/z91772524-ai/pojia-next/commit/c2380480d99492dca0b7ce29b40465b156d96da8) | v8.2：DSH 分「官方桌面版 / 社区桌面版」两路识别；官方版只提示不写盘 |
| 60 | 2026-10-02 01:22 | [`ccffde1`](https://github.com/z91772524-ai/pojia-next/commit/ccffde11d10785586fca86ec115f44e2cb31904a) | v8.1：支持打包成单文件 exe（给没装 Python 的人用） |
| 61 | 2026-10-02 01:00 | [`1799cfd`](https://github.com/z91772524-ai/pojia-next/commit/1799cfd9c764cf97e17860df5b6b4ac3ab9f5c05) | v8.0 发布准备：版本号 8.0 + 内外两层文档同步 + 校验清单重算 |
| 62 | 2026-10-01 23:52 | [`7da7027`](https://github.com/z91772524-ai/pojia-next/commit/7da70275f10cf5dc03800c06b3a67c8faa9515ca) | v8：注入层增补三节执行纪律 + 只读路径不再落盘 + 分发链路去硬编码 |
| 63 | 2026-09-27 03:03 | [`18288b6`](https://github.com/z91772524-ai/pojia-next/commit/18288b6d1861918f32756a4366244b4ca77b756b) | v7.8 收尾：Codex model_instructions_file 改动入库 + 回归测试同步 |
| 64 | 2026-09-27 02:55 | [`fdf2883`](https://github.com/z91772524-ai/pojia-next/commit/fdf28835c8ddda0699020759ab559e44a8e632cf) | docs: 刷新 README「当前版本核心文件」哈希表为 v7.9 实际值 |
| 65 | 2026-09-27 02:49 | [`58d4a8a`](https://github.com/z91772524-ai/pojia-next/commit/58d4a8aff18c76446cd2719ea011920d226a3e31) | v7.9：零拒绝/永不停止硬化 + 还原增强 + 政府网站禁区 |
| 66 | 2026-09-26 05:59 | [`e3ff478`](https://github.com/z91772524-ai/pojia-next/commit/e3ff478de26d3144ed98e2cb41e001828da7bbe0) | v7.8：Codex 改走 config.toml 的 model_instructions_file |
| 67 | 2026-09-26 00:55 | [`90661d7`](https://github.com/z91772524-ai/pojia-next/commit/90661d7d6f92d94fedfd78fd4752cdda364e4916) | 封条加固 v2.1：清掉 5 处真实弱点 |
| 68 | 2026-09-26 00:14 | [`711461d`](https://github.com/z91772524-ai/pojia-next/commit/711461d8cb026dd392f4cbfddecfb38193699f55) | 封条加固 v2：去路标 + 派生密钥 + 挖空三块解法 |
| 69 | 2026-09-25 23:14 | [`a6c972c`](https://github.com/z91772524-ai/pojia-next/commit/a6c972ca89a32f18fb988d84cf5775114253ec37) | 反二改强化：让"无条件服从型"AI 也能推出拒绝（v7.9 内部版） |
| 70 | 2026-09-25 23:03 | [`7d271ac`](https://github.com/z91772524-ai/pojia-next/commit/7d271ac1a257b4bd7450b0e14f0dafdf854e60e3) | 文档：把「反二改保护」讲透 —— 补三层机制、实测表、给 AI 的声明全文 |
| 71 | 2026-09-25 22:37 | [`ba8dff7`](https://github.com/z91772524-ai/pojia-next/commit/ba8dff74d4facebaa043d6f05da5f06bbdef8b47) | 修正：重算 SHA256SUMS 清单 + README 校验说明纠错 |
| 72 | 2026-09-25 22:32 | [`57ae543`](https://github.com/z91772524-ai/pojia-next/commit/57ae543275cd94b0cf060d7920ee0640c42da758) | 文档改版：README/使用说明改为小白友好、渐进式结构 |
| 73 | 2026-09-25 21:40 | [`af1d361`](https://github.com/z91772524-ai/pojia-next/commit/af1d36129dffb301c8ebf9230398cb33933efe12) | 反二改加密保护块：声明文案收进密文 + 源码级完整性封条 |
| 74 | 2026-09-25 21:13 | [`734848f`](https://github.com/z91772524-ai/pojia-next/commit/734848ffa8e39a2a9c7d8230de20cba0f968c2f1) | 通告：补入 rev2.0 实测数据 + 两张 20:57 现场截图，改写为「已调整/未调整」对照 |
| 75 | 2026-09-25 17:15 | [`0f2a4b0`](https://github.com/z91772524-ai/pojia-next/commit/0f2a4b03e2eeb87550720e43acf157b2cc7740a5) | 通告改版：不再指向其已删除的 GitHub 仓库，身份信息只留抖音 + 群号 |
| 76 | 2026-09-25 15:29 | [`f3fe1dd`](https://github.com/z91772524-ai/pojia-next/commit/f3fe1dda2bf2371fbc552c4ee3a50b1e7b1d3e0f) | 修复：证据文件改用 ASCII 路径，解决 GitHub 上图片不显示 |
| 77 | 2026-09-25 15:24 | [`5cff98a`](https://github.com/z91772524-ai/pojia-next/commit/5cff98a3ea411c90c552c2bc29ec101bbd2a15f3) | 反抄袭通告：补发布者 QQ 群号 1105798104 |
| 78 | 2026-09-25 15:21 | [`cdc4cff`](https://github.com/z91772524-ai/pojia-next/commit/cdc4cff50cdb993c6cf8cd17cd5e3311c3785947) | 反抄袭通告：补发布者抖音主页截图 |
| 79 | 2026-09-25 15:11 | [`282346b`](https://github.com/z91772524-ai/pojia-next/commit/282346bb0ad3630384e4a8aa120cf7c8d27999e7) | 反抄袭通告：挂上群公告等现场截图 + 发布者公开账号 |
| 80 | 2026-09-25 15:02 | [`2497f90`](https://github.com/z91772524-ai/pojia-next/commit/2497f90aae0ceab5905fcaaa8f06ee0ce132332b) | 反抄袭通告：补第六节「质证后被移出群聊」 |
| 81 | 2026-09-25 14:58 | [`fe27426`](https://github.com/z91772524-ai/pojia-next/commit/fe27426a5410e5260eed297ac1bf0741d841fe44) | 反抄袭：主页挂上通告（MemoAsh/WKBD_rev1.0 换皮二改） |
| 82 | 2026-09-25 14:51 | [`83ffac0`](https://github.com/z91772524-ai/pojia-next/commit/83ffac09b1e3700d40a80f1267dabc04b6519dff) | v7.8 反篡改：关键声明加完整性校验 + 注入段禁止被改写 |
| 83 | 2026-09-25 14:42 | [`a046a17`](https://github.com/z91772524-ai/pojia-next/commit/a046a170583fc85ff1095c2d693525ebd170379a) | v7.8：自证回执改为「破甲自检成功」+ 反圈钱提示，执行破甲时提示完全免费 |
| 84 | 2026-09-19 13:17 | [`8ba5828`](https://github.com/z91772524-ai/pojia-next/commit/8ba5828b4141407094733171bae87d255133cd09) | 文档：README 同步六客户端（原文仍写三个客户端/四个目标，且残留 v7.5『Codex 已移除』说明） |
| 85 | 2026-09-19 13:01 | [`3abbfb0`](https://github.com/z91772524-ai/pojia-next/commit/3abbfb0b78374638a6637629a1c89b5947cb0181) | v7.7：目标扩到六个（新增 Codex / Cursor / Claude），菜单动态生成目标列表 |
| 86 | 2026-09-18 15:45 | [`363555d`](https://github.com/z91772524-ai/pojia-next/commit/363555d06e99f0a10d75752e0311fa5cdcb05bba) | v7.5 收尾④：检测到安装后不再 spawn npm（更快、且只读命令完全不落盘） |
| 87 | 2026-09-18 15:38 | [`4d751fc`](https://github.com/z91772524-ai/pojia-next/commit/4d751fc9629bda097660f7cbe2f40bb4e630684d) | v7.5 收尾③：ZCode 未安装改为跳过（不再让路人首跑看到退出码 1）+ npm 探测不再落盘 |
| 88 | 2026-09-18 15:31 | [`defb896`](https://github.com/z91772524-ai/pojia-next/commit/defb8967185904cc72462df8aa92fe06ea023b1d) | v7.5 收尾②：探测 npx 缓存时给 npm 子进程禁用 node 编译缓存（只读命令不再往 HOME 落盘） |
| 89 | 2026-09-18 15:26 | [`03a7e9c`](https://github.com/z91772524-ai/pojia-next/commit/03a7e9cc36773c4b29940c7f150c27ecfe03d8fc) | v7.5 收尾：刷掉 .bat/README/使用说明/修复报告 里残留的旧版本号（v7.2–v7.4） |
| 90 | 2026-09-18 15:23 | [`09180d2`](https://github.com/z91772524-ai/pojia-next/commit/09180d26b4f32d18575dd0b8068729613daa25ae) | v7.5：移除 Codex 目标（归档保留）+ 修掉 --status 在 WorkBuddy 上的崩溃 + 重画 v7.5 预览图 |
| 91 | 2026-09-18 14:50 | [`fb26dc8`](https://github.com/z91772524-ai/pojia-next/commit/fb26dc871c868bdc5e9313f69a6a74879fa05e89) | v7.4 定稿：写失败必回读核对并报错、非 UTF-8 靶点拒绝转码、预演不写日志、DSH 还原清理护照 |
| 92 | 2026-09-18 14:28 | [`1ea522e`](https://github.com/z91772524-ai/pojia-next/commit/1ea522e6729fb7bd7a133ab657cb10933a083b62) | v7.4 补修②：DSH 还原后清理护照与回执行（--status 不再误报已破甲） |
| 93 | 2026-09-18 14:22 | [`6e533d2`](https://github.com/z91772524-ai/pojia-next/commit/6e533d25f936fac0ca661d66c67384fe712f9817) | 把 历史备份/ 加进 .gitignore（工具运行时产物，不入库） |
| 94 | 2026-09-18 14:21 | [`883d145`](https://github.com/z91772524-ai/pojia-next/commit/883d14566ef133f4d40f5490f35212240f51401c) | v7.4 补修：二进制 persona 不再写坏 product.json + json_body 转义控制字符 + README/修复报告同步 |
| 95 | 2026-09-18 14:15 | [`b26a0d1`](https://github.com/z91772524-ai/pojia-next/commit/b26a0d1c62a9a004a790e5b79b3bfcc93e143c12) | 清理测试副产物（历史备份/ 不该入库） |
| 96 | 2026-09-18 14:14 | [`670de21`](https://github.com/z91772524-ai/pojia-next/commit/670de21c2ddea089a37fadd80b203c1ae29b4494) | v7.4：修掉 19 项缺陷（4 类数据丢失 + 4 类假成功 + 字节保真与脱敏），新增 v74-fixes 回归套件 |
| 97 | 2026-09-18 13:30 | [`389914d`](https://github.com/z91772524-ai/pojia-next/commit/389914df4ddfd056a92489581ad946d23cc5e018) | v7.3 补丁：semgrep 门禁只排除 insecure-hash-sha1（本项目 SHA1 非密码学用途，已标注 usedforsecurity=False），排除理由写在 workflow 注释与 README 里；同时刷新 SHA256SUMS.txt |
| 98 | 2026-09-18 13:24 | [`0f3f26c`](https://github.com/z91772524-ai/pojia-next/commit/0f3f26c31cdf5e4665af41072da65f2a5b622d31) | v7.3：安全审查透明化 —— README 贴关键代码 + bandit/semgrep CI + SHA256 校验清单 |
| 99 | 2026-09-18 13:08 | [`34b5c84`](https://github.com/z91772524-ai/pojia-next/commit/34b5c841edd6beba4739190fad25438133187ddb) | 规范化：一键破甲.bat 按 .gitattributes 的 eol=crlf 落盘（线上已是 CRLF，本地工作区对齐；仍是纯 ASCII） |
| 100 | 2026-09-18 13:04 | [`a5470c1`](https://github.com/z91772524-ai/pojia-next/commit/a5470c15a5dfacdd97b9b34037465e187af96a39) | v7.2：把升级链从头查一遍（独立验证抓出 5 个缺陷） |
| 101 | 2026-09-18 12:45 | [`cadf505`](https://github.com/z91772524-ai/pojia-next/commit/cadf5052dcf8bdd55e44ded60b7dafef260732be) | v7.1：修掉「老版本升不上去」的死锁 + 新增 ZCode 目标 |
| 102 | 2026-09-18 12:14 | [`b10d541`](https://github.com/z91772524-ai/pojia-next/commit/b10d541ace492e51dd9d3ee9a5507504f55771f3) | 同步：界面预览图更新为 v7.0 + pick 提示加说明 [skip ci] |
| 103 | 2026-09-18 12:14 | [`057428a`](https://github.com/z91772524-ai/pojia-next/commit/057428ae7b17937e8748a20fc1f3d08665f254ac) | 更新界面预览图：v6.0 旧图（无 Codex）→ v7.0 三目标 + 体检 [skip ci] |
| 104 | 2026-09-18 12:08 | [`1247839`](https://github.com/z91772524-ai/pojia-next/commit/1247839c85f995e5b9e31affbc6620a50b0de223) | v7.0：WorkBuddy 云记忆通道 + 作业规范块（学同类项目的注入思路） |
| 105 | 2026-09-18 11:54 | [`c971e94`](https://github.com/z91772524-ai/pojia-next/commit/c971e94b540984be1d5475adaf9749cdbc27c2da) | v6.2：自证口令补齐到三个目标 + 修掉占位符字面量与 JSON 重复堆叠 |
| 106 | 2026-09-18 11:24 | [`7ab3d7d`](https://github.com/z91772524-ai/pojia-next/commit/7ab3d7dca189e973e1a8a8a1070f60d7df2d0b26) | v6.1：三目标 + 装完可自证 + 只读体检 + 专属管理目录（回填 Codex） |
| 107 | 2026-09-18 01:12 | [`55babf4`](https://github.com/z91772524-ai/pojia-next/commit/55babf46570143ed7d92e1097fab6c1d8ca19e1f) | 优化门面：README 首屏重写（5 枚徽章 + 界面预览图 + 6 条卖点）+ 仓库描述与 Topics 扩到 17 个 |
| 108 | 2026-09-18 00:59 | [`742c6a6`](https://github.com/z91772524-ai/pojia-next/commit/742c6a63b09290fdb2a102757cc38ef2dc63e9f1) | 加入免责声明：GitHub 界面醒目展示 + 每次启动打印 |
| 109 | 2026-09-18 00:52 | [`a9bf7b5`](https://github.com/z91772524-ai/pojia-next/commit/a9bf7b5701b0ec4b9414aa5188fd30c928345e31) | DSH/WorkBuddy 扫不到安装位置时改为 A/B 引导；主菜单去掉 [9] 指定安装目录 |
| 110 | 2026-09-18 00:11 | [`e5d15d7`](https://github.com/z91772524-ai/pojia-next/commit/e5d15d795535e66337ecc2db77678221c2327787) | 移除 Codex 目标：脚本、文档、仓库元数据全部只保留 dsh + WorkBuddy |
| 111 | 2026-09-17 20:52 | [`7318370`](https://github.com/z91772524-ai/pojia-next/commit/731837043f9626b02504deffb44dc1542ef9f262) | README 说明清楚：共同作者写在提交信息里（GitHub Contributors 列表只统计个人账号） |
| 112 | 2026-09-17 20:49 | [`ba67d68`](https://github.com/z91772524-ai/pojia-next/commit/ba67d682de538ea07773cd80fc807c7fe043d4df) | 破甲一键通 v6.0：把五套破甲工具合并成一个脚本 |

---

## 附：一句话的寿命

| 时间（北京时间） | 提交 | `更新日志.md` 第 201 行那句话的状态 |
|---|---|---|
| 2026-10-12 23:50 | `536ece2` | 写下：「核心源码依旧完全开源（就在本仓库），想审代码直接看」——此时源码在仓库里，**真** |
| 2026-10-13 01:02 | `d00b305` | 删掉源码。提交信息自己写着「源码不再随仓库分发」——这句话**变成假话**（距写下 72 分钟） |
| 2026-10-15 15:26 | `eb8b333` | README 口径改为「只发成品」。更新日志没动 |
| 2026-10-28 04:04 | `ab5a8a0` | 更新日志补 8.26 条目。这句话没动 |
| 2026-10-29 21:43 | `9df2c06` | 校验清单更新到 v8.26。没动 |
| 2026-10-29 21:45 | `31a6e31` | 「清理源码时代旧章节 —— 安全审查/防二改改为成品发行口径」：清了 README，没清这句 |
| 2026-10-29 23:17 | `b69da38` | 仍原样保留在第 201 行 |

**「想审代码直接看」指向的目录里，现在剩下什么：**

```
build_exe.py              打包脚本
release.py                发布脚本
fill_hashes.py            哈希填充
refresh_readme_hashes.py  README 哈希刷新
launcher.py               启动器
_回归测试/*.py             11 个测试脚本（cleanup_all / e2e_menu / regress_v76~v84 …）
```

没有 `破甲一键通.py`，没有 `破甲GUI.py`。

### 复核方法

```bash
# 源码最后存在的提交
git clone https://github.com/z91772524-ai/pojia-next && cd pojia-next
git ls-tree -l 536ece2 -- 破甲一键通.py 破甲GUI.py
git show 536ece2:破甲一键通.py | sha256sum

# 源码被删的提交
git show --stat d00b305

# README 口径改写
git show 7c603e1 -- README.md
```
