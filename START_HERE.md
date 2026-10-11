# Şu an ne yapmalıyım?

Bu dosya eğitimdeki **tek çalışma panon** olsun. ChatGPT'yi açık tutmana gerek yok.

## Çalışma şekli

1. GitHub Desktop'ta **Fetch origin / Pull origin** ile güncellemeyi al.
2. VS Code'da bu dosyayı (`START_HERE.md`) ve `lessons/01-html-basics/uygulama.html` dosyasını aç.
3. İstersen sekmeye sağ tıklayıp **Split Right** ile görevleri solda, kodu sağda tut.
4. Aşağıdaki görevleri sırayla yap.
5. Tarayıcıda kendin kontrol et.
6. Hepsi bitince **tek commit + tek push** yap.
7. Sonra ChatGPT'ye yalnızca `pushladım` yaz. Kod GitHub reposundan kontrol edilecek.

> Doğru yaptığın görevler tekrar yaptırılmaz. Hata varsa yalnızca hatalı kısım geri verilir.

---

# Aktif çalışma seti — HC03: Tam HTML sayfası

## Amaç

Şu anda `uygulama.html` içinde `html`, `head`, `title` ve `body` yapısını doğru kurdun. Bu sette sayfayı gerçek bir temel HTML belgesine dönüştüreceksin.

Kısa mantık:

```text
html
├── head   → tarayıcıya/sayfaya ait bilgiler
└── body   → ziyaretçinin ekranda gördüğü içerik
```

---

## Görev 1 — Modern HTML belgesini belirt

Dosyanın en üstüne, `<html>` etiketinden önce şunu ekle:

```html
<!DOCTYPE html>
```

Bu satır tarayıcıya dosyanın modern HTML olarak yorumlanacağını söyler. Açılış/kapanış çifti yoktur.

---

## Görev 2 — Sayfanın dilini belirt

Şu satırı:

```html
<html>
```

şuna dönüştür:

```html
<html lang="tr">
```

`lang="tr"` sayfanın ana dilinin Türkçe olduğunu belirtir.

---

## Görev 3 — Türkçe karakter desteği ekle

`<head>` bölümünün içine şunu ekle:

```html
<meta charset="UTF-8">
```

Bu, `ş`, `ğ`, `ı`, `ç`, `ö`, `ü` gibi karakterlerin doğru yorumlanmasına yardımcı olur.

---

## Görev 4 — Tarayıcı sekmesinin adını değiştir

Mevcut `<title>` içeriğini kendine göre değiştir.

Örnek fikir: `Duhan'ın Web Laboratuvarı`

Aynısını yazmak zorunda değilsin. Buradaki amaç `<title>` metninin sayfanın içinde değil, **tarayıcı sekmesinde** göründüğünü görmek.

---

## Görev 5 — Bir bölüm başlığı ekle

`<body>` içinde ana başlığın (`h1`) dışında bir de `h2` kullan.

Örneğin konu olarak şunlardan birini seçebilirsin:

- Hakkımda
- Öğrendiklerim
- Web geliştirme yolculuğum
- Projelerim

`h1` ana başlıktır; `h2` onun altındaki bir bölüm başlığıdır.

---

## Görev 6 — En az 3 maddelik liste oluştur

Yeni etiketler:

```html
<ul>
    <li>Bir madde</li>
</ul>
```

- `ul` = madde işaretli listenin tamamı
- `li` = listedeki tek bir madde

Kendine ait en az **3 maddelik** bir liste yap. Örneğin şu anda öğrendiğin şeyleri yazabilirsin.

---

## Görev 7 — LinkedIn bağlantısı ekle

GitHub bağlantının yanına/altına ikinci bir bağlantı ekle.

Hedef adres:

```text
https://www.linkedin.com/in/duhan-ersagun-findikci
```

Görünen yazıyı sen seç.

Kendin kontrol et:

- `href="..."` var mı?
- Adres `https://` ile başlıyor mu?
- Bağlantı `</a>` ile kapanıyor mu?

---

## Görev 8 — Sayfayı anlamlı bölümlere ayır

Üç yeni etiket kullan:

```html
<header>
</header>

<main>
</main>

<footer>
</footer>
```

Bunlar kendi başlarına görünümü değiştirmez; içeriğin ne işe yaradığını anlatır.

Yerleşim hedefin:

```text
body
├── header → h1
├── main   → paragraf, h2, liste, bağlantılar
└── footer → kısa bir kapanış cümlesi
```

Footer cümlesini kendin yaz.

---

## Görev 9 — Girintileri düzenle

İç içe olan satırları sağa kaydır. Örneğin:

```html
<body>
    <header>
        <h1>Başlık</h1>
    </header>
</body>
```

Girinti tarayıcı için değil, kodu okuyan insan için önemlidir.

VS Code'da `Tab` ile sağa, `Shift + Tab` ile sola kaydırabilirsin.

---

## Görev 10 — Tarayıcıda kendi testini yap

Dosyayı kaydet ve tarayıcıda aç. Şunları tek tek kontrol et:

- Ana başlık görünüyor mu?
- Paragraf görünüyor mu?
- `h2` görünüyor mu?
- En az 3 maddelik liste görünüyor mu?
- GitHub bağlantısı doğru profile gidiyor mu?
- LinkedIn bağlantısı doğru profile gidiyor mu?
- Tarayıcı sekmesinde kendi verdiğin `<title>` görünüyor mu?

Bir şey bozuksa önce kendin HTML'e dönüp hatayı bulmaya çalış.

---

# Mini sınav

Kod bittikten sonra cevapları bir yere yazmana gerek yok. Push'tan sonra ChatGPT sana bunları soracak:

1. `<head>` ile `<body>` arasındaki temel fark nedir?
2. `<title>` nerede görünür?
3. `h1`, paragraf ve bağlantıları neden `<head>` içine koymuyoruz?
4. `header`, `main` ve `footer` sayfanın görünümünü otomatik değiştirir mi? Asıl amaçları nedir?
5. `ul` ve `li` arasındaki ilişki nedir?

---

## Bitirince

GitHub Desktop'ta tek commit oluştur.

Önerilen commit mesajı:

```text
HC03: complete HTML page structure
```

Ardından **Push origin** yap.

Sonra ChatGPT'ye yalnızca:

```text
pushladım
```

yazman yeterli.
