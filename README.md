# chasko-labs

> multi-platform ai agent framework + aws infrastructure + rust retrievers + gpu inference pipelines

![framework](https://img.shields.io/badge/framework-heraldstack-purple?style=flat-square)
![iac](https://img.shields.io/badge/iac-cloudformation-orange?style=flat-square)
![runtimes](https://img.shields.io/badge/agent_clis-5_runtimes-blue?style=flat-square)
![stack](https://img.shields.io/badge/stack-aws_%2B_rust_%2B_gpu-informational?style=flat-square)

## heraldstack — one framework, five cli runtimes

the same agent personas port across commercial agent clis so no single vendor owns the stack

| collective | cli runtime    | role                                                        |
| ---------- | -------------- | ----------------------------------------------------------- |
| shannon    | claude code    | primary — design, architecture, iac authoring              |
| haunting   | kiro cli       | custom agents — kb creation, video-to-document pipelines    |
| gander     | goose cli      | recipes — gpu inference jobs driven over ssh                |
| ibeji      | gemini cli     | reserved slot                                               |
| squad      | github copilot | reserved slot                                               |

core framework in [heraldstack-core](https://github.com/chasko-labs/heraldstack-core) — context-aware agent framework with memory, entity routing, narrative continuity

## public shipping

### agents + agentic workflows

- [heraldstack-core](https://github.com/chasko-labs/heraldstack-core) — the multi-platform agent framework
- [kiro-cli-custom-agent-kb-creator](https://github.com/chasko-labs/kiro-cli-custom-agent-kb-creator) — knowledge base creation with web crawling + semantic indexing
- [kiro-cli-custom-agent-screenpal-video-transcription](https://github.com/chasko-labs/kiro-cli-custom-agent-screenpal-video-transcription) — video-to-document via kiro custom agent, mcp + knowledge base, no fees outside aws kiro credits
- [goose-cli-video-transcription-recipe](https://github.com/chasko-labs/goose-cli-video-transcription-recipe) — whisper + moondream2 + ffmpeg containerized on amd gpu, triggered over ssh
- [kiro-cli-notes](https://github.com/chasko-labs/kiro-cli-notes) — kiro cli setup guide from 10 tutorial videos, full attribution to the aws kiro team

### aws infrastructure

- [aws-cloudformation-best-practices](https://github.com/chasko-labs/aws-cloudformation-best-practices) — authoring rules the cfn pre-deploy validators do not catch, distilled from the field (ec2 sg ascii, sso permission set region parameterization, ssm put-parameter tag-overwrite conflict)
- [jitsi-video-hosting](https://github.com/chasko-labs/jitsi-video-hosting) — on-demand jitsi meet on aws, scale-to-zero cost optimization
- [mac-developer-environment-setup](https://github.com/chasko-labs/mac-developer-environment-setup) — developer environment for building aws-powered solutions on macos 15
- [cognito-authentication](https://github.com/chasko-labs/cognito-authentication) — cognito + amplify auth patterns, following nader dabit's *full stack serverless*
- [rgc3-cloudscape-design-system-website](https://github.com/chasko-labs/rgc3-cloudscape-design-system-website) — [clouddelnorte.org](https://clouddelnorte.org) user group website, built on the aws cloudscape design system

### rust + embeddings

- [ultron-embeddings](https://github.com/chasko-labs/ultron-embeddings) — rust retriever ingesting marvel api data into jsonl embeddings stored as s3 vectors — inevitable, eternal, machine

### content + media pipelines

- [marvel-snap-bytedance](https://github.com/chasko-labs/marvel-snap-bytedance) — marvel snap screenshot pipeline, bytedance models via goose cli, local google photos ingestion, game reconstruction
- [bryan-chasko-com](https://github.com/chasko-labs/bryan-chasko-com) — personal site — hugo + s3 static hosting, custom theme forked from papermod (3d now)

### practice + learning

- [LeetCodeRandoms](https://github.com/chasko-labs/LeetCodeRandoms) — leetcode practice sessions with heraldstack expert coder personas driving the learn-from-mistakes loop
