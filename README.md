# Lead-Scraper-n8n
An n8n workflow for scraping leads automatically
# 🚀 Lead Scraper – n8n Workflow  

An **n8n automation workflow** that scrapes leads from online sources, verifies their email addresses, and prepares clean, ready-to-use contact data for marketing or business development.  

This project demonstrates how **low-code automation with n8n** can replace manual lead collection, reduce bounce rates from invalid emails, and speed up outreach campaigns.

---

## 📌 Use Case  

Lead generation is one of the most time-consuming tasks for businesses. This workflow automates the process:  

1. **Scrape Leads** – Collects raw lead data from sources (websites, APIs, or uploaded lists).  
2. **Email Verification** – Validates emails using APIs (e.g., ZeroBounce, Hunter, NeverBounce, or any email verification service connected in n8n).  
3. **Data Cleaning & Export** – Saves only valid leads in a clean list (CSV, Google Sheets, or Database).  

💡 **Practical Scenarios**  
- Sales teams verifying cold email lists before outreach  
- Marketing teams cleaning scraped leads from LinkedIn, web forms, or CRMs  
- Startups automating lead intake pipelines  
- Agencies reducing bounce rates and spam complaints in campaigns  

---

## ⚙️ Workflow Overview  

- **Input Node**: Accepts a list of leads (CSV, API, or manual entry).  
- **Scraping Node(s)**: Gathers company or contact details (depending on setup).  
- **Email Verification Node**: Calls an email verification API to check:  
  - Valid / Invalid  
  - Disposable / Catch-All  
  - Deliverable / Risky  
- **Filtering Node**: Keeps only verified emails.  
- **Output Node**: Saves results (CSV, Google Sheets, Database, or another API).  

---

## 📂 Project Structure  

Lead-Scraper-n8n/
│── workflows/
│ └── email_verifier.json # Main n8n workflow
│── README.md # Documentation


---

## 🚀 How to Use  

1. Install [n8n](https://n8n.io) locally or on a server.  
2. Open the n8n editor UI.  
3. Import the workflow from `workflows/email_verifier.json`.  
4. Add your **API credentials** (email verification service, Google Sheets, database, etc.).  
5. Run the workflow and watch leads get cleaned automatically.  

---

## 🛠️ Requirements  

- [n8n](https://n8n.io) (v1.0+ recommended)  
- Email Verification API key (e.g., Hunter, ZeroBounce, NeverBounce, or your preferred provider)  
- (Optional) Database or Google Sheets integration for storing results  

---

## 📊 Example Output  

| Name       | Email               | Status     | Source      |
|------------|---------------------|------------|-------------|
| John Doe   | john@company.com    | ✅ Valid   | Web Form    |
| Jane Smith | jane@fakeemail.com  | ❌ Invalid | LinkedIn    |
| Sam Lee    | sam@catchall.com    | ⚠️ Risky   | Scraper Bot |

---

## 🌟 Benefits  

✔️ Saves hours of manual lead verification  
✔️ Increases deliverability & reduces bounce rate  
✔️ Easy to customize & extend with other n8n nodes  
✔️ Scales with your business needs  

---

## 🤝 Contribution  

Feel free to fork this repo, suggest improvements, or adapt the workflow for your specific use case.  

---

## 📜 License  

This project is licensed under the MIT License – you’re free to use, modify, and distribute it.  
