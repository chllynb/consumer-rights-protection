# Consumer Rights Protection Skill

一个面向中国消费纠纷场景的通用维权技能包，适用于把真实消费经历沉淀成可复用的 AI Skill，让其他用户在遇到类似问题时，快速获得取证建议、投诉路径和可直接粘贴的投诉文案。

## 适用场景

- 酒店、民宿、OTA 预订纠纷
- 网购商品质量、货不对板、售后拒绝
- 餐饮食品安全、异物、变质、食后不适
- 预付卡、会员卡、培训课、健身美容闭店跑路
- 虚假宣传、霸王条款、拒绝退款、价格争议

## 核心能力

- 帮用户判断纠纷类型与优先维权路线
- 提供证据收集清单与取证重点
- 生成商家/平台协商话术
- 生成适合 12315 / 12345 的投诉草稿
- 提供简明法律依据与风险提醒
- 按场景拆分专项模块，避免主技能过长

## 仓库结构

```text
consumer-rights-protection/
├── SKILL.md
├── README.md
├── VERSION
├── LICENSE
├── agents/
│   └── openai.yaml
├── assets/
│   └── evidence-checklist.svg
├── references/
│   ├── complaint-channels.md
│   └── legal-basis.md
├── scenarios/
│   ├── food-safety.md
│   ├── hotel-booking.md
│   ├── online-shopping.md
│   └── prepaid-card.md
└── dist/
    └── consumer-rights-protection-v1.0.0.zip
```

## 文件说明

- `SKILL.md`
  技能入口文件，定义触发条件、工作流、输出格式和资源导航。
- `references/legal-basis.md`
  常用维权法律依据与表述模板。
- `references/complaint-channels.md`
  维权投诉渠道选择建议。
- `scenarios/*.md`
  高频消费纠纷场景模板。
- `agents/openai.yaml`
  面向支持技能 UI 的元数据。
- `assets/evidence-checklist.svg`
  可视化证据清单素材。

## 安装与分发

### 方式 1：直接分发压缩包

将 `dist/consumer-rights-protection-v1.0.0.zip` 直接发给其他人即可。对方解压后，保持目录结构不变即可使用或导入到支持 Skill 的工具中。

### 方式 2：作为 GitHub 仓库发布

1. 将整个目录上传到 GitHub 新仓库。
2. 在 Releases 中上传 `dist/consumer-rights-protection-v1.0.0.zip` 作为发布附件。
3. 在仓库首页保留本 `README.md`，方便其他人查看说明与安装方式。

### 方式 3：本地作为技能目录使用

如果你的 AI 工具支持本地技能目录，可直接把整个 `consumer-rights-protection` 文件夹加入其技能路径，保持 `SKILL.md` 位于技能根目录即可。

## 使用示例

### 示例 1：酒店订房纠纷

```text
请用 $consumer-rights-protection 帮我整理一个酒店维权投诉。
我在平台上订了双人间，到店后酒店说只能住 1 人，平台还拒绝退款。
```

### 示例 2：网购商品问题

```text
用 $consumer-rights-protection 帮我生成 12315 投诉文案。
我买到的商品和宣传图严重不符，商家说特价商品不退不换。
```

### 示例 3：预付卡跑路

```text
请用 $consumer-rights-protection 帮我列维权步骤和投诉文本。
我充值的健身房突然闭店，老板失联，还有不少会员也受影响。
```

## 发布建议

- 对外发布前，建议把你自己的典型案例继续补充到 `scenarios/` 中。
- 若需要更强的地域适配，可增加 `references/local-channels.md` 存放各地市场监管局、12345 小程序入口等信息。
- 若后续经常迭代，可按版本号更新 `VERSION` 并重新生成 `dist/` 压缩包。

## 风险提示

- 本技能提供的是维权辅助和文案支持，不构成律师法律意见。
- 具体法律适用、赔偿标准、投诉入口和办理规则，最终以最新官方渠道和当地监管要求为准。
- 涉及人身伤害、大额损失、疑似刑事诈骗时，应尽快同步咨询律师或报警。

## 版本

当前版本见 `VERSION` 文件。
