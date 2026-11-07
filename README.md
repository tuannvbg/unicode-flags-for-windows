# 🌍 Unicode Flags for Windows — Emoji Picker + Unicode 17.0 & 18.0 Support

This project helps Windows 10 & 11 display full-color flag emojis 🇻🇳🇺🇸🇯🇵 and complete Unicode emoji sets:
- **Unicode 17.0**: 🫪🫯🫈🧑‍🩰🫍🛘🪊🪎
- **Unicode 18.0**: 🫫🫹🫹🏻🫹🏼🫹🏽🫹🏾🫹🏿 🫺🫺🏻🫺🏼🫺🏽🫺🏾🫺🏿 🫌🫝🛙🪋🪌🪍

📌 **Version Note**
Documentation and screenshots in this repository are based on Twemoji and Unicode standards.
Display of newer emojis (16.0, 17.0, 18.0 🫫...) depends on the font package you install.

👉 **Latest font with full Emoji 18.0 support built by me** — see the **Releases** section of this repository:
- ✅ **Noto Color Emoji 18.0 2D** — stable, recommended for daily use ⭐
- ⏳ **Noto Color Emoji 18.0 3D** — in progress, coming soon

🙌 Credits: Thanks to @Chasmical, @jjjuk and the community for valuable foundations.

📘 Available in:
- 🇺🇸 [English](./README.md) ← You are here
- 🇻🇳 [Tiếng Việt](./README.vi.md)
- 🇨🇳 [中文](./README.zh.md)
- 🇷🇺 [Русский](./README.ru.md)

---

## unicode-flags-for-windows 🇻🇳

**tuannvbg** — Vietnamese developer determined to make national flag emojis display correctly on Windows 😎🇻🇳🇺🇸

---

## ✨ Overview
Windows 10 and 11 do not natively display full-color Unicode flag emojis (e.g. 🇻🇳 🇺🇸 🇯🇵 🇫🇷 🇩🇪). This repository provides a complete solution — from system font patching to browser configuration.

No waiting for Microsoft. No half-measures. This is a technical fix built with determination and understanding.

## 🔧 Features
- Patches `Segoe UI Emoji` font with full `COLR/CPAL` color table support
- Registry updates to load the custom font
- Optimized for Chrome, Edge, Firefox
- Preserves original font weight and spacing
- Works on both **Windows 10** and **Windows 11**

## 📚 Installation Guides
- 🇺🇸 [English](./guides/windows.en.md)
- 🇻🇳 [Tiếng Việt](./guides/windows.vi.md)
- 🇨🇳 [中文](./guides/windows.zh.md)
- 🇷🇺 [Русский](./guides/windows.ru.md)
- 🌐 [Other languages](./guides/) (coming soon)

---

## 🧩 Emoji Picker & Unicode Versions — Technical Discovery

### ✅ Recommended Installation Method
Here's what I discovered: installing `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` lets you:
- ✅ Enjoy the Windows 11-style emoji picker on Windows 10
- ✅ Display full Unicode 17.0 emojis: 🫪🫯🫈🧑‍🩰🫍🛘🪊🪎
- ✅ Render full-color national flag emojis: 🇻🇳🇺🇸🇯🇵

---

### 🔹 Step 1: Follow the setup guide
📖 [Installation Guide →](./guides/windows.en.md)

