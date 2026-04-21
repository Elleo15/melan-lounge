# Melan Lounge — Sayt Təlimatı

## 📁 Fayl Strukturu

Bütün fayllar **eyni qovluqda** olmalıdır:

```
📁 melan/
├── melan-v3.html       ← Əsas sayt faylı
├── melan-logo.jpg      ← Logo
├── hall-1.jpg
├── hall-2.jpg
├── cabin-1.jpg
├── cabin-2.jpg
├── cabin-3.jpg
├── cabin-4.jpg
├── atmosfer-1.jpg
├── atmosfer-2.jpg
├── atmosfer-3.jpg
├── meal-1.jpg … meal-7.jpg
├── drink-1.jpg … drink-8.jpg
├── tea-set.jpg
├── video-1.mp4 … video-5.mp4
├── place-1.mp4
└── place-2.mp4
```

---

## ✏️ Tez-tez Dəyişdirilən Yerlər

### 🖼️ Şəkilləri dəyişmək
Sadəcə eyni adlı yeni şəkli qovluğa qoy. Məsələn `hall-1.jpg` ni dəyişmək istəyirsənsə — yeni şəkli `hall-1.jpg` adı ilə yadda saxla, köhnənin üstünə yaz.

### 📍 Ünvan / Telefon
HTML-də `Sumqayıt şəhəri, Nizami küçəsi 5` yazısını axtar, dəyiş.
Telefon üçün `+994 55 802 03 03` yazısını axtar, bütün yerlərini dəyiş (3 yer var — rezervasiya seksiyası, WhatsApp linki, footer).

### 🕐 İş saatları
`Hər gün: 13:00 – 01:00` yazısını axtar, dəyiş.

### 🍽️ Menyu qiymətlərini dəyişmək
HTML-də `menu-row-price` class-lı elementləri axtar. Hər sətir belə görünür:
```html
<span class="menu-row-price">8 ₼</span>
```
Qiyməti birbaşa dəyiş.

### 🌍 Məkanlar seksiyası şəkil ardıcıllığı
`sp-slide` class-lı div-ləri tap. Hər birinin içindəki `src="..."` ni istədiyin şəkillə dəyiş:
```html
<div class="sp-slide">
  <img src="BURAYA_ŞƏKİL_ADI.jpg" alt="">
```

### ⏱️ Hero animasiya sürəti
CSS-də `drawText` animasiyasını tap:
```css
animation: drawText 12s ...
```
`12s` — yazının çəkilmə vaxtı. Artırsan yavaşlayar, azaltsan sürətlənər.

Hero arxa fonun açılma vaxtı JS-də:
```js
setTimeout(() => { ... }, 12000);
```
`12000` = millisaniyə (12 saniyə). Animasiya vaxtı ilə eyni tut.

---

## 🌐 3 Dil Sistemi

Sayt **Azərbaycan, Rus, İngilis** dillərini dəstəkləyir. Dil dəyişdirmək üçün yuxarı sağdakı `AZ / RU / EN` düymələrindən istifadə olunur.

Mətnləri dəyişmək üçün JS-dəki `langs` obyektini tap:
```js
const langs = {
  az: { nav_about: 'Haqqımızda', ... },
  ru: { nav_about: 'О нас', ... },
  en: { nav_about: 'About', ... }
}
```
İstədiyin dildəki istənilən mətni birbaşa dəyiş.

---

## 📱 WhatsApp Rezervasiya

Forma doldurulub göndərildikdə avtomatik WhatsApp açılır. Nömrəni dəyişmək üçün JS-də aşağıdakı sətri axtar:
```js
https://wa.me/994558020303
```
Bu nömrə **3 yerdə** var — hamısını dəyiş.

---

## 🚀 Hostingə Yükləmək

1. Bütün faylları (HTML + şəkillər + videolar) hostingə yüklə
2. Əsas fayl `melan-v3.html` dir — hostingdə `index.html` adına dəyişmək tövsiyə olunur
3. Şəkil/video faylları HTML faylı ilə **eyni qovluqda** olmalıdır

---

## 🎨 Rəng Dəyişikliyi

CSS-nin əvvəlindəki `:root` dəyişənlərini tap:
```css
:root {
  --gold: #c9a84c;    ← Qızılı rəng
  --black: #0a0a0a;   ← Arxa fon
  --white: #f5f0e8;   ← Mətn rəngi
}
```

---

## 👤 Hazırladı

**Elvin Eyvazov** — © 2026 Melan Lounge. All rights reserved.
