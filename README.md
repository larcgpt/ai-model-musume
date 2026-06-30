# AI Model Musume

AI 模型娘化角色圖像資料集。收錄 22 個主流 AI 模型（LLM / 圖像生成）的角色設定卡片、編號卡與桌布圖像，按模型分類整理。

![代表圖](Unknown/Unknown_Wallpaper_6.png)

## 概述

每個模型的角色圖像由 ChatGPT 生成，以動漫角色娘化的形式呈現各 AI 模型的特色。資料集包含三種檔案類型：

- **角色設定卡** — 以角色設定表格呈現，包含角色名稱、代號、陣營、核心能力、性格等詳細資料，並提供三種語言版本
- **Main 卡** — 僅含編號與模型名稱的簡單角色展示卡片
- **桌布** — 橫向與直向的高品質角色桌布

## 收錄模型一覽

| 資料夾 | 模型 | 預覽 |
|--------|------|------|
| ChatGPT | OpenAI ChatGPT (GPT) | ![ChatGPT](ChatGPT/ChatGPT_Main_1.png) |
| ChatGPT_GPT-OSS | OpenAI ChatGPT GPT-OSS | ![GPT-OSS](ChatGPT_GPT-OSS/ChatGPT_GPT-OSS_Main_1.png) |
| Claude_Fable | Anthropic Claude (Fable) | ![Claude Fable](Claude_Fable/Claude_Main_1.png) |
| Claude_Opus | Anthropic Claude Opus | ![Claude Opus](Claude_Opus/Claude_Opus_Main_1.png) |
| Claude_Sonnet | Anthropic Claude Sonnet | ![Claude Sonnet](Claude_Sonnet/Claude_Sonnet_Main_1.png) |
| DeepSeek | DeepSeek | ![DeepSeek](DeepSeek/DeepSeek_Main_1.png) |
| Doubao | 豆包 | ![Doubao](Doubao/Doubao_Main_1.png) |
| Gemini | Google Gemini | ![Gemini](Gemini/Gemini_Main_1.png) |
| Gemma | Google Gemma | ![Gemma](Gemma/Gemma_Main_1.png) |
| GLM | 智譜 GLM | ![GLM](GLM/GLM_Main_1.png) |
| Grok | xAI Grok | ![Grok](Grok/Grok_Main_1.png) |
| Kimi | Moonshot Kimi | ![Kimi](Kimi/Kimi_Main_1.png) |
| Llama | Meta Llama | ![Llama](Llama/Llama_Main_1.png) |
| Mai | Microsoft Copilot Mai | ![Mai](Mai/Mai_Main_1.png) |
| Mimo | Mimo | ![Mimo](Mimo/Mimo_Main_1.png) |
| Minimax | MiniMax | ![Minimax](Minimax/Minimax_Main_1.png) |
| Mistral | Mistral AI | ![Mistral](Mistral/Mistral_Main_1.png) |
| Nemotron | NVIDIA Nemotron | ![Nemotron](Nemotron/Nemotron_Main_1.png) |
| Phi | Microsoft Phi | ![Phi](Phi/Phi_Main_1.png) |
| Qwen | 阿里通義千問 | ![Qwen](Qwen/Qwen_Main_1.png) |
| Seedance | Seedance | ![Seedance](Seedance/Seedance_Main_1.png) |
| Stable Diffusion | Stable Diffusion | ![Stable Diffusion](Stable%20Diffusion/Stable%20Diffusion_Main_1.png) |

## 命名規則

每個模型資料夾的圖像依用途統一命名：

### 角色設定卡（每模型 3 張）
- `{Model}_繁體中文_角色設定.png` — 繁體中文版。內容以繁體中文書寫角色設定（角色名稱、代號、陣營、核心能力、數據分析等）
- `{Model}_日文_角色設定.png` — 日文版。包含日文字元（性格、ロール、 Creed、Faction 等）
- `{Model}_English_角色設定.png` — 英文版。內容全英文（Role、Codename、Creed、Faction、Data、Core、System 等）

### 一般編號卡
- `{Model}_Main_1.png`、`{Model}_Main_2.png` ... — 僅顯示編號與模型名稱的簡單角色卡片，無詳細設定表格

### 桌布
- `{Model}_Wallpaper_1.png` — 橫向桌布（寬 > 高），以模型資料夾名稱為前綴
- `Mobile_Wallpaper_1.png` — 直向桌布（高 > 寬），跨資料夾共用統一流水號

### 未分類
- `Unknown/` — 尚未識別來源或等待分類的圖像

## 語言識別方式

角色設定卡的三種語言版本透過 EasyOCR（`ch_tra` + `en` 模型）自動識別分類：
- **繁體中文**：OCR 內容以繁體中文為主，含核心能力、數據分析、雲端、企業運算等詞彙
- **日文**：OCR 結果含日文字元，如性格、ロール、ネメシス、データ等，以及 NVIDIA、GPU 加速等混合內容
- **English**：OCR 結果全為英文，含 Role、Codename、Creed、Faction、Data、Core、System、Inference Engine 等詞彙

## 專案結構

```
AI_MUMUSE/
├── ChatGPT/                # OpenAI ChatGPT
│   ├── ChatGPT_Main_1.png
│   ├── ChatGPT_繁體中文_角色設定.png
│   ├── ChatGPT_日文_角色設定.png
│   ├── ChatGPT_English_角色設定.png
│   ├── ChatGPT_Wallpaper_1.png
│   └── Mobile_Wallpaper_1.png
├── ChatGPT_GPT-OSS/        # ChatGPT GPT-OSS
├── Claude_Fable/           # Claude Fable
├── Claude_Opus/            # Claude Opus
├── Claude_Sonnet/          # Claude Sonnet
├── DeepSeek/               # DeepSeek
├── Doubao/                 # 豆包
├── Gemini/                 # Google Gemini
├── Gemma/                  # Google Gemma
├── GLM/                    # 智譜 GLM
├── Grok/                   # xAI Grok
├── Kimi/                   # Moonshot Kimi
├── Llama/                  # Meta Llama
├── Mai/                    # Microsoft Copilot Mai
├── Mimo/                   # Mimo
├── Minimax/                # MiniMax
├── Mistral/                # Mistral AI
├── Nemotron/               # NVIDIA Nemotron
├── Phi/                    # Microsoft Phi
├── Qwen/                   # 阿里通義千問
├── Seedance/               # Seedance
├── Stable Diffusion/       # Stable Diffusion
├── Unknown/                # 未分類圖像
├── README.md
└── .gitignore
```

## 如何使用

直接瀏覽各模型資料夾即可查看對應的角色圖像。所有檔案均為 PNG 格式，可直接下載使用。

## 附註

- 本專案的 `.py` 腳本僅用於初始自動化分類與重新命名，未納入版本控制
- 角色設定卡由 ChatGPT 生成，每張都包含角色名稱、代號、陣營、核心能力等詳細資訊
- 資料夾名稱與檔案名稱均使用 UTF-8 編碼，支援多語言字元
