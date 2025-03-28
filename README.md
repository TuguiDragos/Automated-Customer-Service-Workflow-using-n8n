# 🤖 Automated Customer Service Workflow using n8n

This project is a real-time, automated customer support system built with **n8n**, **OpenAI**, **Gmail**, and **Google Sheets**.  
It reads incoming customer emails, understands them using AI, categorizes and logs the messages, and sends back personalized responses — all without human input.

---

## 🧠 How It Works

1. **Incoming Emails**  
   Customers send support inquiries (e.g., “My hoodie hasn’t arrived”, “Item arrived damaged”) to the business email address.

2. **Email Filtering**  
   All new emails with the label `N8N-Test` are automatically picked up by the system for processing.

3. **AI-Powered Understanding**  
   Each email is sent to **OpenAI** (GPT) which does three things:
   - Generates a relevant and human-like reply
   - Determines the **category** of the inquiry (e.g., Refund, Exchange, General)
   - Analyzes the **emotional tone** (e.g., calm, happy)

4. **Logging**  
   The system logs every email into a structured **Google Sheet**, including:
   - Timestamp
   - Customer email
   - Original message subject
   - AI-generated reply
   - Detected category
   - Detected tone

5. **Reply Sent Automatically**  
   The reply generated by the AI is sent back to the customer using **Gmail**, closing the loop in a matter of seconds.

---

## 🔍 What It Looks Like

### 📨 Customer Emails
All incoming messages labeled `N8N-Test` are captured for analysis.

![Customer Inquiry - Emails Received](https://github.com/user-attachments/assets/03ea667a-9fea-493d-9fb1-858b3664862a)


---

### ✉️ Smart AI Replies
Each customer receives a personalized response, written by OpenAI and sent through Gmail.

![Email Sent - Customer Response](https://github.com/user-attachments/assets/539dd30c-60d1-4523-a6e3-c4401c5b40b0)
![Automated Response - Customer Service Reply](https://github.com/user-attachments/assets/170752c8-77a5-477e-a1e2-9dfe5017f294)


---

### 📊 Logged in Google Sheets
A full history of conversations is stored with category and tone — ideal for analytics or reporting.


<img width="1107" alt="Customer Interaction Log - Google Sheets" src="https://github.com/user-attachments/assets/8b3a17dc-f539-4646-9412-724e24b0cf73" />


---

### 🧩 Visual Automation Flow (n8n)
Here's the full automation behind the scenes — all built visually in n8n.

![n8n Workflow - Automated Customer Service](https://github.com/user-attachments/assets/2e442274-fc57-4a03-9f78-96efe1ccff3e)


---

## 💡 Use Case

This system is perfect for:
- E-commerce brands handling repetitive support requests
- Small teams who want to reduce support response time
- Any business looking to automate customer service without losing personalization

---

## 👨‍💻 Author

Built with love, logic, and a bit of AI  
by [Tugui Dragoș](https://tuguidragos.com) 💼
