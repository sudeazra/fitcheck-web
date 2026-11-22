# FitCheck

Küçük bir arkadaş grubunun günlük kombinlerini paylaştığı, birbirinin kombinine
yorum yaptığı ve her gün en beğenilen kombini oyladığı bir web sitesi.
BLM2537 Ağ Tabanlı Programlamaya Giriş dersi dönem projesi.
HTML, CSS ve JavaScript ile yapılmıştır. Veriler tarayıcının localStorage'ında saklanır.
Sunucu, veritabanı veya kurulum gerektirmez.

## Nasıl çalıştırılır
1. Depoyu indirin (Code → Download ZIP) veya `git clone` ile klonlayın.
2. Klasörü VS Code ile açın.
3. `index.html` dosyasına sağ tıklayıp **Open with Live Server** seçin.
   (Live Server yoksa `index.html`'e çift tıklayarak da açılabilir.)

## Sayfalar
| Sayfa | İçerik |
|---|---|
| `index.html` | Giriş formu, uygulama tanıtımı |
| `feed.html` | Kombin paylaşma formu, bugünün sıralaması tablosu, bugünün kombinleri (oy, yorum) |
| `profile.html` | Profil bilgileri, istatistikler, profil düzenleme, kullanıcının bugünkü kombinleri |
| `history.html` | Kullanıcı seçimi, tarihe göre geçmiş kombinler, yorumlar, günün kazananı rozeti |

## Klasör yapısı
- `images/sample-fits/` — örnek kombin fotoğrafları (kullanıcı N'in kombinleri: sampleN, sampleN1, sampleN2 …)
- `images/sample-profilepic/` — profil fotoğrafları (pfp1 … pfp10)
- `images/apple.png` — site ikonu (favicon)

## Demo kullanıcıları
sude, gece, zeynep, bahar, cevat, eylul, derin, ruya, oyku, peri
(Şifreler JavaScript giriş kontrolü yazıldığında — 4. hafta — buraya eklenecek.)

## Notlar
- Şifreler yalnızca demo içindir, gerçek şifre değildir.
- Veriler tarayıcıya özeldir; farklı tarayıcı veya cihazda veriler görünmez.
  Aynı tarayıcıda farklı kullanıcılarla giriş-çıkış yapılarak kullanılır.
- Şu an sayfalardaki veriler örnek (elle yazılmış) verilerdir; ilerleyen haftalarda JavaScript ile
  localStorage'daki verilerden oluşturulacaktır.

## Haftalık İlerleme

### Hafta 1 (22–25 Ekim)
- Yapılanlar: GitHub deposu ve klasör yapısı, örnek görseller, favicon, `index.html`, `feed.html` (kazananlar tablosu dahil)
- Öğrenilenler: semantik HTML, form-label-input ilişkisi, tablo

### Hafta 2 (26 Ekim–1 Kasım)
- Yapılanlar: `profile.html`, fotoğrafların kullanıcılarla eşleştirilmesi, `.gitignore`, README
- Öğrenilenler: textarea, article kartları, Git commit düzeni

### Hafta 3 (2–8 Kasım)
- Yapılanlar: `history.html` yazıldı (kullanıcı seçimi, tarihe göre gruplanmış geçmiş kombinler, "Günün kazananı" rozeti, sadece okunur yorumlar); böylece 4 sayfa tamamlandı. Harici `style.css` oluşturulup bütün sayfalara bağlandı: renk paleti (CSS değişkenleri), yazı tipleri, kutu modeli ile kart görünümü ve kartlar arası boşluk. Ortak menü Flexbox ile yatay hale getirildi.
- Düzeltmeler: profil sayfasındaki yorum bölümü hatası ve Sil butonunun yeri düzeltildi, streak kaldırılıp yerine toplam paylaşılan kombin sayısı eklendi, footer'lar ortaklaştırıldı, kartlar arasındaki `<hr>` çizgileri kaldırıldı.
- Plandan sapma: akıştaki "dünün kazananları" tablosu, oy verildiğinde anında değişsin diye "Bugünün sıralaması" oldu; tabloya kombin fotoğrafı sütunu eklendi. Günün kesin kazananı geçmiş sayfasında rozetle görünüyor.
- Öğrenilenler: `select`/`option`, CSS seçicileri, CSS değişkenleri, kutu modeli (margin, border, padding), Flexbox.