# Değerlendirme ve ilerleme

Son değerlendirme: **12 Ekim 2026 · Europe/Istanbul**.

**Genel: 2 / 20 → %10.** Bu eğitim tamamlama oranıdır; genel geliştirici yeterliliği ölçümü değildir.

| Kod | Kontrol noktası | Durum |
| --- | --- | --- |
| HC01 | Başlık, paragraf ve açılış/kapanış etiketleri | Tamamlandı |
| HC02 | Bağlantılar ve tam/göreli adresler | Tamamlandı |
| HC03 | Tam HTML sayfası: head, body ve anlamlı yapı | Başlanmadı |
| HC04 | CSS: seçiciler, renkler ve yazı biçimi | Başlanmadı |
| HC05 | Kutular, yerleşim ve mobil uyumlu mini sayfa | Başlanmadı |
| JS01 | Değişkenler, değerler ve tarayıcı konsolu | Başlanmadı |
| JS02 | DOM: sayfadaki bir öğeyi bulmak ve değiştirmek | Başlanmadı |
| JS03 | Tıklama olayları, koşullar ve fonksiyonlar | Başlanmadı |
| JS04 | Diziler, döngüler ve küçük bir liste uygulaması | Başlanmadı |
| JS05 | Klavye desteği olan etkileşimli mini proje | Başlanmadı |
| GC01 | Repo, yerel kopya ve değişiklikleri görmek | Başlanmadı |
| GC02 | Commit, push ve pull işlemlerini açıklayıp yapmak | Başlanmadı |
| GC03 | Geçmişi incelemek ve bir hatayı güvenle geri almak | Başlanmadı |
| GC04 | Ayrı branch üzerinde çalışmak ve pull request açmak | Başlanmadı |
| GC05 | Otomatik kontrol ve eğitim ortamına yayın akışı | Başlanmadı |
| CD01 | Statik site, sunucu ve Cloudflare'ın rolü | Başlanmadı |
| CD02 | DNS: A, CNAME, MX ve TXT kayıtlarını ayırt etmek | Başlanmadı |
| CD03 | HTTPS, sertifika ve yönlendirme mantığı | Başlanmadı |
| CD04 | Hesap güvenliği, erişim yetkisi ve gizli anahtarlar | Başlanmadı |
| CD05 | Ayrı eğitim ortamında yayın, kontrol ve geri dönüş | Başlanmadı |

## Doğrulanan kanıt

### HC01 — Başlık ve paragraf

Öğrenci başlığı `h1`, paragrafı `p` ile yazdı. Paragraf için `p` seçilmesi gerektiğini doğru söyledi. Hatalı paragraf kapanışını bağımsız biçimde `</p>` olarak düzeltti. Bu uygulama ve soru yanıtı ilk kontrol noktasını karşılar.

### HC02 — Bağlantılar

Öğrenci `lessons/01-html-basics/uygulama.html` dosyasını VS Code'da kendisi oluşturdu. GitHub bağlantısında tam `https://` adresi ve doğru `</a>` kapanışı kullandı; dosyayı tarayıcıda açtı ve bağlantının görüntülendiğini kontrol etti.

Mini sınavda görünen bağlantı yazısının hedefi belirlemediğini, hedefin `href` içinde bulunduğunu doğru açıkladı. `https://` bulunmayan `github.com/ersagun13` biçiminin mevcut sayfaya göre bir yol gibi yorumlanabileceğini kendi cümleleriyle ifade etti. HC02 tamamlandı.

## Kurulum kaydı

Public eğitim reposu ve `main` branch doğrulandı. Windows yerel kopyası `D:\web-lab\ersagun-web-lab` konumunda görüldü. İlk öğrenci uygulaması GitHub Desktop ile commit edildi ve push sonrasında GitHub `main` branch üzerinde bağımsız olarak doğrulandı.

Bu işlemler GitHub kullanım pratiğidir; Git / CI-CD bölümündeki kontrol noktalarını tek başına tamamlamaz.

## Sıradaki görev

HC03 kapsamında mevcut `uygulama.html` dosyasını tam bir HTML sayfasına dönüştürmek: `html`, `head`, `title` ve `body` bölümlerinin ne işe yaradığını öğrenmek, kodu öğrencinin kendisinin yazması ve sonucu tarayıcıda kontrol etmek.

Asıl değerlendirme verisi [progress.json](../progress.json) dosyasındadır. Durum değişirken bu özet ve README de güncellenir. Geçmiş bir değerlendirme düzeltilirse nedeni ayrıca kaydedilir.
