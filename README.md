# 🧠 Multimodal Prompt Engineering with Gemini & GPT-4o
*A comparative study of how multimodal LLMs interpret and reason across text, images, and charts.*

---

## 🧭 Overview
This project compares **Google Gemini** and **OpenAI GPT-4o** on multimodal reasoning tasks that combine **text and visual data**.  
It evaluates both models on chart analysis, image understanding, and text-image reasoning — exploring how prompt structure and context affect their responses.

---

## 📂 Repository Structure
```
multimodal-prompt-engineering/
│
├── notebooks/
|   ├── Multimodal_Prompt_Engineering_light.ipynb # Reduced sized version of the file right below for viewing
│   ├── Multimodal_Prompt_Engineering_with_Google_Gemini.ipynb
│   └── Multimodal_Prompt_Engineering_with_OpenAI_GPT_4o.ipynb
│
```
---

## 🧪 Core Experiments
The project compares how Gemini and GPT-4o handle different multimodal reasoning tasks.  
Each task uses identical inputs (images, charts, or tables) and standardized prompts to ensure fair comparison.

| Task | Input | Gemini | GPT-4o |
|------|--------|---------|--------|
| Chart interpretation | Bar chart | Narrative trend summary | Precise numeric analysis |
| Scene reasoning | Photo | Rich contextual detail | Structured factual output |
| Table extraction | Image of table | Missed totals | Accurate calculations |
| Text+image | Mixed prompt | Story-like response | Analytical summary |

---

## ⚙️ Implementation
- Both models are accessed via official APIs (`google-generativeai` and `openai`).
- Each experiment prompt and image is stored in `/data/`.
- Outputs and comparisons are automatically logged in `/results/`.
- Evaluation metrics include response time, numeric accuracy, and factual consistency.

---

## 📊 Example Output
**Prompt:** “Analyze this chart and describe the quarterly revenue trend.”

**Gemini:**  
> “Revenue rose in Q1–Q2, dipped slightly in Q3, and stabilized in Q4.”

**GPT-4o:**  
> “Revenue increased 11% in Q2 and remained stable through Q4, indicating a seasonal plateau.”

*(See `/results/output_examples/` for screenshots.)*

---

## 💡 Key Findings
- **GPT-4o** produced more structured, concise numeric summaries.  
- **Gemini** provided richer descriptive narratives.  
- GPT-4o excelled in **data-driven reasoning**, while Gemini was stronger in **scene interpretation**.  

---
