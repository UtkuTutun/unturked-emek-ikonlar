# Untürked Emek — eşya ikonları

Unturned eşyalarının envanter ikonları, `<kimlik>.png` olarak (256×256,
kare tuval). Oyunun KENDİ ikon aracıyla çekildi (ana menü → Workshop → F1 →
All Item Icons): varsayılan parçalar (dürbün, şarjör) takılı, oyundaki gibi.

`kf/<kimlik>.png` ve `kfs/<kimlik>.png`: ölüm akışının silah görselleri
(yükseklik 32, renkli ve beyaz siluet).

Bu depo bir **yayın çıktısıdır**, kaynak değil. Üreten kod ve gerekçesi
ana depoda: `scripts/icons/import-game-icons.py` + `scripts/icons/square-icons.py`.

Kullanım (sunucu tarafında `config.yaml → shop.iconBaseUrl`):

```
https://<hesap>.github.io/<depo>/{id}.png
```

`{id}` eşyanın kimliğiyle değişir — Eaglefire için `4.png`.

## Sunucu listesi görselleri

| Dosya | Boyut | Nerede |
|---|---|---|
| `icon.png` | 64×64 | ağ logosu, lobi sayfasının sol üstü (`Config.txt → Browser.Icon`) |
| `tn.png` | 32×32 | ağ logosu, sunucu listesi satırı (`Browser.Thumbnail`) |
| `icon-m.png`, `tn-m.png` | 64×64, 32×32 | Market (mavi) |
| `icon-k.png`, `tn-k.png` | 64×64, 32×32 | Klasik (yeşil) |
| `ui/<ad>.png` | 64×64 | sohbet mesajlarının başındaki simge (`messages.icons`) |

Adları kısa, çünkü thumbnail adresi Steam oyun etiketlerinin içine giriyor
ve o dize 128 karakterle sınırlı.
