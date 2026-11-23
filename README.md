<div align="center">

<img src="docs/01-kapak.png" alt="EventHub — Apollo Client — Enes Öztürk imzalı proje" width="100%">

# EventHub — Apollo Client

**Ödev 4 — Apollo Client, yerel GraphQL şeması, InMemoryCache ve canlı sorgu konsolu ile etkinlik portalı.**

[![Apollo](https://img.shields.io/badge/Apollo-58BDF8?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnesBinMalik/eventhub-apollo)
[![GraphQL](https://img.shields.io/badge/GraphQL-58BDF8?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnesBinMalik/eventhub-apollo)
[![React](https://img.shields.io/badge/React-58BDF8?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnesBinMalik/eventhub-apollo)
[![TypeScript](https://img.shields.io/badge/TypeScript-58BDF8?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnesBinMalik/eventhub-apollo)
[![Doğrulama](https://img.shields.io/badge/Do%C4%9Frulama-lint%20%2B%20build%20ge%C3%A7ti-2EA043?style=for-the-badge)](https://github.com/EnesBinMalik/eventhub-apollo)
[![Enes Öztürk](https://img.shields.io/badge/Enes%20%C3%96zt%C3%BCrk-imzal%C4%B1-EA4338?style=for-the-badge&logo=badge&logoColor=white)](https://github.com/EnesBinMalik)

<img src="docs/rozet-enes-ozturk.png" alt="Enes Öztürk imzalı tasarım rozeti" width="420">

</div>

---

## Hakkında

EventHub, Apollo Client'ı yerel bir GraphQL şemasına bağlayarak gerçek bir istemci tarafı veri katmanı kurar. Tüm sorgular 120 ms gecikmeyle simüle edilir, sonuçlar Apollo Cache'te tutulur ve yerleşik konsol her isteği kayıt altına alır. Harici backend gerektirmez.

> Bu proje **Enes Öztürk** tarafından tasarlanmış, geliştirilmiş ve imzalanmıştır.

---

## Öne çıkan özellikler

| Özellik | Açıklama |
| --- | --- |
| **Apollo Client** | ApolloLink + InMemoryCache ile tam entegrasyon. |
| **Yerel şema** | Tarayıcı içinde çalışan GraphQL çözümleyici. |
| **Sorgu konsolu** | İstek, süre, durum ve yanıt önizlemesi. |
| **120 ms gecikme** | Gerçek ağ davranışını taklit eden simülasyon. |
| **Etkinlik akışı** | Detay modalı, oluşturma formu ve cache güncellemesi. |
| **Ödev 4 raporu** | Apollo entegrasyonunun teknik dokümantasyonu. |

---

## Mimari

| Ölçü | Değer |
| --- | --- |
| İstemci | Apollo |
| Şema | Yerel |
| Cache | Normalize |
| Gecikme | 120 ms |

---

## Galeri

<img src="docs/02-ekran.png" alt="EventHub — Apollo Client ana ekran" width="100%">

<img src="docs/03-ekran.png" alt="EventHub — Apollo Client etkileşimli görünüm" width="100%">

<img src="docs/04-ekran.png" alt="EventHub — Apollo Client detay görünümü" width="100%">

---

## Kurulum

**Gereksinim:** Node.js 20+

```bash
git clone https://github.com/EnesBinMalik/eventhub-apollo.git
cd eventhub-apollo
npm install
npm run dev
```

> Apollo Client'ın peer bağımlılığı olan rxjs package.json içinde tanımlıdır.

Diğer komutlar:

```bash
npm run build     # Üretim derlemesi
npm run preview   # Derlemeyi önizle
npm run lint      # TypeScript tip kontrolü
```

---

## Teknik mimari

```text
src/graphql/client.ts      ApolloLink + InMemoryCache
src/graphql/schema.ts       Yerel şema ve çözümleyiciler
src/graphql/queries.ts      GraphQL sorguları
src/components/GraphQLConsoleModal.tsx  İstek konsolu
src/components/EventList.tsx  Etkinlik listesi
```

---

## İmza

<div align="center">

[![Geliştirici](https://img.shields.io/badge/Geli%C5%9Ftirici-Enes%20%C3%96zt%C3%BCrk-EA4338?style=for-the-badge&logo=github&logoColor=white)](https://github.com/EnesBinMalik)
[![İmza](https://img.shields.io/badge/%C4%B0mza-Enes%20%C3%96zt%C3%BCrk-FFD700?style=for-the-badge&logo=verified&logoColor=white)](https://github.com/EnesBinMalik)

**Bu kod, tasarım ve deneyim Enes Öztürk'ün kişisel imzasını taşır.**

© 2026 Enes Öztürk — Tüm hakları saklıdır.

</div>
