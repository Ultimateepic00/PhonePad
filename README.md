<div align="center">
  <img src="logo.png" alt="PhoneController Logo" width="140" height="140" />

  # 📱 PhonePad 💻
  ### **PC Remote, Low-Latency Touchpad & Wireless Microphone**
  ### **حوّل هاتفك إلى لوحة تحكم، ماوس سريع، ومايكروفون لاسلكي للكمبيوتر**

  <p align="center">
    <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D6?style=for-the-badge&logo=windows&logoColor=white" />
    <img src="https://img.shields.io/badge/Mobile-Android%20(APK)-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
    <img src="https://img.shields.io/badge/Touchpad-60%20FPS-FF4500?style=for-the-badge&logo=speedtest&logoColor=white" />
    <img src="https://img.shields.io/badge/Security-AES--256--GCM-success?style=for-the-badge&logo=letsencrypt&logoColor=white" />
    <img src="https://img.shields.io/badge/License-MIT%20Open%20Source-purple?style=for-the-badge" />
  </p>
</div>

---

> ⚠️ **المشروع قيد التطوير.** المزايا المذكورة هنا هي خطة النسخة الأولى، وبتتعلّم كمكتملة في قسم خارطة الطريق لما تتنفّذ فعلًا.

## 🌟 نظرة عامة | Overview

**PhonePad** مشروع مفتوح المصدر يربط هاتفك الأندرويد بجهاز الكمبيوتر (Windows 10/11) باستجابة سريعة على الشبكة المحلية (الهدف من **20 إلى 50 مللي ثانية** على Wi-Fi). تصميم السيرفر مستوحى من بساطة `PhoneMic v0.4.1`، مع إضافات للتحكم في النظام والوسائط.

---

## 🔥 المميزات المخططة | Planned Features

| القسم (Category) | المميزات (Features) |
| :--- | :--- |
| **📡 الاتصال**<br>*(Connection)* | • **Wi-Fi (LAN)** مع اكتشاف تلقائي للشبكة أو ربط سريع عبر **QR Code**.<br>• **USB** و**Bluetooth** في مرحلة لاحقة.<br>• تشفير البيانات بـ **AES-256-GCM** بمفتاح مشتق من الـ PIN عبر PBKDF2. |
| **🖱️ تاتش باد 60 إطار/ثانية**<br>*(60FPS Touchpad)* | • نقرة بإصبع (كليك شمال) \| نقرة بإصبعين (كليك يمين) \| ضغطة مطولة (Drag & Drop).<br>• تمرير بإصبعين (Scroll) \| تقارب وتباعد الأصابع (**Pinch to Zoom**). |
| **🎙️ مايكروفون لاسلكي**<br>*(Wireless Mic)* | • زر يحوّل مايكروفون الهاتف إلى مايك لاسلكي للويندوز، مثالي للمكالمات والتسجيل. يحتاج تثبيت **VB-CABLE** على الكمبيوتر. |
| **🎵 تحكم بالوسائط**<br>*(Media Keys)* | • 11 زر وسائط: `Play/Pause`, `Next`, `Prev`, `Stop`, `Mute`, `Vol+`, `Vol-`, `Repeat`, `Shuffle`، وتقديم/تأخير بثواني قابلة للتخصيص.<br>• **توجيه الأوامر لبرنامج محدد** حتى لو كان في الخلفية. |
| **🎚️ مكسر صوت التطبيقات**<br>*(Per-App Volume Mixer)* | • التحكم في مستوى صوت كل برنامج مفتوح على الويندوز من شاشة الهاتف. |
| **⚙️ النظام والكيبورد**<br>*(System & Keyboard)* | • `Shutdown`, `Restart`, `Sleep`, `Screenshot`, `Show Desktop`, `Alt+Tab`، والتحكم في **سطوع الشاشة**.<br>• كيبورد كامل + وضع الأزرار الخاصة (`Ctrl, Alt, Shift, Win, Esc, F1-F12`).<br>• مشاركة الحافظة (**Clipboard Sync**) بتفعيل يدوي. |
| **🎨 واجهة قابلة للتخصيص**<br>*(Customizable UI)* | • 3 أوضاع: **Light**, **Dark**, و **AMOLED Pure Black**.<br>• اهتزاز لمسي (**Haptic Feedback**) بشدة قابلة للتحكم.<br>• وضع عمودي وأفقي وترتيب أزرار قابل للتخصيص. |

---

## 🖥️ سيرفر الويندوز | Windows Server

* يعمل في الـ **System Tray** (بجوار الساعة) مع خيار التشغيل مع الويندوز.
* واجهة إعدادات نظيفة تعرض الـ IP والمنفذ والـ PIN وصورة الـ QR وحالة المايك.
* لو المنفذ مشغول، يبحث السيرفر عن منفذ فارغ ويطلب من المستخدم التأكيد أو التغيير.

---

## 🗺️ خارطة الطريق | Roadmap

- [ ] **النسخة الأولى (MVP):** التاتش باد 60FPS + أزرار الوسائط والصوت والنظام + المايك اللاسلكي.
- [ ] **اتصال USB و Bluetooth.**
- [ ] **وضع يد التحكم للألعاب (Gamepad Mode)** مع إعدادات جاهزة لأشهر الألعاب.
- [ ] **نقل الملفات السريع** بين الهاتف والكمبيوتر.

---

## 📥 التحميل والتثبيت | Download & Installation

1. افتح قسم **[Releases](../../releases)** في هذا المستودع.
2. حمّل **`PhonePad_Server.exe`** على جهاز الكمبيوتر (Windows 10 / 11).
3. حمّل **`PhonePad_App.apk`** وثبّته على هاتفك الأندرويد.
4. (للمايك اللاسلكي) ثبّت **[VB-CABLE](https://vb-audio.com/Cable/)** على الكمبيوتر.
5. افتح السيرفر، امسح كود الـ **QR** أو أدخل الـ **PIN**، وابدأ التحكم.

> الهاتف والكمبيوتر لازم يكونوا على نفس شبكة Wi-Fi. لو ظهر تنبيه من Windows Firewall اسمح للبرنامج على الشبكة الخاصة.

---

<div align="center">
  <b>مشروع مفتوح المصدر بالكامل ❤️ | Free & Open Source Software (MIT)</b>
</div>
