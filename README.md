# 📡 TG Reader — خواندن کانال‌های تلگرام بدون فیلتر

> مشاهده پیام‌ها، عکس‌ها و ویدیوهای کانال‌های عمومی تلگرام از طریق GitHub Pages — بدون نیاز به VPN

[![GitHub Actions](https://img.shields.io/badge/Powered%20by-GitHub%20Actions-2088FF?logo=github-actions&logoColor=white)](https://github.com/features/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## ✨ قابلیت‌ها

- 📨 خواندن ۱۰۰ پیام آخر هر کانال عمومی تلگرام
- 🖼 نمایش عکس، ویدیو، فایل، استیکر، و پول
- ⬇ دانلود مستقیم عکس و ویدیو
- 🎨 طراحی شبیه تلگرام (دارک مود)
- 🔍 لایت‌باکس برای مشاهده بزرگ عکس‌ها
- ⚡ بدون نیاز به API Token یا ربات

---

## 🚀 راه‌اندازی

### ۱. Fork کردن این مخزن

روی دکمه **Fork** کلیک کنید.

### ۲. فعال کردن GitHub Pages

به `Settings → Pages` بروید و:
- **Source:** را روی `GitHub Actions` قرار دهید

### ۳. دادن مجوز به Actions

به `Settings → Actions → General` بروید:
- **Workflow permissions:** را روی **Read and write permissions** قرار دهید

### ۴. اجرا کردن

به تب **Actions** بروید:
1. روی **📡 Fetch Telegram Channel** کلیک کنید
2. روی **Run workflow** کلیک کنید
3. نام کانال را بدون `@` وارد کنید (مثال: `bbcpersian`)
4. تعداد پیام را انتخاب کنید (پیش‌فرض: ۱۰۰)
5. **Run workflow** را بزنید

### ۵. مشاهده نتیجه

پس از اجرا، به آدرس GitHub Pages خود بروید:
```
https://[username].github.io/[repo-name]
```

---

## 📋 کانال‌های پشتیبانی‌شده

فقط کانال‌های **عمومی** تلگرام پشتیبانی می‌شوند.

---

## ⚙️ تنظیمات

| پارامتر | پیش‌فرض | توضیح |
|---------|---------|-------|
| `channel` | الزامی | نام کانال بدون @ |
| `count` | 100 | تعداد پیام (۱۰ تا ۲۰۰) |

---

## 🛠 ساختار پروژه

```
├── .github/
│   └── workflows/
│       └── fetch.yml        # GitHub Actions workflow
├── scripts/
│   ├── fetch_channel.py     # اسکریپت دریافت پیام‌ها
│   └── template.html        # قالب HTML
└── README.md
```

---

## 📄 لایسنس

MIT License — آزاد برای استفاده شخصی و تجاری

---

> ساخته شده با ❤️ برای دسترسی آزاد به اطلاعات
