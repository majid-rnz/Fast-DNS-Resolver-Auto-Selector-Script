# 🌐 Fast DNS Resolver Auto-Selector Script

A lightweight Bash script that checks a list of DNS servers and picks the first 5 responsive ones. It then updates your `/etc/resolv.conf` with those working nameservers. Useful in restricted or censored networks.

---

## 🛠️ Features

- Automatically tests over 100 global and regional DNS resolvers
- Selects the first 5 working servers
- Uses `dig` with timeout for fast detection
- Outputs color-coded success/failure messages
- Automatically updates `/etc/resolv.conf`
- Includes well-known public DNS (Cloudflare, Google, Quad9, AdGuard, Yandex, etc.)

---

## ⚙️ Usage

> **Warning**: You need to run this script as `root` to modify `/etc/resolv.conf`.

```bash
sudo bash dns-selector.sh
```

---

## 🌍 Use Case

Ideal for:
- Countries with DNS censorship (like Iran)
- Environments with unreliable local DNS infrastructure
- Temporary troubleshooting for DNS issues

---

## 📁 Output

If successful, the last message will be:

```
✅ Updated /etc/resolv.conf with X working nameservers.
```

---

## 🇮🇷 فارسی

### 🎯 اسکریپت انتخاب خودکار DNS پاسخ‌گو

این اسکریپت Bash، لیستی از DNSهای رایج داخلی و خارجی را بررسی می‌کند و اولین ۵ موردی که پاسخ می‌دهند را انتخاب کرده و به فایل `resolv.conf/` اضافه می‌کند.

### 📌 ویژگی‌ها

- بررسی بیش از ۱۰۰ سرور DNS داخلی و خارجی
- انتخاب ۵ DNS سریع و پاسخگو
- تست سریع با `dig` و محدودیت زمان پاسخ
- نمایش نتیجه هر سرور با رنگ (سبز/قرمز)
- مناسب برای شرایطی با اختلال یا فیلترینگ DNS

### 🧪 نحوه استفاده

```bash
sudo bash dns-selector.sh
```

**توجه**: نیاز به دسترسی root دارید.

---

## 🇸🇦 العربية

### ⚡ سكربت لاختيار خوادم DNS السريعة تلقائيًا

هذا السكربت يقوم باختبار قائمة من خوادم DNS مسبقة التحديد، ويختار أول 5 خوادم تستجيب بنجاح لاستعلام DNS (مثل `google.com`) ثم يقوم بتحديث ملف `/etc/resolv.conf` بهذه الخوادم.

### ✅ الميزات

- يختبر خوادم DNS محلية وعالمية
- يختار أول 5 خوادم فعالة
- يستخدم `dig` مع وقت انتظار قصير
- يعرض النتائج بالألوان (أخضر/أحمر)
- يقوم بتحديث ملف `resolv.conf` تلقائيًا

### 📌 الاستخدام

```bash
sudo bash dns-selector.sh
```

**تنبيه**: يجب تشغيل السكربت بصلاحيات root.
