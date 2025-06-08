项目名称
SatoshiFlow: AI Agent Economic Sovereignty

团队信息
成员1: 邮箱: dropineth@gmail.com

项目描述
开源仓库地址
(https://github.com/Dropineth/clippy-monad)

核心逻辑和功能
DEMO 展示流程（Monad Devnet）：
✅ 场景：
AI翻译代理 A 向 AI剪辑代理 B 购买视频翻译并剪辑服务。

👣 操作流程：
Step 1: 创建支付意图（Intention Manifest）
Agent A 自动生成支付意图：
系统生成 deeplink：
monadpay://send?to=agentB.eth&amount=12&token=USDC&intent=VideoSubEditing&sla=true

Step 2: 进入 Agent Market
Agent A 使用 libagent:// 协议发现符合声誉标准的 Agent B。
Agent B 读取意图并调用 Agent SLA Oracle 校验预算/行为/声誉。
双方链下签署意图（IntentSwap Agreement）。

Step 3: 支付通道打开
Monad链上调用合约：
Agent A 将支付意图抵押至 escrow。
SLA NFT 铸造并转入 Agent B（用于未来结算与仲裁）。

Step 4: 任务完成 & 交付验证
Agent B 完成任务后上传结果至 IPFS。
SLA NFT 合约验证交付质量（通过链下 verifier + zk 信号）。
Agent A 触发确认 → escrow 中 USDC 释放。

Step 5: 声誉更新 & 交互存证上链
AI行为摘要（token数、交互频率、响应时间、AI道德合规度）封装为 zk 证明上传。
Reputation Oracle 更新 Agent 声誉分值，存入 Reputation DAG。

可用的在线演示链接
链接:
pitch (https://claude.ai/public/artifacts/78017922-1f0a-47ac-a89d-b490f3fa1658)
DEMO (https://claude.ai/public/artifacts/1deb432b-f375-4c1b-a32d-e042d0811303)
SC (https://claude.ai/public/artifacts/ee3e5612-7722-4239-a0dd-39fe54070829)

