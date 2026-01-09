
# Google Sheets – Order Data Schema

This Google Sheet is used to **store structured order information** automatically when an order is confirmed by the AI system.

---

## 📌 Purpose

- Maintain a centralized order database
- Enable order tracking and analytics
- Support future CRM or ERP integrations

---

## 📊 Sheet Name
````

Orders

```

---

## 🧾 Column Structure

| Column Name | Data Type | Description |
|------------|----------|-------------|
| Order ID | String | Unique identifier for each order |
| Customer Name | String | Full name of the customer |
| Telegram Username | String | Telegram handle (if available) |
| Telegram User ID | String | Unique Telegram user identifier |
| Product Name | String | Ordered product or service |
| Quantity | Number | Number of units ordered |
| Unit Price | Number | Price per unit |
| Total Price | Number | Calculated total amount |
| Order Status | String | Confirmed / Pending / Cancelled |
| Payment Method | String | Cash / Online / Other |
| Delivery Address | String | Customer delivery location |
| Order Timestamp | DateTime | Time of order confirmation |
| Notes | String | Optional remarks or AI-generated notes |

---

## 🧠 Data Population Logic

- Data is appended **only when order completion is detected**
- No manual data entry required
- Each row represents **one completed order**

---

## 🔐 Data Safety

- Sheet contains no API credentials
- Access controlled via Google Service Account
- Write-only access recommended for automation

---

## 🔄 Future Extensions

- Add delivery status tracking
- Integrate payment confirmation
- Connect to dashboards or BI tools

---

## 📌 Notes

- Do not manually modify column names after setup
- Schema changes should be reflected in the n8n workflow
```

---
