# 🧾 Receipt OCR & Order Lookup

A sleek Python project harnessing **AI-powered OCR** to extract order numbers from receipt images and fetch order details from a database. Perfect for automating e-commerce workflows with precision! 🚀

---

## 📋 Contents
- [Overview](#-overview)
- [Features](#-features)
- [How It Works](#-how-it-works)
- [Setup](#-setup)
- [Usage](#-usage)
- [Dependencies](#-dependencies)
- [Output](#-output)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview
This project uses **DocTR** for OCR to scan receipt images, extract order numbers, and query a database for order status. Built for scalability, it’s ideal for e-commerce and customer service applications. 🛍️

---

## 🔥 Features
- 🖼️ Extract text from receipt images with DocTR.
- 🔍 Detect order numbers using regex.
- 🗄️ Query order details from a database.
- 📤 Return results in JSON format.
- 📊 Visualize OCR output with annotations.

---

## 🛠️ How It Works
1. **Load Image**: Import receipt image (e.g., `reciept.jpg`).
2. **OCR**: DocTR extracts text with high accuracy.
3. **Extract Order Number**: Regex finds patterns like `Order #123`.
4. **Database Check**: Match order number in a dummy database.
5. **Output**: Return JSON with order status or error.

---

## ⚙️ Setup
1. **Clone Repo**:
   ```bash
   git clone https://github.com/your-username/receipt-ocr-order-lookup.git
   cd receipt-ocr-order-lookup
   ```
2. **Install Dependencies**:
   ```bash
   pip install python-doctr pymongo matplotlib
   ```
3. **Run Jupyter**:
   ```bash
   jupyter notebook
   ```

---

## 🚀 Usage
1. Place a receipt image in the project folder.
2. Open `ocr_order_Shopilam_whatsopify.ipynb` in Jupyter.
3. Run cells to process the image and view results.
4. Customize the `dummy_orders` dictionary or connect to a real database (e.g., MongoDB).

---

## 📦 Dependencies
- `python-doctr`: OCR text extraction.
- `pymongo`: Database integration.
- `matplotlib`: Image visualization.
- `re`: Regex for order number extraction.

Install with:
```bash
pip install python-doctr pymongo matplotlib
```

---

## 📈 Output
**Extracted Text Example**:
```
RECEIPT OF SALE
SHOP'S NAME
Order #ORD123
...
Total: 32.1
```

**JSON Response**:
```json
{
    "status": "success",
    "message": "Order ORD123 found.",
    "order_details": {
        "status": "Delivered",
        "details": {"product": "Mouse", "qty": 1}
    }
}
```

---

## 🤝 Contributing
1. Fork the repo.
2. Create a branch: `git checkout -b feature/your-feature`.
3. Commit changes: `git commit -m "Add feature"`.
4. Push: `git push origin feature/your-feature`.
5. Open a Pull Request.

---

## 📜 License
MIT License. See [LICENSE](LICENSE).

---

🌟 **Star this repo** to support AI-driven automation! Let’s make receipt processing smarter! 💡
