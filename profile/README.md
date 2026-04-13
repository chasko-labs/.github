# chasko-labs

> multi-platform ai agent infrastructure for one operator's workshop — aws at the foundation, rocm + mac mini on the desk, heraldstack as the brain

![focus](https://img.shields.io/badge/focus-ai_agents_%2B_aws-orange?style=flat-square)
![bench](https://img.shields.io/badge/bench-rocm_aibox_%2B_mac_mini-informational?style=flat-square)
![clis](https://img.shields.io/badge/agent_clis-claude_%7C_kiro_%7C_goose_%7C_gemini_%7C_copilot-purple?style=flat-square)
![iac](https://img.shields.io/badge/iac-cloudformation-blue?style=flat-square)

## what this place is

aws content builder. ai/ml infra hobbyist. the workshop answering one question: how do you run a multi-agent ai bench on one operator's hardware without the cloud bill eating you alive?

the bet — aws for the durable parts, rocm for the gpu parts, heraldstack as the meta-framework that routes agent personas across whichever commercial cli is best for the job

## heraldstack — five cli runtimes, one brain

the same agent personas port across commercial agent clis so no single vendor owns the bench

| collective | cli runtime      | what it runs                                                     |
| ---------- | ---------------- | ---------------------------------------------------------------- |
| shannon    | claude code      | primary runtime — design, architecture, iac authoring           |
| haunting   | kiro cli         | custom agents — kb creation, video-to-document pipelines         |
| gander     | goose cli        | recipes — rocm-gpu inference jobs driven from mac mini over ssh  |
| ibeji      | gemini cli       | reserved slot                                                    |
| squad      | github copilot   | reserved slot                                                    |

core framework in [heraldstack-core](https://github.com/chasko-labs/heraldstack-core) — context-aware agent framework with memory, entity routing, narrative continuity

## public shipping

### agents + agentic workflows

- [heraldstack-core](https://github.com/chasko-labs/heraldstack-core) — the multi-platform agent framework
- [heraldstack](https://github.com/chasko-labs/heraldstack) — placeholder repo carrying harald's catchphrase *"science bless us everyone"* — the real framework lives in [heraldstack-core](https://github.com/chasko-labs/heraldstack-core)
- [kiro-cli-custom-agent-kb-creator](https://github.com/chasko-labs/kiro-cli-custom-agent-kb-creator) — knowledge base creation with web crawling + semantic indexing
- [kiro-cli-custom-agent-screenpal-video-transcription](https://github.com/chasko-labs/kiro-cli-custom-agent-screenpal-video-transcription) — video-to-document via kiro custom agent, mcp + knowledge base, no fees outside aws kiro credits
- [goose-cli-video-transcription-recipe](https://github.com/chasko-labs/goose-cli-video-transcription-recipe) — whisper + moondream2 + ffmpeg containerized on amd gpu, triggered from mac mini over ssh
- [kiro-cli-notes](https://github.com/chasko-labs/kiro-cli-notes) — kiro cli setup guide from 10 tutorial videos, full attribution to the aws kiro team

### aws infrastructure

- [jitsi-video-hosting](https://github.com/chasko-labs/jitsi-video-hosting) — on-demand jitsi meet on aws, scale-to-zero cost optimization
- [mac-developer-environment-setup](https://github.com/chasko-labs/mac-developer-environment-setup) — developer environment for building aws-powered solutions on macos 15
- [cognito-authentication](https://github.com/chasko-labs/cognito-authentication) — cognito + amplify auth patterns, following nader dabit's *full stack serverless*
- [rgc3-cloudscape-design-system-website](https://github.com/chasko-labs/rgc3-cloudscape-design-system-website) — [clouddelnorte.org](https://clouddelnorte.org) user group website, built on the aws cloudscape design system

### rust + embeddings

- [ultron-embeddings](https://github.com/chasko-labs/ultron-embeddings) — rust retriever ingesting marvel api data into jsonl embeddings stored as s3 vectors — inevitable, eternal, machine

### content + media pipelines

- [marvel-snap-bytedance](https://github.com/chasko-labs/marvel-snap-bytedance) — marvel snap screenshot pipeline, bytedance models via goose cli, local google photos ingestion, game reconstruction
- [bryan-chasko-com](https://github.com/chasko-labs/bryan-chasko-com) — personal site, hugo + s3 static hosting, custom theme hacked from papermod (3d now)

### practice + learning

- [LeetCodeRandoms](https://github.com/chasko-labs/LeetCodeRandoms) — leetcode practice sessions with heraldstack expert coder personas driving the learn-from-mistakes loop

## the bench

- **rocm aibox** — linux workstation, amd gpu, primary dev machine. agents run here, models fine-tune here, docker jobs execute here
- **mac mini** — secondary. drives remote jobs over ssh, handles macos-only workflows, agent-forwards git identity
- **five agent clis in rotation** — routed by task fit, not vendor loyalty. whichever cli does the job best that week wins

## the operator

bryan chasko — aws content builder, ai/ml infrastructure hobbyist. personal site code in [bryan-chasko-com](https://github.com/chasko-labs/bryan-chasko-com)
