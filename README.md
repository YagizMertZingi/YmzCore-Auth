# YmzCore-Auth

`YMZCore` eklentisi için uzaktan lisans ve erişim yönetim dosyası (`licenses.json`).

## Kullanım
- `"mode": "open"`: `revoked` listesindeki kurulum kimlikleri (`YMZ-...`) hariç tüm kurulumlar çalışır. Kendi bilgisayarlarınıza erişimi kaybetmeden başlangıç için uygundur.
- `"mode": "allowlist"`: Yalnızca `allowed` listesinde olan (ve `revoked` içinde olmayan) kurulum kimlikleri çalışır.
- Bir kişinin erişimini kapatmak için `YMZ-...` kimliğini `allowed` listesinden silip `revoked` listesine ekleyin (`git commit && git push`).
- Eklenti her 15 dakikada bir güncellemeyi okur.
