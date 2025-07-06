# AdGuardHome-Whitelist

Kendi AdGuard Home sunucum için oluşturduğum blacklist ve whitelist listeleri ile yapılandırma bilgilerini içeren bir depo.

## Kullanılan Başlıca Blacklist Kaynakları

Reklamları, kötü amaçlı yazılımları ve izleyicileri engellemek için kullanılan başlıca blacklist kaynakları:

- https://adguardteam.github.io/HostlistsRegistry/assets/filter_1.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_2.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_59.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_34.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_26.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_40.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_30.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_8.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_10.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_42.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_31.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_9.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_11.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_55.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_44.txt
- https://adguardteam.github.io/HostlistsRegistry/assets/filter_50.txt
- https://raw.githubusercontent.com/mertcangokgoz/AdGuardHome-Whitelist/refs/heads/main/blocklist.txt
- https://raw.githubusercontent.com/mertcangokgoz/usom-mirror/refs/heads/main/usom_adguard_blacklist.txt

## Kullanılan Başlıca Whitelist Kaynakları

Hatalı siteleri ve reklamları engelleyen blacklist kaynaklarından etkilenen siteleri beyaz listeye almak için kullanılan başlıca whitelist kaynakları:

- https://adguardteam.github.io/HostlistsRegistry/assets/filter_45.txt
- https://raw.githubusercontent.com/mertcangokgoz/AdGuardHome-Whitelist/refs/heads/main/whitelist.txt


## Dinlenen IP ve Portlar

AdGuard Home sunucum şu IP ve portlarda dinlemektedir:

- 194.5.236.109
- https://dns.gokgoz.net/dns-query
- tls://dns.gokgoz.net:853
- quic://dns.gokgoz.net:853

## Yapılandırma Ayarları

- Günlük yapılandırması 
  - [x] Günlüğü etkinleştir
  - [x] İstemcinin IP adresini gizle
  - [x] Sorgu günlükleri rotasyonu 24 saat

- İstatistikleri sakla
    - [x] İstatistikleri etkinleştir
    - [x] İstatistikleri saklama süresi 90 gün

- Şifreleme ayarları
    - [x] DNS over HTTPS (DoH) etkinleştir
    - [x] DNS over TLS (DoT) etkinleştir
    - [x] DNS over QUIC etkinleştir

- DNS ayarları
    - [x] DNSSEC etkinleştir
    - [x] DNS over HTTPS (DoH) için TLS sertifikası doğrulamasını etkinleştir
    - [x] DNS over TLS (DoT) için TLS sertifikası doğrulamasını etkinleştir
    - [x] DNS over QUIC için TLS sertifikası doğrulamasını etkinleştir

- Kullanılan Üst DNS Sunucuları

```
1.1.1.1
1.0.0.1
9.9.9.9
149.112.112.112
94.140.14.140
94.140.14.141
8.8.8.8
8.8.4.4
```

- Kullanılan Yedek DNS Sunucuları

```
208.67.222.222
208.67.220.220
76.76.2.0
76.76.10.0
```

- Rate Limit: 20
- Maksimum DNS Sorgu Boyutu: 4096 bayt
- IPv4 adresleri için alt ağ önek uzunluğu: 24
- IPv6 adresleri için alt ağ önek uzunluğu: 56
- EDNS istemci alt ağı etkin
- Engelleme modu: `NXDOMAIN: NXDOMAIN koduyla yanıt ver`

## LICENSE

Bu proje MIT lisansı altında lisanslanmıştır. Lütfen [LICENSE](LICENSE) dosyasını inceleyin.