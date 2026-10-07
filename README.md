<div align="center">

# Banka Sırası Otomasyonu

**Öncelikli kuyruk simülasyonu**

![C#](https://img.shields.io/badge/C%23-2563eb?style=flat-square)
![Queue](https://img.shields.io/badge/Queue-0891b2?style=flat-square)
[![MIT License](https://img.shields.io/badge/License-MIT-16a34a?style=flat-square)](LICENSE)

Banka işlem sırasını üç öncelik grubu ve her grup içinde FIFO mantığıyla yöneten konsol simülasyonu.

</div>

---

## Öne Çıkanlar

- İsim ve öncelik ile müşteri kaydı
- Öncelik grupları arasında sıralı işlem
- Bekleyen müşteriler ve kuyruk durumunu görüntüleme

## Teknolojiler

C# · Queue

## Teknik yaklaşım

Müşteriler öncelik gruplarına ayrılır; gruplar arasında öncelik, grup içinde FIFO sırası uygulanır. Konsol menüsü kayıt ve hizmet akışını yönetir.

## Kodu incelemeye başlayın

- [Program.cs](Program.cs)

## Kapsam ve sınırlar

Gerçek banka entegrasyonu veya kalıcı işlem kaydı sunan bir sistem değil, kuyruk davranışı simülasyonudur.

<details>
<summary><strong>Kurulum, kullanım ve teknik ayrıntılar</strong></summary>

Bu proje, **C#** programlama dili kullanılarak geliştirilmiş bir konsol uygulamasıdır. Amaç, **Queue (Kuyruk)** veri yapısının çalışma mantığını gerçek hayattaki banka sırası sistemi üzerinden simüle etmektir. Sistem, müşterileri öncelik seviyelerine göre sıralayarak işlemleri **FIFO (First In First Out / İlk Giren İlk Çıkar)** mantığıyla yönetmektedir.

---

## Proje Hakkında

Uygulama, müşterileri üç farklı öncelik grubuna ayırarak işlem sırasını yönetir:

- **1. Öncelik:** VIP / Acil müşteriler
- **2. Öncelik:** Standart müşteriler
- **3. Öncelik:** Düşük öncelikli müşteriler

Sistem, öncelik seviyelerine göre otomatik işlem akışı sağlar:

1. Önce 1. öncelikli müşteriler işlenir.
2. 1. kuyruk boşaldığında 2. öncelikli müşterilere geçilir.
3. Tüm üst öncelikler tamamlandığında 3. öncelikli müşteriler işleme alınır.

Bu yapı sayesinde Queue veri yapısının mantığı pratik bir senaryo üzerinden anlaşılır hale getirilmiştir.

---

## Teknik Detaylar

| Özellik | Açıklama |
|---|---|
| Dil | C# |
| Platform | .NET Framework 4.7.2 |
| Veri Yapısı | `Queue<string>` |
| Uygulama Türü | Console Application |
| Programlama Yaklaşımı | Nesne Yönelimli Programlama (OOP) |

---

## Temel Özellikler

## Müşteri Kaydı
- Sisteme yeni müşteri ekleme
- İsim ve öncelik seviyesi belirleme
- Dinamik kuyruk yönetimi

## Akıllı İşlem Yönetimi
- Öncelikli müşteri mantığı
- FIFO tabanlı işlem sırası
- Kuyruklar arası otomatik geçiş

## Kuyruk Görüntüleme
- Tüm müşterileri öncelik sırasına göre listeleme
- Bekleyen müşteri kontrolü
- Anlık kuyruk durumu görüntüleme

---

## Kurulum ve Çalıştırma

## 1. Projeyi İndirin

```bash
git clone https://github.com/silanpehlivan/Banka-S-ras-.git
```

veya ZIP olarak indirip çıkarın.

---

## 2. Visual Studio ile Açın

`7.Odev.sln` dosyasını Visual Studio üzerinden açın.

---

## 3. Projeyi Çalıştırın

Visual Studio içerisinde:

```bash
F5
```

tuşuna basarak projeyi derleyip çalıştırabilirsiniz.

---

## Proje Yapısı

```bash
7.Odev/
│
├── Program.cs
├── 7.Odev.csproj
├── .gitignore
└── README.md
```

| Dosya | Açıklama |
|---|---|
| `Program.cs` | Kuyruk algoritması ve menü sistemi |
| `7.Odev.csproj` | Proje yapılandırma dosyası |
| `.gitignore` | Gereksiz Visual Studio dosyalarını filtreler |
| `README.md` | Proje tanıtım dosyası |

---

## Kullanılan Veri Yapısı

Bu projede temel olarak aşağıdaki veri yapısı kullanılmıştır:

```csharp
Queue<string>
```

Queue yapısı:
- İlk eklenen veriyi ilk çıkarır.
- FIFO mantığı ile çalışır.
- Gerçek hayattaki banka sırası sistemlerine uygundur.

---

## Projenin Amacı

Bu proje sayesinde:

- Queue veri yapısının çalışma mantığı öğrenilir.
- Öncelikli işlem sistemleri anlaşılır.
- Gerçek hayat senaryoları yazılıma aktarılır.
- C# konsol uygulaması geliştirme pratiği kazanılır.

---


</details>

---

<div align="center">

**© 2024 Şilan PEHLİVAN**

Bu proje MIT lisansı kapsamında sunulmaktadır. Kullanım ve dağıtım koşulları: [LICENSE](LICENSE).

</div>
