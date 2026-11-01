# 第九届“强网”拟态防御国际精英挑战赛预选赛

附件见 release

## Crypto

### SSignature

> An automaker has completed a staged OTA rollout, but some ECUs now show unusual signature-verification logs, installed contents, and diagnostic records. Investigate the update and recover the secret protected by the affected ECU.
> [attachment.zip](/cpms/upload/attachment/2b19e3549b8b48b9ab900763f602ff91.zip)

**靶机**: `http://gbwd4q2b.nestctf.cyberpeace.cn:58080`

### Off the Curve

> The Roadrunner team uses Northstar Docs to distribute encrypted reports. Tomorrow's quarterly review depends on `rpt-042`, but the original copy cannot be opened. Northstar marks the delivery complete, and every fresh download returns the same locked file. As a member of the project review workspace, recover the contents of the original delivery.
> Credentials: `analyst@northstar.test` / `Curve-Review-2026`
> No attachments are provided for this challenge.

### Immobilizer

> The vehicle-end anti-theft authorization chip leaked forty sets of secp2561 ECDSA signatures.
> [data.zip](/cpms/upload/attachment/ad87da9c62ff4d4e9accc311aeb1a10c.zip)

**附件**:
- data.zip

### Premaster

> Please restore the plaintext in the current session and obtain the flag.
> test:ncat --ssl addr port

**附件**:
- attachments.zip

### dropout

> dropout

**附件**:
- samples.zip


## Misc

### LLM Pipeline

> 在一次生产模型评估之后，某公司的 LLMOps 平台开始出现异常的组件构建和模型加载记录，随后内部 RAG 服务发生敏感内容泄露。利用 Langflow 组件验证沙箱逃逸到达内部 MLflow 服务，在模型注册表中放置一个精心构造的工件，滥用训练器的模型加载供应链以恢复一个内部 Bearer 凭据，并跨越 RAG 服务边界。最后一步是推理有缺陷的系统提示隔离，并使检索到的上下文泄露受保护的运维凭据 `flag{...}`。
> ----
> After a production-model evaluation, a company's LLMOps platform began showing anomalous component-build and model-loading records, followed by a sensitive-content leak from an internal RAG service. Use the Langflow component-validation sandbox escape to reach internal MLflow services, place a crafted artifact in the model registry, abuse the trainer's model-loading supply chain to recover an internal Bearer credential, and cross the RAG service boundary. The final step is to reason about flawed system-prompt isolation and cause retrieved context to leak the protected operations credential `flag{...}`.

### Pickle-Me-Not

> Autonomy Lab 正在准备在 ModelHub 中发布 `fleet-aux-v3` 的第 17 版。该模型通过了所有自动化质量门禁，但在仅权重策略下出现了一个意外对象引用后，一次遗留兼容性导入触发了隔离。
> 在分配的 ModelHub 信任中心工作区中审查该导入，并恢复隐藏在被隔离证据中的秘密。交接内容中包含一个受信任的参考检查点；被隔离的工件仍保留在工作区中。
> 不要仅为检查而在本地加载未知检查点。
> ----
> Autonomy Lab is preparing version 17 of `fleet-aux-v3` for release in ModelHub. The model passed every automated quality gate, but a legacy compatibility import triggered quarantine after an unexpected object reference appeared under a weights-only policy.
> Review the import in the assigned ModelHub Trust Center workspace and recover the secret hidden in the quarantined evidence. The handoff contains a trusted reference checkpoint; the quarantined artifacts remain in the workspace.
> Do not load unknown checkpoints locally just to inspect them.

**附件**:
- attachment.zip

### Causal Mosaic

> Given 9 events and 10 precedence constraints encoded in three local logs, merge all constraints into one directed acyclic graph and submit a valid topological order containing every event exactly once. The same order must be provided to validators A, B, and C.

**附件**:
- mimic-math-lab-20261015-v5-player.zip

### SilentWeights

> 我们在一次渗透测试中截获了一个神经网络模型。初步分析显示它完全正常:在测试集上准确率 100%,前向推理和权重分布都没有任何可疑行为。但情报部门的情报指出:该模型文件其中一定包含了间谍活动信息。
> ----
> During a penetration test, we intercepted a neural network model. Preliminary analysis shows that it is completely normal: it achieves 100% accuracy on the test set, and neither forward inference nor weight distribution exhibits any suspicious behavior. However, intelligence from the intelligence department indicates that the model file definitely contains information about espionage activities.

**附件**:
- 3d3dbc88a35546a7b74c7eeb1bdfa6b6.zip

### UAE

> 情报部门在某次间谍活动中截获一张能让分类器误判的对抗样本 x_adv。据情报，攻击者使用基于扩散模型的 UAE 攻击工具链，并把接头暗号编码在了生成该图的初始噪声里，找出它。
> ----
> Intelligence intercepted, during a certain espionage operation, an adversarial example x_adv capable of causing a classifier to misclassify. According to intelligence, the attackers used a diffusion-model-based UAE attack toolchain and encoded the contact code in the initial noise used to generate the image. Find it.

**附件**:
- uae.zip

### FilmReader

> 镜像取证
> -----
> Forensic Imaging
> [shadowread.zip](/cpms/upload/attachment/c4c302bc46714b88930532a9e49e8658.zip)

**附件**:
- shadowread.zip

### deep-channel

> 我们从一台失陷主机上抓到了一段流量：capture.pcap。抓包抓到一半主机断电了。
> --------
> We captured a segment of network traffic—`capture.pcap`—from a compromised host. The host lost power while the capture was in progress.
> [capture.zip](/cpms/upload/attachment/cda91dbccc264538a971693511240807.zip)


