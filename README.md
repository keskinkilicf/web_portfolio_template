# gzhno // Krul_Tepes — Security Researcher Portfolio

Smart contract güvenlik araştırmacısı ve bug bounty hunter kişisel portfolyo sitesi.

## Hakkında

Solana ve EVM ekosistemlerinde DeFi protokol güvenliği üzerine çalışıyorum. **Code4rena** ve **Immunefi** platformlarında bug bounty araştırmaları yapıyorum. Aynı zamanda RISC-V mimarisi üzerinde safety-critical bir gerçek zamanlı işletim sistemi çekirdeği — **Sipahi** — geliştiriyorum.

## Site Yapısı — 7 Sayfa

```
web_portfolio_template/
├── index.html                    # Ana sayfa — Three.js 3D Sipahi logo, particle morphing
├── README.md                     # Bu dosya
├── assests/
│   ├── css/
│   │   └── style.css             # Global stiller
│   ├── js/
│   │   ├── main.js               # Temel scriptler
│   │   └── senior.js             # Ctrl+K Command Palette, GSAP ScrollTrigger, sayfa geçişleri
│   └── img/                      # Görseller
└── pages/
    ├── project.html              # Sipahi mimari (Three.js Exploded View, D3.js Force Graph)
    ├── rust.html                 # Rust tanıtımı (Canvas Ownership animasyonu, Ferris)
    ├── scenario.html             # Hava savunma simülasyonu (AI video + HUD overlay)
    ├── about.html                # Hakkımda (Krul Tepes hero, Three.js Skill Sphere)
    ├── contact.html              # İletişim formu + Three.js Rune Portal
    ├── defense.mp4               # AI-generated füze simülasyon videosu
    ├── ferris.png                # Rust maskotu Ferris görseli
    └── krul.png                  # Krul Tepes hero görseli
```

## Kullanılan Teknolojiler

| Teknoloji | Kullanım Alanı |
|-----------|---------------|
| **Three.js + GLSL** | 3D Sipahi logo (index), Rune Portal (contact), Skill Sphere (about), Exploded View (project) |
| **D3.js** | Force-directed modül bağımlılık grafiği (project) |
| **GSAP + ScrollTrigger** | Stagger animasyonlar, parallax, bounce efektleri (tüm sayfalar) |
| **Canvas 2D API** | Ownership animasyonu (rust), HUD simülasyonu (scenario) |
| **Video API** | AI-generated füze videosu arka plan (scenario) |
| **CSS Animations** | Keyframe animasyonlar, transitions, hover efektleri |
| **Google Fonts** | JetBrains Mono, Outfit, Cinzel |

## Sayfa Detayları

### index.html — Ana Sayfa
- **Three.js 3D Sipahi Logosu:** 4 katmanlı kernel mimarisi (oktahedron çekirdek, IPC torus halkaları, WASM halka, icosahedron kalkan), metalik material, 4 ışık kaynağı, mouse etkileşimi
- **Particle Morphing:** 500 parçacık dağınık küre ↔ "SİPAHİ" yazısı arasında morph döngüsü
- **Typing efekti:** Döngüsel metin animasyonu
- **Proje carousel:** 4 proje kartı, otomatik döngü + ok navigasyonu
- **Terminal animasyonu:** Gerçek zamanlı yazılan Sipahi kernel build çıktısı
- **Newsletter formu:** Validasyonlu e-posta abonelik

### pages/project.html — Projeler
- **Three.js Exploded View:** 4 katman geometri (Donanım, Çekirdek, IPC, WASM), slider ile ayır/birleştir, mouse ile döndür
- **D3.js Force Graph:** 19 düğüm, 22 bağlantı, sürüklenebilir fizik simülasyonu, 5 renk kategorisi
- **Sipahi Microkernel:** İnteraktif tab sistemi ile 4 katman detayı
- **National Cyber Stack:** 5 modüllü interaktif flow diagram (PRELUDE, ORACLE, MANTIS, ARES, OBSIDIAN)
- **Invariant kartları** ve doktrin bloğu

### pages/rust.html — Rust Programlama Dili
- **Ferris görseli:** Floating + glow animasyonu
- **Canvas Ownership Animasyonu:** 4 adımlı otomatik döngü (let → move → clone → drop), Stack/Heap kutuları, oklu bağlantılar
- **6 özellik kartı:** Bellek güvenliği, sıfır maliyetli soyutlama, korkusuz eşzamanlılık, Cargo, no_std, formal doğrulama
- **Dil karşılaştırma tablosu:** Rust vs C vs C++ vs Go vs Python, 7 metrik
- **Kimler kullanıyor:** Mozilla, AWS, Google, Microsoft, Linux Kernel, Solana
- **Tarihçe timeline:** 2006'dan Sipahi'ye

