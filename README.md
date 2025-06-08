# n8n Web Automation Workflow

This repository contains an advanced web automation workflow built using [n8n](https://n8n.io), a powerful workflow automation tool for developers and data engineers.

## 🚀 What It Does
![WORKFLOW](https://github.com/user-attachments/assets/12bc0714-5032-4954-a953-a5d6fe867511)


This n8n workflow demonstrates how to automate:

- Web scraping using `HTTP Request` nodes
- Dynamic input processing with `Split Out`, `Loop Over Items`, and `Set`
- HTML parsing via custom JavaScript `Code` nodes
- Efficient batching and rate-limiting with `Wait` and chunk logic
- Final report generation in clean HTML format

It serves as a scalable blueprint for any repetitive data collection or transformation process.

## 📌 Features

- Headless scraping using `HTTP Request` (no browser needed)
- Resilient to pagination, chunked batching (~100–200 items per batch)
- Easily extendable: plug in new data sources or outputs (e.g., Google Sheets, Airtable, DB)
- Written fully in n8n’s visual interface — no external dependencies

## 🛠️ Tech Stack

- n8n (self-hosted)
- JavaScript (in-code nodes)
- HTML templating
- Optional: Google Sheets / File System / MongoDB (not included)

## 📂 Folder Structure

📁 n8n-workflow/
├── workflows/ # Exported workflow JSON
├── README.md # This file
└── LICENSE # MIT License

## 🧠 How To Use

1. Import the `.json` workflow into your n8n instance
2. Review and edit nodes: especially any `Set`, `HTTP Request`, and `Code` logic
3. Adjust the `Wait` delay or batch size if handling large-scale crawling
4. Trigger the workflow manually or schedule it

> ⚠️ Note: Ensure target URLs allow scraping and respect their rate limits.

## 💡 Use Cases 
![output](https://github.com/user-attachments/assets/687dace6-f9b7-454b-ae26-26955f83c74a)


- Automated report generation
- Data collection for research/internal use
- No-code/low-code backend processing

OUTPUT : 

## 🤝 Contributions

Pull requests are welcome if you improve efficiency, modularity, or add new export formats.

---