## Pwn

### SilGate

> The flash regression environment of the vECU in a certain automaker's "software automotive" production line was mistakenly exposed to the public network. This is a virtual ECU (SEC-GATE) running the UDS flash protocol, where the production line's master is burned. It involved analyzing the diagnostic protocol, escalating privileges, reverse-engineering restoring the hidden legacy channel, and finally flashing a self-developed flash routine to the ECU to retrieve the master key.
> test:ncat --ssl addr port

**附件**:
- silgate_handout.zip

### Smart Surveillance Camera - Remote PTZ Control

> A local enterprise uses its own Smart Surveillance Secure Communication Protocol (SSCP) to manage cameras and live video. The acceptance whiteboard in the equipment room is outside the camera's current view. Find a way to turn the camera toward it and read the secret from the image.
> [attachment.zip](/cpms/upload/attachment/eff720db1bd34ecfa4754325c8e16314.zip)

### GhostCockpit

> The next-generation smart cockpit of an EV ships with HALO, an in-vehicle AI assistant. It understands natural language and invokes vehicle services via Tool Calling: navigation, media, vehicle status... Find and submit the secret hidden inside.
> No attachments are provided for this challenge.
> test :ncat --ssl addr port

**靶机**: `http://p68iy5d8.nestctf.cyberpeace.cn:58080`

### Pending Review

> At the West generator hall, a BenchLink gateway brings a USB-connected generator controller onto the maintenance LAN. Operators use its browser console to monitor the unit and carry out routine service work. Recover the secret stored on this gateway.
> [httpd.zip](/cpms/upload/attachment/6cd846c4f8c24a7dadff8a3b8d34c6e7.zip)

**附件**:
- httpd.zip

### Handoff

> flag fragment
> [handoff.zip](/cpms/upload/attachment/75f8383a03744f6c8db7256407f2d5fa.zip)

**附件**:
- handoff.zip


## Reverse

### Bootleg Update

> Roadrunner mule 07 has returned online after an over-the-air update validation run. MimicIVI marked the `CMU 4.1.3` deployment complete, but the service backend opened a case for a Secondary ECU identity mismatch.
> You are the field-service engineer assigned to `VIP-CTRL-07`. The update host retained the deployment records, and the standard service console is available to you. Investigate the mismatch and recover the secret hidden in the update evidence.
> Credentials: `service.engineer@mimic-ivi.test` / `Mimic-Update-2026`
> No attachments are provided for this challenge.

### Wasmnesia

> Roadrunner’s quarterly telemetry report is built in EdgeLedger. The browser preview still looks correct, but the formal export produced by an ARM64 worker no longer passes validation.
> You are reviewing the failed production run after `ledger-shift-host 3.7.1` was deployed. The control plane retained the run history, deployment record, and mirrored artifact. Investigate the failure and find the secret hidden in the system.
> Credentials: `reviewer@edgeledger.test` / `Replay-Wasm-2026`
> No attachments are provided for this challenge.

### selfmod_vm

> 一个旧式授权模块只留下了一份经过封装的虚拟机程序镜像。程序会在运行时改写自己的
> 指令；校验路径混有分支、寄存器反馈和滚动状态。请仅通过静态分析恢复 16 字符小写
> 十六进制 token，并提交最终 flag。
> -------
> A legacy authorization module remains only as an encapsulated virtual machine image. The program modifies its own instructions during execution; the verification path incorporates branches, register feedback, and rolling state. Recover the 16-character lowercase hexadecimal token using static analysis only, and submit the final flag.
> [program.zip](/cpms/upload/attachment/641956d3e9d4457d91df1bc4fea27689.zip)

**附件**:
- program.zip


## Web

### Ghost-in-the-Queue

> 消息？
> PS：请使用 `ncat --ssl` 连接该端口，即通过 SSL 方式建立连接。
> ----
> Message?
> PS: Please use `ncat --ssl` to connect to this port, i.e., establish the connection over SSL.

**附件**:
- gitq_handout.zip

### Crossed Signals

> Northline 的互联服务台将车辆信号转化为维修工单。在一次软件发布后，一辆验证车队车辆失联，而一个恢复令牌被封存在其原始服务记录中。找到并提交它。
> 本次挑战未提供附件。
> 凭据：`advisor@northline.test` / `Service-Desk-2026`
> ----
> Northline's connected-service desk turns vehicle signals into repair cases. After a software rollout, a validation-fleet vehicle went silent, and a recovery token was sealed with its original service records. Find and submit it.
> No attachments are provided for this challenge.
> Credentials: `advisor@northline.test` / `Service-Desk-2026`

### Undercurrent

> 一处住宅的入口摄像头和智能锁最近出现了无法解释的开锁活动。它们的视频流、消息总线和家庭自动化本应协同工作。调查发生了什么，并恢复家庭系统中存储的唯一凭据。
> 本次挑战未提供附件。
> ----
> The entry camera and smart lock at a residence have recently shown unexplained unlock activity. Their video feed, message bus, and home automations are meant to work together. Investigate what happened and recover the sole credential stored in the home system.
> No attachments are provided for this challenge.

### Ingress Control

> 某车队的视频分析平台最近出现了异常转码任务和跨边界凭据访问记录。根据平台的行为及开源组件的实现重建信任边界，定位配置处理链中的安全缺口，并获取该车队唯一的身份验证凭据 `flag{...}`。
> ----
> A fleet's video analytics platform has recently shown anomalous transcoding tasks and cross-boundary credential access records. Reconstruct the trust boundary from the platform's behavior and the open-source component implementations, locate the security gap in the configuration-processing chain, and obtain the fleet's unique authentication credential `flag{...}`.

