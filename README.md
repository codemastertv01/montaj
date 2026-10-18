# Montaj Pro Studio 3.1

Qisqa kliplar + ovoz fayllari + matn → subtitrli, platformalarga tayyor video.
**Har safar yangi montaj**: bir xil materialdan har gal boshqa ritm, kamera harakati,
o'tishlar, rang va subtitr uslubi chiqadi.

## Imkoniyatlar

**Montaj (har safar yangi)**
- 6 ta montaj uslubi: Kinematik, Dinamik, Energetik, Hujjatli, Orzumand, Minimal + **Avto**
- Kadr uzunligi qat'iy emas (5s / 6.5s / 4s emas) — uslub oralig'idan tasodifiy, "nafas oladigan" ritm
- Kesimlar gap chegaralariga (pauza, nuqta) tushadi, yangi ovoz fayli = yangi kadr
- Kamera harakatlari: push-in, pull-out, pan, tilt, drift, yaqin plan — silliq (smoothstep)
- Sekin harakat, teskari, stop-kadr, "zarb" zoom (punch-in)
- 11 xil o'tish: fade, dissolve, qorong'ilik, oq chaqnash, whip, zoom, blur, doira, surilish
- 8 ta rang "look": Tabiiy, Kino (teal & orange), Iliq, Sovuq, Yorqin, Matte, Vintage, Qora-oq
- Kino polosalari (2.39:1), grain + vignette
- **Seed**: shu seed — aynan shu montaj. «Yangi variant» — yangi seed; «Shu montajni yangi sozlamalar bilan» — kesimlar o'sha, faqat subtitr/rang/matn o'zgaradi
- 10 video + 10 ovoz bo'lsa — avtomatik **1-video → 1-ovoz** rejimi (yoki «Aralash»)

**Subtitr (CapCut darajasida)**
- 14 shablon: Karaoke, Hormozi, MrBeast, Quti (CapCut), Sakrovchi, Paydo bo'lish, Karaoke oqim,
  Ko'tarilish, Neon, Komiks, Klassik, Nafis, Minimal, Pop + **Avto**
