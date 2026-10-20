# XOLERIC ∞ · 10 sotix hovli

**10 sotixli hovli uyining 3D interaktiv sahna** — bitta HTML fayl, Three.js (r128) va boshqa hech narsa yo'q.
Brauzerda ochsangiz bas. Internet ham, server ham kerak emas — Three.js kutubxonasi `three.min.js` faylda mahalliy saqlangan.

🌐 **Onlayn:** <https://xolerc.github.io/xoleric-home/>

---

## 🎮 Rejimlar (4 ta kamera)

| Rejim | Tugma | Nimani ko'rsatadi |
|---|---|---|
| **Ko'cha** | `Ko'cha` | Ko'chadan turib — hovli devori orqasidagi uy ichi ko'rinmaydi, faqat tom va darvoza |
| **Hovli** | `Hovli` | Hovli ichidan yuqoridan 3/4 ko'rinish — uy, bog', personajlar |
| **Ichki** | `Ichki` | Uyning ichida birinchi shaxs ko'rinishida yurish (WASD / tugma) |
| **Tepadan** | `Tepadan` | To'liq hovli xaritasi; tom shaffof, ichki mebel ko'rinadi |

## 🛠 Asboblar (3 ta)

- **Kamera** — chap tugma bilan aylantirish, g'ildirak bilan masofa
- **Jang** — personaj ustiga bosing (2.3 m ichida). 3 zarba = **KO**, ochko'z +1 kuch beradi
- **Chizish** — kub / shar / daraxt / chiroq shakllarini chizing. Chizilganlar `localStorage`'da saqlanadi

## ⌨️ Boshqaruv

| Harakat | Sichqoncha | Telefon |
|---|---|---|
| Aylantirish | chap tugma (yoki o'ng tugma) | bitta yoki ikki barmoq |
| Masofa / zoom | g'ildirak | pinch (qisqartirish) |
| Yurish (ichki) | `W` `A` `S` `D` / o'q strelkalari | chap pastdagi tugma (joystick) |
| Jang / chizish | chap tugma | chap tugma |

## ✨ Nima qo'shildi

- **Offline ishlaydi** — `three.min.js` mahalliy; CDN faqat zaxira sifatida
- **Ko'p CDN zaxirasi** + aniq "yuklanmadi" xabari (bo'sh oq sahifa qolmaydi)
- **Jon / KO / kuch** o'yin sikli: personajlar 3 zarbadan keyin yiqilib ketadi
- **Eshik** — uyning oldida haqiqiy ochiq eshik bargi (personajlar shu teshikdan o'tadi)
- **Parraklar** — 4 ta ichki + 4 ta tashqi; tugma bilan yoqiladi/o'chiriladi
- **Shrift bloklamaydi** — sekin internetda ham sahna darhol ochiladi
- **Mobil moslashuv** — portret ekranda kamera avtomatik uzoqlashadi, joystick, ikki barmoq bilan aylantirish
- **Chizilganlar saqlanadi** — sahifa yangilansa ham yo'qolmaydi
- **WebAudio** — zarba, KO va chizish ovozlari (tashqi fayl yo'q)
- **FPS ko'rsatkichi** + zaif qurilma uchun avtomatik sifat pasaytirish
- **To'liq dispose** — GPU xotirasi oshib borMAYdi (chizilgan obyektlar va halqalar)

## 🗂 Tuzilma

```
index.html              ← butun o'yin (HTML + CSS + JS)
three.min.js            ← Three.js r128 (MIT), mahalliy
.github/workflows/pages.yml  ← GitHub Pages avtomatik deploy
.nojekyll
```

## 🚀 Joylash (GitHub Pages)

`main` branshi push qilinganda workflow avtomatik ishga tushadi va
<https://xolerc.github.io/xoleric-home/> manziliga joylaydi.

```bash
git clone git@github.com:xolerc/xoleric-home.git
cd xoleric-home
# fayllarni o'zgartiring
git add -A && git commit -m "update" && git push
```

## 🧱 Texnologiya

Three.js `r128` · WebGL · WebAudio · localStorage · bitta fayl · chetdan hech narsa talab qilinmaydi

© XOLERIC
