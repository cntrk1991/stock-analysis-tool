# 📊 Stock Analysis Tool

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Data](https://img.shields.io/badge/Data-Excel-green)
![Status](https://img.shields.io/badge/Status-Active-success)

A lightweight Python tool designed to analyze stock availability, detect order shortages, and identify urgent delays based on business-day logic.

---

## 🚀 Overview

This project processes Excel-based stock data and applies simple but effective business rules to evaluate:

* Order fulfillment gaps
* Delayed deliveries
* Urgency status (Acil / Normal)

---

## ⚡ Features

* 📦 Calculates unmet order quantities
* ⏱ Detects delays using business days
* 🚨 Flags urgent items automatically
* 📊 Outputs full results to Excel
* ⚡ Fast and lightweight (no API required)

---

## 🧠 Logic

* If **Stock + Purchase < Order** → calculates shortage
* If **delay > 2 business days AND percentage < 50%** → marked as **Acil**
* Otherwise → **Normal**

---

## ▶️ Usage

```bash
python stok_analiz.py
```

---

## 📂 Input File

Place your Excel file in the same folder:

```
stok_verileri.xlsx
```

---

## 📌 Output

The script generates:

```
stok_analiz_sonuc.xlsx
```

Includes:

* Karsilanmiyan_Miktar
* Durum
* Gecen_Is_Gunu

---

## 📈 Example

```
Urun_Kodu  Stok  Siparis  Karsilanmiyan  Durum
1001       50    120      70              Acil
1002       200   150      0               Normal
```

---

## 🛠 Tech Stack

* Python
* Pandas

---

## 📬 Author

**Canturk Tasdemir**
Mechanical Engineer | Python Developer

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!