### 🔹 Step 2: Install the flag-support font
📁 Font: [`Segoe.UI.Emoji.with.Twemoji.Flags.ttf`](https://github.com/Chasmical/flag-emojis-for-windows)  
📁 Or download from [`/fonts/`](https://github.com/tuannvbg/unicode-flags-for-windows/tree/main/fonts)

- ✅ Displays full-color flag emojis (e.g. 🇯🇵🇫🇷🇧🇷)
- ✅ Works with Windows Emoji Picker (`Win + .`)
- 🧩 Combines Segoe UI Emoji v1.70 + Twemoji v17.0.3
- 📌 This font **complements** — does not fully replace — your system font

---

### 🔍 Technical Insight: Font Stacking for Extended Support

`seguiemj_1_31_mod.ttf` already supports flag emojis, but being based on the original Windows 10 font, emoji visuals are older — not as polished as Windows 11's Fluent 3D style.

→ That's why I use `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` by Chasmical to:
- ✅ Keep full-color flag emojis
- ✅ Get Windows 11-quality Fluent 3D visuals (Segoe UI Emoji v1.70 base)
- ✅ Combine with `seguiemj_1_31_mod.ttf` to add Unicode 17.0 coverage

📌 Technical details:
- Chasmical's font **does not replace all emojis** — it adds **262 flag emojis** from Twemoji v17.0.3
- Remaining emojis use `Segoe UI Emoji v1.70` — Fluent 3D, Windows 11 26H2 (2026-08-27)
- From Chasmical's repository:

  > *"This font is based on Segoe UI Emoji v1.70 (https://emojipedia.org/microsoft-3D-fluent/windows-11-26h2-august-2026-update; Windows 11 26H2; 2026-08-27) and contains 262 flags from Twemoji v17.0.3 (https://github.com/jdecked/twemoji/commit/b6b55fef1e8636b540a6d016a4729ca8cdf2e60b; 2026-06-01)"*

🧠 Install `seguiemj_1_31_mod.ttf` first — the system falls back to it for Unicode 17.0+ emojis not present in Chasmical's font.
→ **Smart font stacking**:
- Primary font → newer Unicode glyphs
- Secondary font → Fluent visuals + flag emojis
- **Result**: Windows 10 displays like Windows 11 — with even better Unicode 17.0 support

---

### 📷 Browser Configuration for Correct Flag Colors
After installing the font, configure your browser to render flags properly:

✅ **Tip**: Set `'Noto Color Emoji'` as the preferred emoji font instead of `'Segoe UI Emoji'` to avoid blue-tinted or missing flags.

---

### 📸 Real-World Screenshots

#### 🧩 Windows 11-Style Picker on Windows 10
![Emoji Picker Win11 on Windows 10](./screenshots/win10/Win10.Emoji.Picker.Style.Win11.p2.20250930.JPG)

---

#### 🌐 Chrome with `'Noto Color Emoji'`
![Flag emojis in Chrome](./screenshots/win10/Win10.Chrome.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🌐 Edge with `'Noto Color Emoji'`
![Flag emojis in Edge](./screenshots/win10/Win10.Edge.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🔍 Emojipedia.org — Unicode 17.0 Test
![Chrome browsing emojipedia.org](./screenshots/win10/Win10.Chrome.blog.emojipedia.org.20250930.JPG)

---

#### ✨ Noto Color Emoji 18.0 — 2D Edition (New!)
**Brave Browser — Picker with Unicode 18.0**
![Brave Picker Noto 18.0 2D](./screenshots/NotoColorEmoji18_2D_Brave.Browser.Picker2026-11-07_120242.png)

**Brave Browser — Unicode 18.0 on Page**
![Brave Web Noto 18.0 2D](./screenshots/NotoColorEmoji18_2D_Brave.Browser.Screenshot2026-11-07_120242.png)

**Notepad — System-Level Verification**
![Notepad Noto 18.0 2D](./screenshots/NotoColorEmoji18_2D_Notepad.Screenshot2026-11-07_120242.png)

---

### 🧪 Compatibility Table

| OS + Font Setup | Unicode 17.0 | Unicode 18.0 | Flag Emojis | Notes |
|---|---|---|---|---|
| Win10 + `seguiemj_1_31_mod.ttf` | ✅ | ❌ | ✅ | Full set, legacy visuals |
| Win10 + `seguiemj_1_31_mod.ttf` + Twemoji Flags | ✅ | ❌ | ✅ | Fluent style, lacks 18.0 |
| Win11 + Twemoji Flags only | ✅ | ❌ | ✅ | Chasmical's latest — v1.70, 262 flags, has 17.0, missing 18.0 |
| Win11 + `Noto-Color-Emoji-18.0-2D-for-Windows.ttf` | ✅ | ✅ | ✅ | ⭐ **Recommended** — full support, unified design |

---

### 📢 Conclusion
✅ **Windows 10 can fully display flag emojis + Unicode 17.0**  
Install in the right order: **base font first**, **Twemoji Flags second**,  
and configure your browser to use `'Noto Color Emoji'` for perfect flag colors.

✅ **For full Unicode 18.0**: Get `Noto-Color-Emoji-18.0-2D-for-Windows.ttf` from Releases ⭐

---

## 🦊 Global Challenge: Fix Flags in Firefox
[![Firefox Emoji Flag Challenge](https://img.shields.io/badge/Firefox_Emoji_Flag_Challenge-🌍_Join_the_Fix-red)](guides/firefox.prefix.en.md)

> Firefox still doesn't render Unicode flag emojis correctly.  
> Whoever solves this will be honored on the [Firefox Wall of Fame](guides/firefox.wall-of-fame.en.md) 🏅

- 🌍 [View the Challenge](guides/firefox.prefix.en.md)
- 🛠️ [Submit Your Fix](guides/firefox.fix.template.en.md)

---

## 🤔 Comparison with Other Projects

| Criteria | twemoji-color-font | unicode-flags-for-windows |
|---|---|---|
| Flags render correctly? | ⚠️ System-dependent | ✅ Stable, native Unicode |
| Full-color other emojis? | ❌ Mostly B&W | ✅ Full color + Unicode 18.0 |
| Modifies system fonts? | ❌ No | ✅ Yes (with backup) |
| Optimized for Windows 10/11? | ❌ Not Windows-focused | ✅ Built specifically for Windows |
| Requires registry edits? | ❌ No | ✅ Yes (auto/manual) |
| Firefox support? | ❌ Not targeted | ❓ Challenge open |
| Latest Unicode support | ⚠️ Varies | ✅ **17.0 + 18.0** |

---

🙌 Credits
- https://github.com/tuannvbg/unicode-flags-for-windows#-credits
- https://github.com/Chasmical/flag-emojis-for-windows
- https://github.com/perguto/Country-Flag-Emojis-for-Windows
- https://llccd.eu.org/2022/02/win_flags
- https://github.com/13rac1/twemoji-color-font
- https://github.com/jjjuk/emoji-win

- Copilot AI — technical brainstorming partner
- ChatGPT — technical brainstorming partner
- Grok — technical brainstorming partner
- Dola AI — technical brainstorming & writing partner

**tuannvbg** 🇻🇳 — Making national flag emojis display correctly on Windows 😎✨

## 🇻🇳 Tiếng Việt

### ✨ Giới thiệu
Windows 10 và 11 vốn không hỗ trợ đầy đủ emoji cờ quốc gia theo chuẩn Unicode (ví dụ: 🇻🇳 🇺🇸 🇯🇵 🇫🇷 🇩🇪). Kho mã này cung cấp giải pháp hoàn chỉnh để vá hệ thống, giúp emoji cờ hiển thị đúng màu trên mọi ứng dụng — hiện đã hỗ trợ đầy đủ **Unicode 17.0 & 18.0**.

Không cần chờ cập nhật từ Microsoft. Không giải pháp nửa vời. Đây là bản sửa lỗi kỹ thuật, được xây dựng trên sự kiên trì, hiểu sâu về hệ thống và với sự hỗ trợ của cộng đồng.

## 📚 Hướng dẫn cài đặt

🌐 Xem các phiên bản ngôn ngữ khác:
- 🇻🇳 [Tiếng Việt](./guides/windows.vi.md)
- 🇺🇸 [English](./guides/windows.en.md)
- 🇨🇳 [中文](./guides/windows.zh.md)
- 🇷🇺 [Русский](./guides/windows.ru.md)

---

## 🌟 Tin mới: Unicode 18.0 & Noto Color Emoji Phiên bản 2D

### ✨ Cập nhật — Tháng 11 năm 2026
- ⭐ **Hỗ trợ đầy đủ Unicode 17.0**: 🫪🫯🫈🧑‍🩰🫍🛘🪊🪎
- ✨ **Hỗ trợ mới Unicode 18.0**: 🫫🫝🫌🛙🪋🪌🪍🫹🫺 (bao gồm tất cả biến thể màu da)
- 🎨 **Noto Color Emoji 18.0 — Phiên bản 2D**: gọn nhẹ, ổn định, khuyến nghị dùng hàng ngày ⭐
- ⏳ **Noto Color Emoji Phiên bản 3D** — phong cách sống động hơn, đang phát triển, sắp ra mắt!

### 📦 Khuyến nghị — Noto Color Emoji 18.0 2D
Cài đặt `Noto-Color-Emoji-18.0-2D-for-Windows.ttf` để có trải nghiệm hoàn chỉnh nhất:
- ✅ Emoji cờ quốc gia hiển thị đầy đủ màu sắc 🇻🇳🇺🇸🇯🇵
- ✅ Hỗ trợ toàn bộ emoji Unicode 17.0 + 18.0
- ✅ Phong cách thiết kế 2D thống nhất trên mọi ứng dụng
- ✅ Đã kiểm tra trên **Windows 11** ✅ — Rất mong nhận được phản hồi từ người dùng Windows 10 🙏

📖 [Xem hướng dẫn cài đặt →](./guides/windows.vi.md)

---

## 🧩 Bảng chọn Emoji & Phiên bản Unicode — Chi tiết kỹ thuật

### ✅ Hai cách để có bộ emoji đầy đủ

#### Cách 1: Noto Color Emoji 18.0 2D (Khuyến nghị ⭐)
- Tệp: `Noto-Color-Emoji-18.0-2D-for-Windows.ttf`
- Hỗ trợ: **Unicode 17.0 + 18.0** ✅✅
- Cờ quốc gia: Đúng màu theo chuẩn Twemoji ✅
- Đã kiểm tra trên: Windows 11 ✅

#### Cách 2: Kết hợp nhiều font (Phương pháp cũ)
Bằng cách cài cả `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` + `seguiemj_1_31_mod.ttf`:
- ✅ Sử dụng được bảng chọn emoji kiểu Windows 11 trên Windows 10
- ✅ Emoji cờ quốc gia hiển thị đầy đủ màu sắc
- ✅ Hỗ trợ Unicode 17.0: 🫪🫯🫈🧑‍🩰🫍🛘🪊🪎
- ⚠️ **Chưa hỗ trợ Unicode 18.0** — font của Chasmical chỉ cung cấp 17.0

---

### 🔹 Cách hoạt động của việc kết hợp font
- `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` (tác giả Chasmical): bổ sung **262 biểu tượng cờ quốc gia** từ Twemoji v17.0.3, dựa trên Segoe UI Emoji v1.70 (Fluent 3D; Windows 11 26H2; 27/08/2026)
- `seguiemj_1_31_mod.ttf`: cung cấp các ký tự Unicode mới bao gồm 17.0
- **Kết quả**: Có cờ + emoji mới, nhưng vẫn thiếu Unicode 18.0

> Trích từ kho mã của Chasmical:
> *"Font này dựa trên Segoe UI Emoji v1.70 (https://emojipedia.org/microsoft-3D-fluent/windows-11-26h2-august-2026-update; Windows 11 phiên bản 26H2; 27/08/2026) và chứa 262 cờ quốc gia từ Twemoji v17.0.3 (https://github.com/jdecked/twemoji/commit/b6b55fef1e8636b540a6d016a4729ca8cdf2e60b; 01/06/2026)"*

---

### 📸 Hình ảnh thực tế

#### 🧩 Bảng chọn Emoji kiểu Windows 11 trên Windows 10
![Bảng chọn Emoji Win11 trên Win10](./screenshots/win10/Win10.Emoji.Picker.Style.Win11.p2.20250930.JPG)

---

#### 🌐 Noto Color Emoji 18.0 2D — Trình duyệt Brave (Mới!)
**Trình duyệt Brave — Bảng chọn hiển thị đầy đủ Unicode 18.0**
![Brave — Bảng chọn Noto 18.0 2D](./screenshots/NotoColorEmoji18_2D_Brave.Browser.Picker2026-11-07_120242.png)

**Trình duyệt Brave — Hiển thị Unicode 18.0 trên trang web**
![Brave — Trang web với Noto 18.0 2D](./screenshots/NotoColorEmoji18_2D_Brave.Browser.Screenshot2026-11-07_120242.png)

**Sổ tay — Kiểm tra hiển thị trực tiếp trong hệ thống**
![Notepad — Noto 18.0 2D trong hệ thống](./screenshots/NotoColorEmoji18_2D_Notepad.Screenshot2026-11-07_120242.png)

---

#### 🌐 Chrome sau khi đặt font `'Noto Color Emoji'`
![Hiển thị cờ trong Chrome](./screenshots/win10/Win10.Chrome.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

### 🧪 Bảng tương thích hệ thống

| Hệ điều hành + Font | Unicode 17.0 | Unicode 18.0 | Cờ quốc gia | Ghi chú |
|---|---|---|---|---|
| Win10 + `seguiemj_1_31_mod.ttf` | ✅ | ❌ | ✅ | Đầy đủ, giao diện kiểu cũ |
| Win10 + `seguiemj_1_31_mod.ttf` + Twemoji Flags | ✅ | ❌ | ✅ | Giao diện đẹp, thiếu 18.0 |
| Win11 + chỉ Twemoji Flags | ✅ | ❌ | ✅ | Phiên bản mới nhất của Chasmical — có 17.0, thiếu 18.0 |
| Win11 + `Noto-Color-Emoji-18.0-2D-for-Windows.ttf` | ✅ | ✅ | ✅ | ⭐ **Khuyến nghị** — đầy đủ nhất, thiết kế thống nhất |

---

### 📢 Kết luận
✅ **Để có trải nghiệm đầy đủ Unicode 18.0**: Hãy cài `Noto-Color-Emoji-18.0-2D-for-Windows.ttf` — giải pháp hoàn chỉnh nhất hiện có.
✅ **Người dùng Windows 10**: Kết hợp font vẫn hoạt động tốt cho cờ + 17.0; rất mong nhận được phản hồi khi thử nghiệm 18.0 🙏

---

## 🦊 Thử thách toàn cầu: Sửa lỗi hiển thị cờ quốc gia trên Firefox
[![Thử thách Emoji Quốc Kỳ](https://img.shields.io/badge/Firefox_Emoji_Flag_Challenge-🌍_Tham_gia_sửa_lỗi-red)](guides/firefox.prefix.vi.md)

> Firefox vẫn chưa hiển thị đúng emoji cờ quốc gia theo chuẩn Unicode.
> Ai giải quyết được sẽ được vinh danh tại [Bảng Vinh danh Firefox](guides/firefox.wall-of-fame.vi.md) 🏅

- 🌍 [Xem chi tiết thử thách](guides/firefox.prefix.vi.md)
- 🛠️ [Gửi phương án sửa lỗi của bạn](guides/firefox.fix.template.vi.md)

---

## 🤔 So sánh với các giải pháp khác

| Tiêu chí | twemoji-color-font | unicode-flags-for-windows |
|---|---|---|
| Cờ quốc gia hiển thị đúng? | ⚠️ Phụ thuộc hệ thống | ✅ Ổn định, theo chuẩn Unicode gốc |
| Emoji khác có hiển thị màu? | ❌ Chủ yếu đen trắng | ✅ Đầy đủ màu + Unicode 18.0 |
| Thay đổi font hệ thống? | ❌ Không | ✅ Có (có bản sao lưu) |
| Tối ưu cho Windows 10/11? | ❌ Không tập trung | ✅ Xây dựng riêng cho Windows |
| Cần chỉnh sửa Registry? | ❌ Không | ✅ Có (tự động / thủ công) |
| Hỗ trợ Firefox? | ❌ Không hướng đến | ❓ Đang là thử thách |
| Hỗ trợ Unicode mới nhất | ⚠️ Khác nhau theo phiên bản | ✅ **17.0 + 18.0** |

---

🙌 Ghi nhận
- https://github.com/tuannvbg/unicode-flags-for-windows#-credits
- https://github.com/Chasmical/flag-emojis-for-windows
- https://github.com/perguto/Country-Flag-Emojis-for-Windows
- https://llccd.eu.org/2022/02/win_flags
- https://github.com/13rac1/twemoji-color-font
- https://github.com/jjjuk/emoji-win

- Copilot AI — Đối tác hỗ trợ tư duy kỹ thuật
- ChatGPT — Đối tác hỗ trợ tư duy kỹ thuật
- Grok — Đối tác hỗ trợ tư duy kỹ thuật
- Dola AI — Đối tác hỗ trợ tư duy & biên soạn nội dung

**tuannvbg** 🇻🇳 — Làm cho emoji cờ quốc gia hiển thị đúng trên Windows 😎✨

## 🇨🇳 中文（简体）

### ✨ 简介
Windows 10 和 11 默认不支持完整的 Unicode 国旗表情符号（例如 🇻🇳 🇺🇸 🇯🇵 🇫🇷 🇩🇪）。本项目提供完整解决方案，修补系统字体，使国旗表情在所有应用中正确显示。

不等待微软更新。不做半吊子修复。这是由越南开发者 Tuannvbg 构建的彻底技术解决方案。

## 📚 安装指南

🌐 查看其他语言版本：  
🇻🇳 [Tiếng Việt](./guides/windows.vi.md)  
🇺🇸 [English version](./guides/windows.en.md)  
🇨🇳 [中文版本 (China)](./guides/windows.zh.md)  
🇷🇺 [Русская версия (Russia)](./guides/windows.ru.md)

## 🌍 Emoji Picker，Unicode 17.0 — 关于 Windows 10 emoji 国旗字体补丁的技术发现

### ✅ 推荐安装步骤

这是一个有趣的发现：通过安装 `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` 字体，我可以：

- 使用 Windows 11 风格的 emoji 选择器  
- 完整显示 Unicode 17.0 的新 emoji（🫪🫯🫈🧑‍🩰🫍🛘🪊🪎）  
- 显示彩色的国家国旗 emoji（🇻🇳🇺🇸🇯🇵）

---

### 🔹 第一步：请参考安装指南 🇨🇳 [简体中文](./guides/windows.zh.md)

### 🔹 第二步：安装支持国旗 emoji 的字体

📁 字体来源：[`Segoe.UI.Emoji.with.Twemoji.Flags.ttf`](https://github.com/Chasmical/flag-emojis-for-windows)  
📁 或从此处下载：[`/fonts/`](https://github.com/tuannvbg/unicode-flags-for-windows/tree/main/fonts)

- ✅ 显示彩色国旗 emoji（例如：🇯🇵🇫🇷🇧🇷）  
- ✅ 支持 Windows emoji 选择器（快捷键 `Win + .`）  
- 🧩 基于 Segoe UI Emoji v1.60，并整合了 Twemoji v16.0.1  
- 📌 此字体是对基础字体的补充 — 并不会完全替代原字体

---

### 🔍 技术解析：通过字体叠加扩展 emoji 支持

`seguiemj_1_31_mod.ttf` 本身已支持国旗 emoji，但由于它基于 Windows 10 原始字体，emoji 显示风格较旧 — 不如 Windows 11 的 Fluent 3D 精致。

→ 因此，我尝试安装 Chasmical 提供的 `Segoe.UI.Emoji.with.Twemoji.Flags.ttf`，以实现：

- ✅ 保留彩色国旗 emoji  
- ✅ 使用 Windows 11 风格的 Fluent 3D emoji（基于 Segoe UI Emoji v1.60）  
- ✅ 与 `seguiemj_1_31_mod.ttf` 结合，补充 Unicode 17.0 的新 emoji（🫪🫯🫈🧑‍🩰🫍🛘🪊🪎）

📌 技术说明：

- Chasmical 的字体并未替换全部 emoji — 它仅添加了来自 Twemoji v16.0.1 的 258 个国旗 emoji  
- 其余 emoji 保留自 Segoe UI Emoji v1.60 — 即 Fluent 3D 15.1（Windows 11 23H2，发布日期 2024-06-25）  
- 来自 Chasmical 仓库的说明：

  > *“此字体基于 Segoe UI Emoji v1.60（3D Fluent 15.1；Win11 23H2；2024-06-25），并包含来自 Twitter Color Emoji SVGinOT v16.0.1（2025-04-14）的 258 个国旗，由 quarrel 编译。”*

🧠 先安装 `seguiemj_1_31_mod.ttf` 后，系统会自动 fallback 到该字体以显示 Chasmical 字体中未包含的 Unicode 17.0 emoji。  
→ 这是一种巧妙的字体叠加策略：  
- 第一个字体提供新的 Unicode 字形  
- 第二个字体提供 Fluent 风格和国旗支持  
→ 最终效果：Windows 10 显示效果媲美 Windows 11，甚至更强，因为支持 Unicode 17.0。

---

### 📷 浏览器字体配置：确保国旗 emoji 正确显示

安装 `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` 后，我对浏览器进行了字体配置，以确保国旗 emoji 显示为彩色。

✅ 建议：使用 `'Noto Color Emoji'` 替代 `'Segoe UI Emoji'`，避免国旗 emoji 显示为蓝色或缺失。

---

### 📸 实际效果截图

#### 🧩 Windows 10 上的 Windows 11 风格 emoji 选择器

![Windows 10 上的 emoji 选择器](./screenshots/win10/Win10.Emoji.Picker.Style.Win11.p2.20250930.JPG)

---

#### 🌐 Chrome 配置 `'Noto Color Emoji'` 后的效果

![Chrome 中的国旗 emoji](./screenshots/win10/Win10.Chrome.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🌐 Edge 配置 `'Noto Color Emoji'` 后的效果

![Edge 中的国旗 emoji](./screenshots/win10/Win10.Edge.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🔍 Chrome 浏览 emojipedia.org — 测试 Unicode 17.0 emoji

![Chrome 浏览 emojipedia.org](./screenshots/win10/Win10.Chrome.blog.emojipedia.org.20250930.JPG)

---

### 🧪 系统兼容性对比表

| 操作系统 + 字体组合 | 支持 Unicode 17.0 | 支持国旗 emoji | 说明 |
|----------------------|--------------------|------------------|------|
| Win10 + `seguiemj_1_31_mod.ttf` | ✅ | ✅ | emoji 完整但风格较旧 |
| Win10 + `seguiemj_1_31_mod.ttf` + Twemoji Flags | ✅ | ✅ | emoji 完整且视觉现代 |
| Win11 + 仅安装 Twemoji Flags | ❌ | ✅ | 仅支持国旗，缺少 Unicode 17.0 emoji |

---
### 📢 总结

✅ **Windows 10 完全可以显示 Unicode 17.0 和彩色国旗 emoji**，  
只需按顺序安装字体：**先安装基础字体**，**再安装 Twemoji Flags 补丁**，  
并在浏览器中配置 `'Noto Color Emoji'`，确保国旗 emoji 正确显示。

## 🧪 兼容性矩阵

| 操作系统 + 字体 | Unicode 17.0 表情符号 | 彩色国旗 Emoji | 说明 |
|------------------|------------------------|------------------|------|
| Windows 10 + `seguiemj_1_31_mod.ttf` | ✅ | ✅ | 最佳组合 — 支持全部 emoji |
| Windows 11 + `seguiemj_1_33_mod.ttf` | ❌ | ✅ | 国旗显示正常，缺少新 emoji |
| Windows 11 + 仅安装 Twemoji Flags | ❌ | ✅ | 有彩色国旗，无 Unicode 17.0 表情 |
> 此表展示了在不同 Windows 系统中使用修改字体后的 emoji 支持情况。


## 🦊 全球挑战：修复 Firefox 中的国旗 emoji 显示问题
[![Firefox 国旗 Emoji 挑战](https://img.shields.io/badge/Firefox_Emoji_国旗挑战-🌏_立即参与-red)](guides/firefox.prefix.zh.md)

> Firefox 目前仍无法正确显示 Unicode 国旗 emoji。  
> 成功修复者将被收录在 [Firefox 荣誉墙](guides/firefox.wall-of-fame.zh.md) 🏅

- 🌍 [查看挑战详情](guides/firefox.prefix.zh.md)  
- 🛠️ [提交你的修复方案](guides/firefox.fix.template.zh.md)
## 🤔 与其他方案对比

你可能听说过以下项目：

- [`13rac1/twemoji-color-font`](https://github.com/13rac1/twemoji-color-font)
- 注入自定义 emoji 字体的脚本
- 使用 SVG 图片替代浏览器中的 emoji（如 Twemoji CDN）

每种方案都有其优缺点。

| 对比项                     | twemoji-color-font         | unicode-flags-for-windows     |
|----------------------------|----------------------------|-------------------------------|
| 国旗 emoji 显示正确？      | ⚠️ 可能正确（依赖系统）       | ✅ 稳定，原生 Unicode          |
| 其他 emoji 有颜色？        | ❌ 大多数是黑白的             | ✅ 全彩支持                    |
| 是否修改系统字体？         | ❌ 否                        | ✅ 是（含备份）                |
| 针对 Windows 10/11 优化？  | ❌ 尚未完善                   | ✅ 专为 Windows 优化           |
| 是否需要修改注册表？       | ❌ 否                        | ✅ 是（自动或手动）            |
| 支持 Firefox？             | ❌ 非目标平台                 | ❓（当前为挑战）               |
| 社区活跃度？               | ✅ 较活跃                     | 🆕 刚刚启动                    |

📣 想帮助 Firefox 正确显示国旗 emoji？  
→ [立即参与挑战](guides/firefox.prefix.zh.md) 🦊🔥


## 🇷🇺 Русский

### ✨ Обзор
Windows 10 и 11 по умолчанию не поддерживают полные флаговые эмодзи Unicode (например 🇻🇳 🇺🇸 🇯🇵 🇫🇷 🇩🇪). Этот репозиторий предлагает полное решение для исправления системы и корректного отображения флагов во всех приложениях.

Без ожидания обновлений от Microsoft. Без полумер. Это техническое решение от Tuannvbg — разработчика из Вьетнама, сделавшего всё, чтобы флаги отображались правильно.

## 🦊 Глобальный вызов: исправить отображение эмодзи-флагов в Firefox
[![Вызов Emoji-флагов Firefox](https://img.shields.io/badge/Firefox_Emoji_Флаги-🚩_Исправь_и_прославься-red)](guides/firefox.prefix.ru.md)

## 📚 Руководство по установке
🌐 Просмотреть другие языковые версии:  
🇻🇳 [Tiếng Việt](./guides/windows.vi.md)  
🇺🇸 [English version](./guides/windows.en.md)  
🇨🇳 [中文版本 (China)](./guides/windows.zh.md)  
🇷🇺 [Русская версия (Russia)](./guides/windows.ru.md)
## 🧪 Матрица совместимости

## 🌍 Emoji Picker, Unicode 17.0 — Техническое открытие о модификации emoji-флагов для Windows 10

### ✅ Рекомендуемая инструкция по установке

Это интересное открытие: установив шрифт `Segoe.UI.Emoji.with.Twemoji.Flags.ttf`, я получил возможность:

- Использовать emoji-панель в стиле Windows 11  
- Полноценно отображать emoji из Unicode 17.0 (🫪🫯🫈🧑‍🩰🫍🛘🪊🪎)  
- Отображать цветные emoji-флаги стран (🇻🇳🇺🇸🇯🇵)

---

### 🔹 Шаг 1: Ознакомьтесь с инструкцией 🇷🇺 [Русский](./guides/windows.ru.md)

### 🔹 Шаг 2: Установите шрифт, поддерживающий emoji-флаги

📁 Шрифт: [`Segoe.UI.Emoji.with.Twemoji.Flags.ttf`](https://github.com/Chasmical/flag-emojis-for-windows)  
📁 Или загрузите из: [`/fonts/`](https://github.com/tuannvbg/unicode-flags-for-windows/tree/main/fonts)

- ✅ Отображает цветные emoji-флаги (например: 🇯🇵🇫🇷🇧🇷)  
- ✅ Работает с emoji-панелью Windows (`Win + .`)  
- 🧩 Основан на Segoe UI Emoji v1.60 и дополнен Twemoji v16.0.1  
- 📌 Этот шрифт дополняет базовый — не заменяет его полностью

---

### 🔍 Технический анализ: объединение шрифтов для расширения поддержки emoji

Шрифт `seguiemj_1_31_mod.ttf` уже поддерживает emoji-флаги, но так как он основан на оригинальном шрифте Windows 10, визуальный стиль emoji устаревший — не такой современный, как Fluent 3D в Windows 11.

→ Поэтому я попробовал установить `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` от Chasmical, чтобы:

- ✅ Сохранить цветные emoji-флаги  
- ✅ Получить визуальный стиль emoji, как в Windows 11 (на базе Segoe UI Emoji v1.60)  
- ✅ Совместить с `seguiemj_1_31_mod.ttf` для поддержки Unicode 17.0 (🫪🫯🫈🧑‍🩰🫍🛘🪊🪎)

📌 Технические детали:

- Шрифт Chasmical не заменяет все emoji — он добавляет только 258 emoji-флагов из Twemoji v16.0.1  
- Остальные emoji взяты из Segoe UI Emoji v1.60 — Fluent 3D 15.1 (Windows 11 23H2, дата: 25 июня 2024)  
- Из репозитория Chasmical:

  > *“Этот шрифт основан на Segoe UI Emoji v1.60 (3D Fluent 15.1; Win11 23H2; 2024-06-25) и содержит 258 флагов из Twitter Color Emoji SVGinOT v16.0.1 (2025-04-14), собранных quarrel.”*

🧠 Установив сначала `seguiemj_1_31_mod.ttf`, система использует его как fallback для отображения emoji из Unicode 17.0, которых нет в шрифте Chasmical.  
→ Это умная стратегия объединения шрифтов:  
- Первый шрифт — для новых символов Unicode  
- Второй — для современного визуального стиля и флагов  
→ В результате Windows 10 отображает emoji как Windows 11 — но даже лучше, с поддержкой Unicode 17.0.

---

### 📷 Настройка шрифта в браузере для корректного отображения emoji-флагов

После установки `Segoe.UI.Emoji.with.Twemoji.Flags.ttf` я настроил браузер, чтобы emoji-флаги отображались в цвете.

✅ Совет: используйте `'Noto Color Emoji'` вместо `'Segoe UI Emoji'`, чтобы избежать синеватых или отсутствующих флагов.

---

### 📸 Примеры отображения

#### 🧩 Emoji-панель Windows 11 в Windows 10

![Emoji-панель Windows 11 в Windows 10](./screenshots/win10/Win10.Emoji.Picker.Style.Win11.p2.20250930.JPG)

---

#### 🌐 Chrome после настройки `'Noto Color Emoji'`

![Флаги в Chrome](./screenshots/win10/Win10.Chrome.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🌐 Edge после настройки `'Noto Color Emoji'`

![Флаги в Edge](./screenshots/win10/Win10.Edge.Show.Fonts.NotoColorEmoji.20250930.JPG)

---

#### 🔍 Chrome на сайте emojipedia.org — тест Unicode 17.0

![Chrome на emojipedia.org](./screenshots/win10/Win10.Chrome.blog.emojipedia.org.20250930.JPG)

### 🧪 Таблица совместимости

| ОС + Шрифт | Unicode 17.0 | Emoji-флаги | Примечание |
|--------------------------|----------------|------------------|-------------|
| Win10 + `seguiemj_1_31_mod.ttf` | ✅ | ✅ | Полный набор emoji, но устаревший стиль |
| Win10 + `seguiemj_1_31_mod.ttf` + Twemoji Flags | ✅ | ✅ | Полный набор emoji с современным стилем |
| Win11 + только Twemoji Flags | ❌ | ✅ | Только флаги, нет поддержки Unicode 17.0 |

---

### 📢 Заключение

✅ **Windows 10 полностью поддерживает Unicode 17.0 и цветные emoji-флаги**,  
если установить шрифты в правильном порядке: **сначала базовый**, **затем Twemoji Flags**,  
и настроить браузер на использование `'Noto Color Emoji'` для корректного отображения флагов.

| ОС + Шрифт | Emoji Unicode 17.0 | Флаги emoji | Примечание |
|------------|---------------------|--------------|------------|
| Windows 10 + `seguiemj_1_31_mod.ttf` | ✅ | ✅ | Идеальное сочетание — поддержка всех emoji |
| Windows 11 + `seguiemj_1_33_mod.ttf` | ❌ | ✅ | Флаги отображаются, но нет новых emoji |
| Windows 11 + только Twemoji Flags | ❌ | ✅ | Есть цветные флаги, нет Unicode 17.0 emoji |
> Эта таблица показывает, какие функции emoji поддерживаются в разных версиях Windows при использовании модифицированных шрифтов.


> Firefox всё ещё неправильно отображает эмодзи-флаги Unicode.  
> Тот, кто решит проблему, будет внесён в [Стену славы Firefox](guides/firefox.wall-of-fame.ru.md) 🏅

- 🌍 [Посмотреть вызов](guides/firefox.prefix.ru.md)  
- 🛠️ [Отправить своё решение](guides/firefox.fix.template.ru.md)
## 🤔 Сравнение с другими решениями

Возможно, вы слышали о таких проектах, как:

- [`13rac1/twemoji-color-font`](https://github.com/13rac1/twemoji-color-font)
- Скрипты для внедрения кастомных emoji-шрифтов
- Замена emoji на SVG-изображения в браузере (Twemoji CDN и др.)

У каждого подхода есть свои плюсы и минусы.

| Критерий                   | twemoji-color-font         | unicode-flags-for-windows     |
|----------------------------|----------------------------|-------------------------------|
| Эмодзи-флаги отображаются правильно? | ⚠️ Возможно (зависит от системы) | ✅ Стабильно, Unicode по умолчанию |
| Цветные эмодзи?            | ❌ В основном чёрно-белые    | ✅ Полноцветные                 |
| Меняет системные шрифты?   | ❌ Нет                      | ✅ Да (с резервной копией)      |
| Оптимизация под Windows 10/11? | ❌ Не завершена            | ✅ Специально оптимизировано    |
| Требуется правка реестра?  | ❌ Нет                      | ✅ Да (авто / вручную)          |
| Поддержка Firefox?         | ❌ Не целевая платформа     | ❓ (текущий вызов)              |
| Активность сообщества?     | ✅ Довольно активное         | 🆕 Только стартовало            |

📣 Хотите помочь Firefox правильно отображать эмодзи-флаги?  
→ [Примите участие в вызове](guides/firefox.prefix.ru.md) 🦊🔥


## 📸 Screenshots

### ✅ Copilot PC App
> Emoji flags rendered correctly in Copilot PC app on Windows 11  
![Copilot PC App Screenshot](screenshots/Copilot.PC.app.Windows11.Screenshot.2025-09-21.103357.jpg)

### ✅ Notepad
> Even the simplest app now displays Unicode flags properly  
![Notepad Screenshot](screenshots/Notepad.Screenshot.2025-09-21.103618.jpg)

### ✅ Visual Studio Code
> VS Code shows full emoji flags in markdown and code comments  
![VS Code Screenshot](screenshots/VSC2.Screenshot.2025-09-21.104033.jpg)

### ✅ Chrome Browser
> Chrome renders emoji flags perfectly after patch  
![Chrome Screenshot](screenshots/Chrome.Browser.Show.Screenshot.2025-09-21.111129.jpg)

### ✅ Microsoft Edge
> Edge displays emoji flags in Copilot Web and multilingual content  
![Edge Screenshot](screenshots/Edge.Browser.Show.Screenshot.2025-09-21.111408.jpg)

### ✅ Firefox Browser
> Firefox still fails to render Unicode flag emojis correctly  
![Firefox Screenshot](screenshots/Firefox.Browser.Screenshot.2025-09-21.183410.jpg)

---

## 🙌 Credits
- [`Chasmical/flag-emojis-for-windows`](https://github.com/Chasmical/flag-emojis-for-windows)
- [`perguto/Country-Flag-Emojis-for-Windows`](https://github.com/perguto/Country-Flag-Emojis-for-Windows)
- [`llccd.eu.org`](https://llccd.eu.org/2022/02/win_flags)
- [`13rac1/twemoji-color-font`](https://github.com/13rac1/twemoji-color-font)
- Copilot AI – technical brainstorming partner

---

## 💬 Author
Tuannvbg – the first Vietnamese developer to make Unicode flag emojis display correctly on Windows 😎🇻🇳🇺🇸

---

## 📄 License
This project is licensed under the MIT License – feel free to use, modify, and share it to help Unicode flag emojis display correctly across Windows systems.
