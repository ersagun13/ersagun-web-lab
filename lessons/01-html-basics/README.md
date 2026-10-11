# Ders 1 — HTML etiketleri

## Kısa teori

HTML, tarayıcıya içeriğin ne olduğunu söyler: başlık, paragraf veya bağlantı.

```html
<h1>Bir başlık</h1>
<p>Bir paragraf.</p>
<a href="https://ersagun.com.tr">Benim sitem</a>
```

- `<h1>` ana başlığı açar; `</h1>` kapatır.
- `<p>` paragrafı açar; `</p>` kapatır.
- `<a>` bağlantı oluşturur; `href` hedef adresi belirtir.
- Etiketlerin arasındaki yazı ekranda görünür.
- Tam bir web adresi için `https://` kullanılır. `github.com/ersagun13` tek başına yazılırsa tarayıcı bunu mevcut sayfaya göre bir yol olarak çözümleyebilir.
- HTTPS, tarayıcı ile site arasındaki iletişimi şifreler; tek başına bir sitenin güvenilir olduğunu kanıtlamaz.

Gerçek ersagun.com.tr kaynaklarında bulunan `<a href="/">Haritaya dön</a>` örneğinde `/`, bulunduğun sitenin kök adresidir. Burada yalnızca küçük ve herkese açık içerikli bir HTML örneği kullanılır.

## Uygulama

Kendi adını ana başlık, kendin yazdığın kısa bir cümleyi paragraf olarak yaz. Altına tam HTTPS adresi kullanan bir bağlantı ekle. Uygulama dosyasını öğrenci kendisi oluşturacak; bu not bir tamamlanmış öğrenci uygulaması değildir.

## Küçük ödev

GitHub ve Instagram profillerine iki ayrı bağlantı ekle. Her bağlantının görünen yazısı, hangi profile gittiğini anlatsın. Bağlantıların hedeflerini tarayıcıda kontrol et.

## Mini sınav

1. Normal bir paragraf için hangi etiketi kullanırsın?
2. `<p>Bir cümle.<p/>` örneğinde kapanışı nasıl düzeltirsin?
3. Bir bağlantının görünen yazısını değiştirince hedefi değişir mi? Neden?
4. `href="github.com/ersagun13"` ile `href="https://github.com/ersagun13"` arasında hedefin yorumlanması açısından ne fark vardır?

HC01 doğrulandı. HC02 için doğru bağlantı uygulaması ve 3–4. sorulara doğru açıklama gereklidir. Kontrol yapılmadan yeni konuya geçilmez.
