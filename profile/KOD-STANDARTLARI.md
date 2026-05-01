# Kod Standartları

Bu organizasyondaki donanım repoları için kanonik kodlama referansı:

- Kaynak doküman: <https://www.akkoyun.net/acik-kaynak/kod-standartlari/>
- Sürüm: `02.00.01 [V2]`

## Kod Yapısı

Kanonik format:

`ABbbCD-(G)-(Eeeeee)-(F)`

Örnek:

`B403BA-PCIe`

- `A` → segment
- `Bbb` → grup kodu
- `C` → ana revizyon
- `D` → bugfix / alt revizyon
- `G` → opsiyonel form / platform / arayüz eki
- `Eeeeee` → opsiyonel ek alan
- `F` → opsiyonel ek alan

## Segmentler

- `P` → Product
- `A` → Assembly
- `B` → Board
- `C` → Casting
- `M` → Metal
- `H` → Hardware
- `W` → Wire
- `S` → Sticker
- `E` → Electrical

## Board Segmenti Grup Özeti

Board kodlarında ilk rakam baskın elektronik işlevi göstermelidir:

- `B1xx` → İşlemci / kontrol kartları
- `B2xx` → Ölçüm / dönüştürücü kartları
- `B3xx` → Giriş / arayüz kartları
- `B4xx` → Çıkış / sürücü kartları
- `B5xx` → Sensör arayüz / sensör kartları
- `B6xx` → Rezerve
- `B7xx` → Rezerve
- `B8xx` → Güç yönetimi / besleme kartları
- `B9xx` → Ana kart / backplane / bağlantı kartları

## Kullanım Notları

- Repo adı, kart kodunun kanonik formunu mümkün olduğunca korumalıdır.
- Grup kodu parça adına göre değil, baskın teknik işleve göre seçilmelidir.
- Rezerve alanlar (`B6xx`, `B7xx`) aktif ürün ailesi gibi kullanılmamalıdır.
- Platform eki gerekiyorsa kısa ve tutarlı kullanılmalıdır. Örnek: `-PCIe`.
- Bu dosya kısa organizasyon özeti içindir; detayların kaynağı web üzerindeki kanonik dokümandır.
