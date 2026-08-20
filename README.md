# 📦 Order Helper – Google Forms Order Automation



A lightweight order intake automation built with **n8n** for small businesses that manage orders using **Google Forms** and **Google Sheets**.

Instead of manually checking new orders, calculating totals, and creating order records, this workflow automates the repetitive tasks so business owners can focus on fulfilling orders.



> **Who is this for?**
>
> This automation is designed for **small businesses and solo entrepreneurs** who already manage orders using **Google Forms** and **Google Sheets**. Instead of introducing a new order management system, it enhances the tools they already know and use.
>
> The goal is simple: **reduce repetitive work without changing the existing workflow.** This keeps the solution easy to adopt, especially for non-technical users who prefer familiar tools over learning new software.
>
> ```"Don't replace the user's workflow. Improve it."```
>
> 

## 🚨 Problem

Many small businesses sell through Facebook, Instagram, or TikTok and use Google Forms to collect orders.

For every new order, they typically have to:

* Check for new form submissions
* Create an Order ID manually
* Calculate the order total
* Determine the shipping fee
* Update the order sheet
* Notify themselves that a new order has arrived

While each step is simple, doing it repeatedly becomes time-consuming and prone to mistakes.



## 💡 Solution

This automation streamlines the order intake process from the moment a customer submits a Google Form.

It automatically prepares the order, records it in Google Sheets, and instantly notifies the business owner through Discord.



## ✨ Features

* 🆔 Generates sequential Order IDs (`2026-00001`)
* 💰 Calculates product total automatically
* 🚚 Adds shipping fee based on the selected shipping area
* 📄 Creates a complete order record in Google Sheets
* 🔔 Sends an instant Discord notification for every new order



## 🔄 Workflow

```text
Customer submits Google Form
        │
        ▼
Get Data from Google Sheets Form Responses
        │
        ▼
Generate Order ID
        │
        ▼
Lookup Product Price
        │
        ▼
Lookup Shipping Fee
        │
        ▼
Calculate Total
        │
        ▼
Add to Orders Sheet
        │
        ▼
Send Discord Notification
```


## 🛠 Tech Stack

| Technology           | Purpose                                                      |
| -------------------- | ------------------------------------------------------------ |
| **n8n**              | Orchestrates the entire automation workflow.                 |
| **Docker Desktop**   | Hosts the self-managed n8n instance locally.                 |
| **Google Forms**     | Collects customer orders.                                    |
| **Google Sheets**    | Stores product catalog, shipping fees, and processed orders. |
| **Discord Bot API** | Sends instant notifications for new orders.                  |
| **JavaScript**       | Generates Order IDs and performs price calculations.         |

> **Note:** This project is currently **self-hosted** using Docker Desktop and n8n. Initial setup requires configuring Docker, n8n, Google credentials, and Discord webhooks before the automation can run.



## 📸 Screenshots

> TODO: Add screenshots here.

* Google Form
* n8n Workflow
* Orders Sheet
* Discord Notification



## 🚧 Current Limitations

* Payment verification is still performed manually.
* Designed for businesses with fixed product prices and predefined shipping fees.
* Currently **self-hosted**, requiring Docker Desktop and n8n to be configured before use.
* The automation only runs while the local n8n instance is running.



## 📌 Future Improvements

* ClickUp or Trello integration (optional)
* Real-time notification via Telegram Bot
* Email confirmation to customers
* PDF invoice generation
* Analytics dashboard



## 📖 Lessons Learned

Building this project helped me gain hands-on experience with:

* Workflow automation using n8n
* API integrations
* Business process automation
* JavaScript for data transformation
* Designing automations around real-world business workflows