### pages/scenario.html — Hava Savunma Simülasyonu
- **AI-generated video arka plan:** Kling 2.6 ile üretilmiş füze savunma videosu
- **Askeri HUD overlay:** Scanlines, vignette, crosshair, köşe bilgileri, telemetri panelleri
- **Otomatik senaryo:** C++ RTOS fail (KERNEL PANIC) → Sipahi success — 1 kere oynuyor
- **Teknik karşılaştırma:** Rust vs C++ metrikleri, animasyonlu barlar
- **Savaş senaryosu timeline:** 5 adımlı balistik füze önleme zaman çizelgesi

### pages/about.html — Hakkımda
- **Full-screen Krul Tepes hero:** AI-generated görsel, kırmızı vignette, kan parçacıkları
- **"Gazihan ÖCBE // Krul_Tepes":** Cinzel font, gradient, animasyonlu unvanlar
- **Three.js Skill Sphere:** 28 yetenek, Fibonacci spiral dağılımı, 3D dönen küre, mouse ile döndür
- **Timeline:** Kırmızı→yeşil gradient, animasyonlu giriş
- **Skill barlar:** Kırmızı→yeşil gradient, scroll-triggered
- **17 araç, 6 kategoride interaktif filtre:** Formal Verification, Fuzzing, Observability, Testing, Security, Infra
- **Ticker:** Kayan metin bandı

### pages/contact.html — İletişim
- **Three.js Mystical Rune Portal:** GLSL shader enerji küresi, 3 dönen halka, 12 Elder Futhark rün sembolü, 150 spiral parçacık, dikey enerji ışınları, zemin ışık halkası
- **Gerçek zamanlı form validasyonu:** Blur tetiklemeli, karakter sayacı, konu dropdown
- **Loading spinner** ve toast bildirimi
- **İletişim kartları:** Hover animasyonlu

## Senior-Level Özellikler (senior.js)

- **Ctrl+K Command Palette:** Vercel/Linear tarzı arama paneli, fuzzy search, ok tuşları + Enter navigasyon, ESC kapatma
- **Sayfa Geçiş Animasyonu:** 6 yeşil bar aşağıdan yukarı, fade-in geçiş
- **GSAP ScrollTrigger:** Stagger grid animasyonları, section header parallax, badge bounce, timeline slide-in

## Sipahi Microkernel

Sipahi, robotik ve endüstriyel kontrol sistemleri için tasarlanan capability-based bir mikro çekirdek:

- **Katman 0 — Donanım:** RISC-V 64-bit, CLINT, PMP izolasyon, Watchdog Timer
- **Katman 1 — Çelik Çekirdek:** Heap-free, panic-free TCB. Preemptive RR scheduler, capability broker
- **Katman 2 — Sinir Sistemi:** Lock-free SPSC ring buffer ile zero-copy IPC, blackbox flight recorder
- **Katman 3 — Güvenli Bölge:** WASM sandbox (wasmi), no-float enforcement, cycle accounting
- **Formal Doğrulama:** Kani (panic-freedom) + Lean 4 (capability doğruluğu)

## National Cyber Stack

Sipahi üzerine inşa edilen 5 katmanlı sovereign siber savunma doktrini:

- **PRELUDE** — Early Sensing: ML bağımsız desen algılama
- **ORACLE** — Campaign Reasoning: Tekil olayları kampanya resmine dönüştürme
- **MANTIS** — Defensive Continuity: Graceful degradation, kademeli policy enforcement
- **ARES** — Counter-Pressure: M-of-N onaylı caydırıcılık
- **OBSIDIAN** — Evidence & Truth: Append-only, replay-safe kanıt zinciri

## Araç Kutusu (16 araç)

**Formal Verification:** Kani, Lean 4, TLA+, Miri, Loom
**Fuzzing & Mutation:** cargo-fuzz (libFuzzer), AFL++, cargo-mutants
**Observability:** eBPF + Flamegraph, RR (Record & Replay)
**Testing:** proptest/quickcheck, Insta, Criterion.rs, llvm-cov/grcov
**Security:** cargo-audit + cargo-deny, Clippy
**Infrastructure:** cross-rs

## Yerel Geliştirme

```bash
git clone https://github.com/KrulTepes40/web_portfolio_template.git
cd web_portfolio_template
# Tarayıcıda index.html'i aç
```

## İletişim

- **GitHub:** [KrulTepes40](https://github.com/KrulTepes40)
- **Code4rena:** @Krul_Tepes
- **Immunefi:** Krul_Tepes

## Lisans

MIT

---

> *"Kodu kırmadan önce doğrulama şarttır."* — gzhno // Krul_Tepes
