# Şu an ne yapmalıyım?

Bu dosya senin **tek görev panon**. ChatGPT'yi yanında açık tutmana gerek yok.

## Önce bunu yap — görünümü sadeleştir

VS Code'da `START_HERE.md` açıkken:

**Ctrl + Shift + V**

bas.

Bu, Markdown kodlarını gizleyip dosyayı **normal, okunabilir ders sayfası gibi** gösterir.

İstersen bu önizlemeyi solda, `uygulama.html` dosyanı sağda tut.

> Önemli: Ders notlarında gördüğün ` ```html ` ve ` ``` ` satırları sadece örnek kod kutusunu gösterir. Bunları `uygulama.html` içine yazma. Ekran görüntünde bu işaretlerden birkaçını HTML dosyana yazmışsın; devam etmeden önce o satırları sil.

---

# HC03 — Bu turda yapacağın 10 küçük görev

Hepsini `lessons/01-html-basics/uygulama.html` dosyasında yapacaksın.

Her görevde sana üç şey söylüyorum:

- **BUL:** mevcut kodunda neresi
- **YAP:** ne değiştireceksin
- **NEDEN:** ne işe yarıyor

Hepsi bitince tek commit + tek push yap.

---

## 1) HTML belgesi olduğunu belirt

**BUL:** Dosyanın en başındaki `<html>` satırını.

**YAP:** `<html>` satırının hemen üstüne bunu yaz:

```html
<!DOCTYPE html>
```

**NEDEN:** Tarayıcıya bunun modern bir HTML belgesi olduğunu söyler.

---

## 2) Sayfanın dilini belirt

**BUL:**

```html
<html>
```

**YAP:** Onu şuna çevir:

```html
<html lang="tr">
```

**NEDEN:** Sayfanın ana dilinin Türkçe olduğunu belirtir.

---

## 3) Türkçe karakter bilgisini ekle

**BUL:**

```html
<head>
```

**YAP:** `<head>` satırının hemen altına bunu yaz:

```html
<meta charset="UTF-8">
```

Yani bu bölüm kabaca şöyle olmalı:

```html
<head>
    <meta charset="UTF-8">
    <title>Benim İlk Sayfam</title>
</head>
```

**NEDEN:** `ş, ğ, ı, ç, ö, ü` gibi karakterlerin doğru okunmasına yardım eder.

---

## 4) Tarayıcı sekmesinin adını değiştir

**BUL:**

```html
<title>Benim İlk Sayfam</title>
```

**YAP:** Sadece iki etiket arasındaki yazıyı değiştir.

Örneğin:

```html
<title>Duhan'ın Web Laboratuvarı</title>
```

İstersen başka bir isim yaz.

**NEDEN:** Bu yazı sayfanın içinde değil, tarayıcı sekmesinde görünür.

---

## 5) Bir alt başlık ekle

**BUL:** `<body>` içindeki mevcut `<h1>...</h1>` satırını.

**YAP:** H1'in altına bir `h2` ekle.

Örnek:

```html
<h2>Öğrendiklerim</h2>
```

**NEDEN:** `h1` ana başlık, `h2` onun altındaki bölüm başlığıdır.

---

## 6) Üç maddelik liste ekle

**BUL:** Biraz önce eklediğin `h2` satırını.

**YAP:** H2'nin altına şu yapıda bir liste ekle:

```html
<ul>
    <li>HTML</li>
    <li>GitHub</li>
    <li>VS Code</li>
</ul>
```

İstersen maddeleri kendine göre değiştir.

**NEDEN:** `ul` listenin tamamı, her `li` ise tek bir listedir.

---

## 7) LinkedIn bağlantısını ekle

**BUL:** Mevcut GitHub bağlantını:

```html
<a href="https://github.com/ersagun13">GitHub Profili</a>
```

**YAP:** Hemen altına ikinci bir bağlantı ekle.

Hedef adresin:

```text
https://www.linkedin.com/in/duhan-ersagun-findikci
```

Görünen yazıyı sen seç.

Kontrol et:

- `href="..."` var mı?
- adres `https://` ile başlıyor mu?
- sonda `</a>` var mı?

---

## 8) Sayfayı üç bölüme ayır

Şimdi sadece `<body>` içindeki içerikleri düzenleyeceksin.

Hedef şu:

```text
<body>
    header  → h1
    main    → paragraf + h2 + liste + bağlantılar
    footer  → kısa kapanış cümlesi
</body>
```

Kullanacağın etiketler:

```html
<header>
</header>

<main>
</main>

<footer>
</footer>
```

### Tam olarak neyi nereye taşıyacaksın?

- Mevcut `h1` → `<header>` içine
- Mevcut `p` → `<main>` içine
- Yeni `h2` → `<main>` içine
- Yeni `ul` listesi → `<main>` içine
- GitHub ve LinkedIn bağlantıları → `<main>` içine
- Footer içine kendi kısa cümleni yaz

**NEDEN:** Bu etiketler sayfanın görünümünü otomatik değiştirmez. İçeriğin hangi bölümde olduğunu anlatır.

---

## 9) Girintileri düzelt

İçerideki satırları `Tab` ile biraz sağa kaydır.

Örnek:

```html
<body>
    <header>
        <h1>Başlık</h1>
    </header>
</body>
```

Kural basit:

> Bir satır başka bir etiketin içindeyse, bir kademe sağa girsin.

`Tab` → sağa

`Shift + Tab` → sola

---

## 10) Tarayıcı testi

Kaydet ve `uygulama.html` dosyasını tarayıcıda aç.

Kontrol et:

- Ana başlık görünüyor mu?
- Paragraf görünüyor mu?
- H2 görünüyor mu?
- 3 maddelik liste görünüyor mu?
- GitHub bağlantısı doğru yere gidiyor mu?
- LinkedIn bağlantısı doğru yere gidiyor mu?
- Tarayıcı sekmesinin adı değişti mi?

Bir şey yanlışsa önce kendi kodunda bulmaya çalış.

---

# En son dosyanın genel şekli nasıl olmalı?

Buradaki yazıları birebir kopyalama; bu sadece **harita**:

```text
DOCTYPE
html
├── head
│   ├── meta charset
│   └── title
└── body
    ├── header
    │   └── h1
    ├── main
    │   ├── p
    │   ├── h2
    │   ├── ul
    │   │   ├── li
    │   │   ├── li
    │   │   └── li
    │   ├── GitHub linki
    │   └── LinkedIn linki
    └── footer
        └── kısa cümle
```

---

# Bitirince

1. `Ctrl + S`
2. Tarayıcıda kontrol et
3. GitHub Desktop'u aç
4. Commit mesajı:

```text
HC03: complete HTML page structure
```

5. Commit
6. Push origin
7. ChatGPT'ye sadece `pushladım` yaz

Ben kodu GitHub'dan kontrol edeceğim. Hata varsa yalnızca yanlış olan görevi geri vereceğim.
