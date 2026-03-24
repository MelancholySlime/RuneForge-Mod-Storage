

<div align="center">

![RuneForge Mod-Storage Banner](https://raw.githubusercontent.com/MelancholySlime/RuneForge-Mod-Storage/main/banner.png)

#  RuneForge Mod Storage

[![Auto Scraper](https://github.com/MelancholySlime/RuneForge-Mod-Storage/actions/workflows/runeforge_scraper.yml/badge.svg)](https://github.com/MelancholySlime/RuneForge-Mod-Storage/actions/workflows/runeforge_scraper.yml)
[![Last Commit](https://img.shields.io/github/last-commit/MelancholySlime/RuneForge-Mod-Storage?color=7c3aed&label=Cập%20nhật%20lần%20cuối&logo=github)](https://github.com/MelancholySlime/RuneForge-Mod-Storage/commits/main)
[![Repo Size](https://img.shields.io/github/repo-size/MelancholySlime/RuneForge-Mod-Storage?color=db2777&label=Dung%20lượng%20kho&logo=databricks)](https://github.com/MelancholySlime/RuneForge-Mod-Storage)
[![Source](https://img.shields.io/badge/Nguồn-Runeforge.dev-f59e0b?logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyTDIgN2wxMCA1IDEwLTV6TTIgMTdsOCA0IDgtNE0yIDEybDggNCA4LTQiLz48L3N2Zz4=)](https://runeforge.dev)
[![League of Legends](https://img.shields.io/badge/Game-League%20of%20Legends-C89B3C?logo=riot-games)](https://leagueoflegends.com)

*Một kho lưu trữ tự động — thu gom, gìn giữ toàn bộ Mod từ [Runeforge.dev](https://runeforge.dev) mà không bỏ sót bất kỳ phiên bản nào.*

</div>
<div align="center">

🌐 **Language / Ngôn ngữ:** [🇬🇧 English](./README.md) · [🇻🇳 Tiếng Việt](./README.vi.md)

</div>



---

## 📖 Giới Thiệu

**RuneForge Mod-Storage** là hệ thống lưu trữ tự động chạy mỗi ngày lúc **7:00 sáng (UTC+7)** — âm thầm thu thập và bảo quản toàn bộ file `.fantome` được đăng trên [Runeforge.dev](https://runeforge.dev): skin tùy chỉnh, âm thanh, hiệu ứng VFX, màn loading và nhiều hơn nữa dành cho **League of Legends**.

Không một Mod nào bị lãng quên. Không một phiên bản nào bị bỏ lại phía sau.

---

## 📦 Cấu Trúc Kho Lưu Trữ

Các tệp được tổ chức theo hai cấp thư mục. Mỗi **RF_Storage** chứa tối đa ~990 thư mục **Part**, mỗi Part chứa tối đa ~990 thư mục mod. Khi một Part đầy, hệ thống tự động mở Part mới — tương tự với Storage.

```
📦 RuneForge-Mod-Storage/
├── 🗄️ RF_Storage1/
│   ├── 📁 Part1/
│   │   ├── 📂 Demon Yasuo LOLSKINARCHIVE/
│   │   │   └── demon-yasuo-lolskinarchive-v2.fantome
│   │   └── 📂 Spirit Blossom Yone Chroma VFX/
│   │       ├── spirit-blossom-yone-chroma-vfx_1.0.0.fantome
│   │       └── spirit-blossom-yone-chroma-vfx_1.1.0.fantome
│   └── 📁 Part2/ ...
├── 🗄️ RF_Storage2/ ...
└── 🗄️ RF_StorageN/ ...
```

> File có dung lượng **trên 50 MB** sẽ được tải lên thẳng [GitHub Releases](https://github.com/MelancholySlime/RuneForge-Mod-Storage/releases) thay vì commit thông thường.

---

## ⚙️ Cỗ Máy Hoạt Động Như Thế Nào?

```
Runeforge.dev ──────► Bot Cào Dữ Liệu ──────► GitHub Repository
 (2.800+ mods)          (7h sáng mỗi ngày)       (Kho lưu trữ này)
```

| Bước | Hành động |
|------|-----------|
| 🔍 **Quét** | Duyệt qua toàn bộ 2.800+ bài mod trên 120 trang |
| 📋 **Đối chiếu** | So sánh với lịch sử `_runeforge_scraped.json` đã lưu |
| ☁️ **Kiểm tra Cloud** | Tra cứu GitHub API — bỏ qua file đã có trên Cloud |
| 📥 **Tải xuống** | Hốt sạch toàn bộ artifacts của mọi phiên bản |
| 📤 **Đẩy lên** | Tự động push mỗi ~950 MB để an toàn với giới hạn GitHub |

---

## 📊 Thống Kê Kho Lưu Trữ

| Chỉ số | Giá trị |
|--------|---------|
| 🌐 Nguồn | [runeforge.dev](https://runeforge.dev) |
| 🎮 Tổng Mod được theo dõi | 2.800+ |
| 🗓️ Ngày tạo kho | 12 tháng 3, 2026 |
| 🔄 Tần suất cập nhật | Hàng ngày · 7:00 sáng UTC+7 |
| 💾 Dung lượng kho | ~34 GB và đang tăng |
| 🗄️ Parts tối đa mỗi Storage | 990 |
| 📦 Mods tối đa mỗi Part | 990 |
| 🚀 Tối đa mỗi lần push | 999 MB |

---

## 🔗 Liên Kết Liên Quan

| Liên kết | Mô tả |
|----------|-------|
| 🌐 [Runeforge.dev](https://runeforge.dev) | Nền tảng đăng tải mod gốc |
| 🛠️ [cslol-manager](https://github.com/LeagueToolkit/cslol-manager) | Tool để áp dụng file `.fantome` trong game |
| 📋 [Lịch sử chạy](https://github.com/MelancholySlime/RuneForge-Mod-Storage/actions) | Nhật ký hoạt động của bot |

---

## 💌 Lời Nhắn Đến Các Tác Giả Mod

Kho lưu trữ này được xây dựng với tất cả tình yêu và sự tôn trọng sâu sắc dành cho cộng đồng sáng tạo. Chúng tôi **không** có bất kỳ quyền sở hữu nào đối với các mod tại đây — toàn bộ công sức và vinh dự thuộc về những tác giả gốc trên Runeforge.

**Nếu bạn là tác giả và muốn gỡ bỏ tác phẩm của mình**, vui lòng mở một [Issue](https://github.com/MelancholySlime/RuneForge-Mod-Storage/issues) với tiêu đề `[Takedown Request]`. Yêu cầu của bạn sẽ được xử lý ngay lập tức và trân trọng. 🌷

---

## 🦊 Về Con Cáo Nhỏ

Kho lưu trữ này được một con cáo nhỏ âm thầm gìn giữ — chạy khắp internet nhặt nhạnh từng chiếc mod một, chạy được bằng cà phê và trái tim. 🦊


<div align="center">
  <sub>Được vận hành bởi 🦊 với ☕, 💖 · Tự động hóa bởi GitHub Actions · Không liên kết với Riot Games</sub>
</div>
