# Anti Lag V4 

🇬🇧 [English](#english) · 🇹🇷 [Türkçe](#türkçe)

---

## English

A Windows game-latency optimization tool written in **Rust** with an **egui** GUI.

This repository is shared **as a source-code example**: read it, learn from it, adapt it to your own projects. It is not a polished product.

### What's inside

- **Network:** ping monitor, MTU optimizer, Nagle / TCP ACK tweaks, QoS policies, packet manager
- **System:** process priority manager, RAM optimizer, system tweaks, service management
- **Game guard:** background thread that applies optimizations when a game is detected
- **Safety nets:** settings backup, reset, fixer, crash log
- **Extras:** VPN assistant

### Build

Requires Windows and the [Rust toolchain](https://rustup.rs).

```bash
cargo build --release
```

The binary ends up in `target/release/anti-lag.exe`. Run it as administrator, since registry and service changes need elevated rights.

###  Warning

This tool modifies the Windows registry, services and network settings. The backup module saves settings before changes, but **there is no guarantee**. Use at your own risk and create a system restore point first.


---

## Türkçe

**Rust** ile yazılmış, **egui** arayüzlü bir Windows oyun gecikmesi (lag) optimizasyon aracı.

Bu repo **örnek kaynak kod** olarak paylaşıldı: oku, öğren, kendi projene uyarla. Cilalı bir ürün değil.

### İçinde ne var

- **Ağ:** ping izleyici, MTU optimizasyonu, Nagle / TCP ACK ayarları, QoS politikaları, paket yöneticisi
- **Sistem:** işlem önceliği yöneticisi, RAM optimizasyonu, sistem ayarları, servis yönetimi
- **Game guard:** oyun algılandığında optimizasyonları otomatik uygulayan arka plan thread'i
- **Güvenlik ağları:** ayar yedekleme, sıfırlama, onarıcı, çökme kaydı
- **Ekstra:** VPN asistanı

### Derleme

Windows ve [Rust araç zinciri](https://rustup.rs) gerekir.

```bash
cargo build --release
```

Çıktı `target/release/anti-lag.exe` içinde olur. Registry ve servis değişiklikleri yönetici yetkisi istediği için yönetici olarak çalıştır.

###  Uyarı

Bu araç Windows registry'sini, servisleri ve ağ ayarlarını değiştirir. Yedekleme modülü değişiklikten önce ayarları kaydeder ama **garanti yoktur**. Kendi sorumluluğunda kullan ve önce bir sistem geri yükleme noktası oluştur.




