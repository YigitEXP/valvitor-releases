# Valvitor — Otomotiv Telemetri ve Akıllı Kokpit

**`Durum: Açık Beta (v1.0) • Tüm Pro Özellikler Aktif`**

Valvitor; gerçek zamanlı OBD-II araç telemetri verilerini, yüksek kontrastlı gece kokpiti deneyimini, organik rota haritalarını ve doğal Türkçe sesli sürüş asistanını tek arayüzde birleştiren yeni nesil Android otomotiv sistemidir.

---

## Hızlı İndirme ve Resmi Dağıtım

| Dağıtım Kanalı | Bağlantı | Açıklama |
| :--- | :--- | :--- |
| **Doğrudan APK İndir** | [En Son Sürüm (v1.0 Beta)](https://github.com/YigitEXP/valvitor-releases/releases/latest) | Doğrudan imzalı Release APK dosyası |
| **Resmi Web Vitrini** | [valvitor.web.app](https://valvitor.web.app) | Ürün özellikleri ve etkileşimli önizleme |
| **Sistem Uyumluluğu** | Android 8.0 (Oreo) ve üzeri | ARM64 & x86_64 mimarileri |

---

## Neyi, Neden Yaptık? (Tasarım ve Sürüş Deneyimi Tercihleri)

Geleneksel araç uygulamalarının yol açtığı aşırı pil tüketimi, gece kabin içinde göz kamaşması, karmaşık menüler ve gereksiz uyarı kalabalığı gibi sorunları çözmek için Valvitor'da her özelliği sürücü odaklı bir anlayışla geliştirdik:

### 1. Düşük Pil Tüketimi ve Cihazın Isınmaması İçin
- **Neden?** Telefon araç tutucusunda veya ön camda çalışırken şarjın çabuk bitmesi ve cihazın ısınması sürüş konforunu bozar.
- **Nasıl Çözdük?** Arayüzü hafif, enerji tasarruflu ve gereksiz arka plan işlemlerini durduran bir yapıyla kurduk. Araç dururken veya sabit hızda seyrederken veri akışını akıllıca dengeleyerek telefonun serin kalmasını sağladık.

### 2. Gece Sürüş Güvenliği ve Göz Kamaşmasını Önlemek İçin
- **Neden?** Gece sürüşlerinde parlak açık renkli ekranlar sürücünün gözünü yorar ve ön camda yansıma yaparak yolu görmeyi zorlaştırır.
- **Nasıl Çözdük?** Tüm kokpiti derin siyah ve kontrastı dengeli gece tonlarıyla tasarladık. Tek dokunuşla tüm ekranı karartan ve mavi ışığı süzen kehribar **OLED Dimmer** modunu ekledik. Ayrıca menülere girmeden temalar arasında geçiş yapabilmek için üst panelde pratik yatay kaydırma desteği sağladık.

### 3. Haritada Rota Çizgilerinin Üst Üste Binip Parlamasını Önlemek İçin
- **Neden?** Günlük kullanılan güzergahlardan defalarca geçildiğinde harita çizgileri üst üste binerek ekranı parlayan beyaz lekelere boğar ve sokakların görünmesini engeller.
- **Nasıl Çözdük?** Çizgileri ince tel veya aşırı parlak neon yapmak yerine, harita zeminine yumuşakça oturan yarı saydam **Saten Mürekkep** şeritleri kullandık. Sürüş detayında ise hız ve tempo değişimlerini yumuşak renk tonlarıyla göstererek viraj ve düzlük temposunun bir bakışta anlaşılmasını sağladık.

### 4. Sürüş Esnasında Dikkatin Dağılmaması İçin
- **Neden?** Sürekli ekrana bakmak zorunda kalmak veya uygulamanın aynı uyarıları peş peşe tekrarlaması dikkati yoldan ayırır.
- **Nasıl Çözdük?** Sürücüyü ekrana baktırmayan doğal Türkçe sesli sürüş koçu geliştirdik. Asistanın aynı uyarıyı arka arkaya seslendirip rahatsız etmesini kesin olarak engelledik. Motor henüz çalışma sıcaklığına ulaşmamışken sürücüyü nazikçe bilgilendiren soğuk motor uyarısı ekledik.

### 5. Çevrimdışı ve Kesintisiz Telemetri İçin
- **Neden?** Tünellerde veya hücresel verinin çekmediği kırsal yollarda veri akışının durması sürüş takibini engeller.
- **Nasıl Çözdük?** Standart araç adaptörleri üzerinden doğrudan kablosuz bağlantıyla çalıştık. İnternet paketiniz olmasa veya telefon hiç çekmese dahi anlık motor devri, soğutma suyu sıcaklığı, akü voltajı ve gaz tepkileri kesintisiz görüntülenir.

### 6. Geçmiş Sürüşleri Canlı İncelemek İçin
- **Neden?** Sürüş bittikten sonra yalnızca ortalama hız ve süre görmek, virajlarda aracın nasıl tepki verdiğini anlamak için yetersizdir.
- **Nasıl Çözdük?** Kaydedilen sürüşleri zaman çizelgesi üzerinde haritayla birlikte yeniden oynatabilen **Ghost Replay** özelliğini ekledik. Ayrıca en yüksek hız, en tempolu aralık gibi zirve anları otomatik özetleyen sosyal medya kartları hazırladık.

---

## Kurulum ve İzin Rehberi (Android 13 – 16)

Valvitor, bağımsız olarak imzalanmış güvenli APK formatında dağıtılmaktadır. Uygulamanın arka planda sorunsuz çalışması için gereken 3 temel adım:

| Ayar / İzin | Neden Gereklidir? |
| :--- | :--- |
| **Bilinmeyen Kaynak İzni** | İmzalı APK paketinin telefona yüklenebilmesi için gereklidir. |
| **Kısıtlı Ayarlar Kilidi (Android 13+)** | Bluetooth adaptörüne bağlanma ve sürüş servislerinin arka planda engellenmeden çalışabilmesi için gereklidir. |
| **Kesintisiz Arka Plan (Unrestricted Pil)** | Ekran kilitlendiğinde veya başka bir uygulamaya geçildiğinde GPS ve sürüş kaydının yarıda kesilmemesi için gereklidir. |

### Adım Adım Kurulum:
1. **İndirme ve Yükleme:** İndirilen `Valvitor-v1.0-Beta.apk` dosyasına dokunun. *"Bu kaynaktan izin ver"* seçeneğini onaylayın (Play Protect uyarısı çıkarsa *"Yine de Yükle"* seçeneğine dokunun).
2. **Kısıtlı Ayarlar Kilidini Açma:** **Ayarlar → Uygulamalar → Valvitor → Sağ üst üç nokta (⋮) → Kısıtlı ayarlara izin ver** seçeneğine dokunup onaylayın.
3. **Pil Kısıtlamasını Kaldırma:** **Ayarlar → Uygulamalar → Valvitor → Pil** adımından kullanımı **"Kısıtlanmamış"** olarak seçin.

---

## Özel Harita Temaları

- **Uydu & Sokak:** Güneş altında maksimum görünürlük sunan yüksek kontrastlı sokak katmanı.
- **Koyu Telemetri:** Gece sürüşleri için optimize edilmiş, gözü yormayan saf koyu arayüz.
- **1986 Retro Radar:** Analog göstergeleri anımsatan yeşil katmanlı retro radar estetiği.
- **Night City 2077:** Derin lacivert ve elektrik camgöbeği neon hatlara sahip kokpit teması.
- **Underground 2004:** Kült sokak yarışı atmosferini yaşatan koyu asfalt ve mor-kehribar tonları.

---

## Yol Haritası ve Açık Beta Erişimi

- **Açık Beta (v1.0 - Aktif):** Tüm harita temaları, canlı araç telemetrisi, Ghost Replay oynatıcısı ve Türkçe sesli sürüş koçu Açık Beta süresince **tamamen ücretsiz ve kilitsizdir**.
- **Yakında:** Tak-çalıştır modüler Valvitor araç adaptörü ve gelişmiş telemetri analiz özellikleri.

---

## Lisans ve İletişim

Valvitor Otomotiv Telemetri Sistemleri. Tüm hakları saklıdır.  
Resmi dağıtım ve sürüm takibi: [github.com/YigitEXP/valvitor-releases](https://github.com/YigitEXP/valvitor-releases)
