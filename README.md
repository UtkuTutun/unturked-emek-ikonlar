# Untürked Emek — eşya ikonları

Unturned eşyalarının envanter ikonları, `<kimlik>.png` olarak.
Oyunun kendi modellerinden, oyunun kendi ikon kamerasıyla üretildi
(`ItemTool.captureIcon` ayarları birebir taklit edilerek).

Bu depo bir **yayın çıktısıdır**, kaynak değil. Üreten kod ve gerekçesi
ana depoda: `scripts/build-item-index.py` + Unity'deki
`Untürked Emek/Esya Ikonlari` menüsü.

Kullanım (sunucu tarafında `config.yaml → shop.iconBaseUrl`):

```
https://<hesap>.github.io/<depo>/{id}.png
```

`{id}` eşyanın kimliğiyle değişir — Eaglefire için `4.png`.

## Sunucu listesi görselleri

| Dosya | Boyut | Nerede |
|---|---|---|
| `icon.png` | 64×64 | lobi sayfasının sol üstü (`Config.txt → Browser.Icon`) |
| `tn.png` | 32×32 | sunucu listesi satırı (`Browser.Thumbnail`) |

Adları kısa, çünkü thumbnail adresi Steam oyun etiketlerinin içine giriyor
ve o dize 128 karakterle sınırlı.