- Hammasi sozlanadi: shrift (18 ta + o'zingizniki), o'lcham, katta harf, matn/urg'u/kontur/fon/neon
  ranglari, kontur va soya qalinligi, joylashuv (tepa/o'rta/past) va siljitish, bir ekrandagi so'zlar,
  1–2 qator, paydo bo'lish animatsiyasi, so'z effekti
- Matnda `*so'z*` — urg'u rangida chiqadi; raqamlar avtomatik ajratiladi
- Jonli ko'rinish (preview) — o'zgarishni darhol ko'rasiz

**Matn, hook va CTA elementlari** (xohlagancha, har biri to'liq sozlanadi)
- 18 shablon: Katta sarlavha, Sariq quti, Stiker, Diqqat-lenta, Raqam/fakt, Minimal yorliq, Neon,
  Yozuv mashinkasi, Pastki yozuv (ism), @kanal belgisi, Yakuniy ekran;
  CTA: **Subscribe, Like, Comment, Share, Save, Bell, Follow** va Combo
- Matn: shrift, o'lcham, rang, urg'u rangi (`*so'z*`), kontur, soya, neon, shaffoflik, katta harf
- Fon: rang, zichlik, **burchak radiusi** (to'rtburchakdan "pill"gacha), ichki bo'shliq,
  ramka (border) qalinligi va rangi, qiyalik, orqa videoni qoraytirish
- Ikonkalar (qo'ng'iroqcha, like, izoh, ulashish, saqlash, yurak, play ...) va ularning rangi
- Animatsiya: kirish (sakrab, kattadan, o'sib, ko'tarilib, **4 tomondan uchib**, aylanib, xiradan,
  yozuv mashinkasi) → ekranda (puls, tebranish, suzish, yurak urishi) → chiqish (4 tomonga uchib ...)
- **Bosish animatsiyasi**: kursor kelib tugmani bosadi → «Obuna boʻldingiz ✓» (rang/matn/ikonka o'zgaradi) + ovoz
- Vaqt: boshidan / oxiridan / foizda; joy — jonli ko'rinishda **sichqoncha bilan suriladi**
- **Muqobil matnlar** — har variantda boshqasi (hook A/B test)
- Progress bar, logo/watermark

**Muqova (obloshka) muharriri** — videodan alohida, 16:9 (YouTube) va 9:16 (Shorts/Reels) uchun:
- Fon: o'z rasmingiz yoki **videodan istalgan kadr**; zoom, surish, yorqinlik, kontrast, to'yinganlik,
  xiralik, rang tusi, qorong'i gradient (chap/o'ng/past/tepa), vinyetka
- Qatlamlar: **matn** (shrift, o'lcham, rang, urg'u `*so'z*`, kontur, soya, neon, harf/qator oralig'i,
  fon qutisi + radius, qiyalik), **rasm/stiker** (doira kesim, ramka, soya, ko'zgu), **shakllar**
  (to'rtburchak, doira, strelka, chiziq), **ikonkalar**
- Kanvasda sichqoncha bilan surish, sariq burchak — kattalashtirish, strelka tugmalari — aniq surish
- 8 shablon: Hayratli (MrBeast), Savol qutisi, Hujjatli kino, Katta raqam, Neon, Qizil lenta, Minimal
- Ekranda ko'ringan rasm = yakuniy fayl (brauzer kanvasida chiziladi); YouTube'ga ham shu yuklanadi
- **Videoning boshiga qo'shish** (0.15–1.5 s) — Shorts/Reels/TikTok'da muqova sifatida tanlash uchun
- **Yakuniy ko'rinish**: YouTube lentasidagi kartochka, pleyer, telefondagi Shorts va profil to'ri —
  muqova + video birga. Muqovani o'zgartirsangiz, «Joriy muqovani shu variantga qo'llash» —
  qayta render qilmasdan

**Loyihalar**: hammasi diskda saqlanadi (`ishlar/<id>/project.json`) — sahifa yangilansa ham,
server qayta ishga tushsa ham yo'qolmaydi. «Loyihalar» oynasi: ochish, nusxa olish, o'chirish,
nomini o'zgartirish. Har bir render — saqlanadigan **variant**: ⭐, «Sozlamalarni tiklash»
(muharrirga qaytarib o'zgartirish), «Shu montaj + yangi sozlamalar», o'chirish.
Bir yo'la 1–3 variant buyurtma qilish mumkin — ular **navbat** bilan render qilinadi.
Havola: `http://localhost:8001/?p=<loyiha_id>`

**Montajchi qo'shimchalari**: kesimlarni **musiqa zarbiga** moslash (beat-sync), kalit so'zlarni
avtomatik ajratish, fayl sifati (kichik hajm / standart / yuqori)

**Platformalar** (har biri o'z xavfsiz zonasi bilan): YouTube 16:9, YouTube Shorts, TikTok,
Instagram Reels, Facebook Reels, Instagram/Facebook lenta 4:5, Kvadrat 1:1, Facebook 16:9.
**Avto** — 9:16 kliplardan Shorts, 16:9 dan YouTube. Bir xil o'lchamdagi formatlar bir marta render qilinadi.

**Audio**: ovozlarni ulash, pauzalarni qisqartirish, maqsadli uzunlikka tezlashtirish (maks. 1.25x),
tozalash + kompressor, −14 LUFS, fon musiqasi (ducking, fade), o'tish ovoz effektlari

**Nashr**: SRT, YouTube boblari, muqova 1280×720 va vertikal 1080×1920, post matni
(sarlavha + tavsif + boblar + heshteglar), YouTube'ga to'g'ridan-to'g'ri yuklash

## O'rnatish

Faqat **Python 3.8+** va **ffmpeg** kerak (qo'shimcha kutubxona shart emas).

```bash
# Fedora — standart "ffmpeg-free" da libx264 yo'q, to'liq ffmpeg (RPM Fusion) tavsiya etiladi:
sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
sudo dnf swap ffmpeg-free ffmpeg --allowerasing
# Arch / Manjaro
sudo pacman -S ffmpeg
# Ubuntu / Debian
sudo apt install ffmpeg
```

Dastur bir nechta ffmpeg'ni o'zi tekshiradi va subtitr chiza oladiganini tanlaydi (`ffbin.py`).
libx264 bo'lmasa `libopenh264` ga o'tadi (ishlaydi, lekin fayl kattaroq / sifati biroz past).
Qo'lda tanlash: `MONTAJ_FFMPEG=/yo'l/ffmpeg python3 app.py`.

**VS Code Flatpak** ichidan ishga tushirsangiz ham ishlaydi: Flatpak'dagi ffmpeg'da subtitr
(libass) yo'q, shuning uchun dastur avtomatik `flatpak-spawn --host` orqali tizim ffmpeg'idan foydalanadi.

## Ishga tushirish

```bash
cd montaj_pro
python3 app.py
```

Brauzerda oching: **http://localhost:8001**

1. Videolarni tashlang (tartib fayl nomi bo'yicha: `1.mp4`, `2.mp4` …)
2. Ovoz fayllarini tashlang, har birining ostiga matnini yozing
3. Format(lar) — yoki **Avto**
4. Montaj uslubi va rang — yoki **Avto** (har safar yangi)
5. Subtitr shablonini tanlang va sozlang (o'ngda jonli ko'rinish)
6. «Montajni boshlash». Yoqmasa — «Yangi variant»

### Buyruq qatoridan

```bash
python3 montaj.py \
  --clips 1.mp4 2.mp4 3.mp4 4.mp4 5.mp4 6.mp4 7.mp4 8.mp4 9.mp4 10.mp4 \
  --audio 1.mp3 2.mp3 3.mp3 4.mp3 5.mp3 6.mp3 7.mp3 8.mp3 9.mp3 10.mp3 \
  --texts 1.txt 2.txt 3.txt 4.txt 5.txt 6.txt 7.txt 8.txt 9.txt 10.txt \
  --formats youtube,shorts,tiktok --subs hormozi \
  --sub-style '{"font":"Anton Regular","position":"middle","size":1.1}' \
  --accent "#3CF06E" --pack auto --target 3:00 --tighten \
  --hook "Qadimda choʻlda MUZ qanday qilingan?" --cta "Obuna boʻling!" --progress-bar top \
  --overlays @elementlar.json --quality small --beat-sync --music musiqa.mp3 --auto-emph \
  --title "Choʻldagi muz" --out natija/video.mp4
```

Aynan shu montajni qaytarish: `--seed 123456` (seed natija oxirida chiqadi).
Barcha sozlamalar: `python3 montaj.py --help`

## Subtitr qanday ishlaydi

Matn berilsa, dastur ovozdagi pauzalarni topadi va so'zlarni ularga optimal
taqsimlaydi (dinamik dasturlash). Sun'iy ovozda (TTS) gap chegarasidagi
o'rtacha xato **~50–90 ms** — ko'z sezmaydi.

- Matn ovozda aytilgan so'zlarga **aynan** mos bo'lsin
- Raqamlarni raqam bilan yozing (`10`) — ular avtomatik urg'u rangida chiqadi
- O'zbekcha matnda `o'` va `g'` avtomatik `oʻ` `gʻ` ga aylanadi (inglizcha matnga tegilmaydi)
- Shriftda `ʻ` belgisi bo'lmasa, o'xshash belgiga almashtiriladi

Matn bo'lmasa, `--whisper` bilan ovozdan tanib olish mumkin (`pip install faster-whisper`).

## O'z shriftingiz

Interfeysda «+ O'z shriftim (.ttf)» yoki `.ttf`/`.otf` faylni `fonts/` papkasiga tashlang —
avtomatik paydo bo'ladi. Qo'shilgan shriftlar: Google Fonts (SIL OFL / Apache 2.0 litsenziyasi).

## YouTube'ni ulash (bir martalik)

```bash
pip install google-api-python-client google-auth-oauthlib
```

1. https://console.cloud.google.com → yangi loyiha yarating
2. **APIs & Services → Library** → «YouTube Data API v3» → **Enable**
3. **OAuth consent screen** → User type: **External** → ilova nomi, email →
   **Test users** ga o'z Gmail'ingizni qo'shing
4. **Credentials → Create credentials → OAuth client ID** → turi: **Desktop app**
5. JSON faylni yuklab oling va shu papkaga **`client_secret.json`** nomi bilan qo'ying
6. Interfeysda «YouTube'ga ulanish» → brauzerda ruxsat bering

**Yuklash tartibi** (8-bo'lim → «Video tayyor bo'lgach»):
- **Yuklashdan oldin so'rash** (tavsiya) — render tugashi bilan «YouTube'ga jo'natishga rozimisiz?»
  oynasi chiqadi: videoni ko'rasiz, format (Shorts / 16:9), sarlavha, tavsif, teglar, ko'rinish,
  til, rejalashtirishni tekshirasiz va «Ha, yuklash» ni bosasiz. Sahifa yopilgan bo'lsa ham,
  keyingi ochilishda so'raydi. «Yo'q, keyinroq» — variant ostidagi «YouTube'ga yuklash…» tugmasi qoladi
- **Avtomatik** — so'ramasdan yuklaydi; **Hech narsa** — faqat qo'lda

Muqova (thumbnail) o'rnatish uchun kanal telefon orqali tasdiqlangan bo'lishi kerak:
https://www.youtube.com/verify

**Audit**: tekshiruvdan o'tmagan API loyihasidan yuklangan videolar **faqat «private»**
rejimda qoladi. Ommaviy qilish uchun: https://support.google.com/youtube/contact/yt_api_form

## Fayllar

| Fayl | Vazifasi |
|---|---|
| `app.py` | Server (API), loyihalar va render navbati |
| `ui.html` | Brauzer interfeysi (jonli ko'rinish bilan) |
| `cover.js` | Muqova (obloshka) muharriri va yakuniy ko'rinish |
| `montaj.py` | Montaj dvigateli (render, audio, muqova) |
| `styles.py` | Ijodiy dvigatel: uslublar, ranglar, o'tishlar, kesimlar, seed |
| `subtitles.py` | Matnni ovozga moslash, 14 subtitr shablon, progress bar, SRT, boblar |
| `overlays.py` | Matn / hook / CTA elementlari: ikonkalar (SVG→ASS), fon, animatsiya, bosish |
| `fontmetrics.py` | Har qanday TTF/OTF shriftni o'qish (qatorlarni aniq bo'lish uchun) |
| `ffbin.py` | To'g'ri ffmpeg'ni topish (Flatpak, libx264/openh264) |
| `youtube.py` | YouTube'ga yuklash |
| `fonts/`, `sfx/` | Shriftlar va ovoz effektlari |
| `ishlar/` | Interfeys orqali qilingan ishlar (o'chirib tashlash mumkin) |
| `ROADMAP.md` | Kelajakdagi imkoniyatlar tahlili |

## Muammolar

- **`Unknown encoder 'libx264'`** — tizimda `ffmpeg-free`. Dastur endi o'zi `libopenh264` ga o'tadi; eng yaxshisi — RPM Fusion ffmpeg (yuqorida)
- **`No option name near 'subs.ass:fontsdir=fonts'`** — ishlatilgan ffmpeg'da libass yo'q (masalan Flatpak ichidagisi). Dastur endi subtitr chiza oladigan ffmpeg'ni o'zi tanlaydi
- **Render sekin** — `--smooth` o'chirilganini tekshiring; 60 fps o'rniga 30 fps
- **Subtitr kechikadi** — matn ovozga aynan mosligini tekshiring
- **Kliplar xira** — 1080p manbada kuchli krop yumshoq chiqadi; 1440p yoki 4K generatsiya qiling
