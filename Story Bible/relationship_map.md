# 🕸️ RELATIONSHIP MAP

> Bản đồ quan hệ nhân vật. Edit trực tiếp, xem trên GitHub.

---

## Bàn cờ tổng thể

```mermaid
graph TD
    subgraph "🌍 MACRO — Không can thiệp"
        USA["🇺🇸 USA"]
        RUS["🇷🇺 Russia"]
        UN["🌐 UN/SOGA"]
        USA ---|"Liên minh ngầm 50/50"| RUS
        USA --> UN
        RUS --> UN
    end

    subgraph "🇯🇵 QUỐC GIA"
        GOV["Japan Gov"]
        JSDF["JSDF"]
        XRU["X.R.U — O"]
        IHI["Ilumyx Heavy Industries"]
        UN --> GOV
        GOV --> JSDF
        GOV --> XRU
        IHI -.->|"trang bị"| XRU
    end

    subgraph "🏘️ THỊ TRẤN"
        MAYOR["Thị trưởng"]
        POLICE["Cảnh sát — 5-15 người"]
        SCHOOL["Trường học"]
        PEOPLE["Dân thị trấn"]
        GOV -.->|"bỏ mặc"| MAYOR
        JSDF -.->|"Green Demons — quét rồi đi"| ORC
    end

    subgraph "⚔️ CUỘC CHIẾN CỦA RUBY"
        RUBY["🔴 Akari / Esca Ruby"]
        FRIENDS["👥 Nhóm bạn thiên tài"]
        ORC["💀 Orc — Old World"]
        RUBY ---|"bảo vệ"| PEOPLE
        RUBY ---|"chiến đấu"| ORC
        FRIENDS ---|"hỗ trợ ngầm"| RUBY
        ORC -.->|"Phase 3: thao túng"| MAYOR
        ORC -.->|"Phase 3: thao túng"| SCHOOL
    end

    style RUBY fill:#ff4444,color:#fff,stroke:#ff0000
    style ORC fill:#6b21a8,color:#fff,stroke:#4c1d95
    style FRIENDS fill:#f59e0b,color:#000
    style XRU fill:#10b981,color:#fff
    style JSDF fill:#10b981,color:#fff
```

---

## Trường học — Monster Parent Wars

```mermaid
graph LR
    subgraph "Lớp A — Tokushin"
        PA["Phụ huynh A — quyền lực"]
        SA["Học sinh A"]
        PA -->|"quan hệ ruột"| PRINCIPAL["Hiệu trưởng"]
    end

    subgraph "Lớp B — Shingaku"
        PB["Phụ huynh B — tham vọng"]
        SB["Học sinh B + AKARI"]
        TB["Cô chủ nhiệm B — stress"]
        PB -->|"dọa kiện"| TB
        PB -->|"ép điểm"| TB
    end

    subgraph "Lớp C — Sōgō"
        PC["Phụ huynh C"]
        SC["Học sinh C"]
    end

    PA ===|"LIÊN MINH"| PC
    PA -.->|"spoil đề thi"| SC
    SA -->|"khinh"| SB
    SC -->|"điểm vượt"| SB

    style SB fill:#ff4444,color:#fff
    style TB fill:#fbbf24,color:#000
    style PA fill:#6b21a8,color:#fff
```

---

## Nhóm bạn Akari (chưa hoàn thiện)

```mermaid
graph TD
    AKARI["🔴 Akari"]

    BF1["👩 Bạn thân nữ 1 — sau bị bắt con tin"]
    BF2["👩 Bạn thân nữ 2"]
    BM1["👨 Bạn thân nam — support ngon"]
    GRP["👥 Nhóm thân 70% — 3-4 người"]
    TEAM["⭐ 2-3 người → team support MG"]
    BULLY["💢 Đầu gấu — sau bán mình cho quỷ?"]

    AKARI --- BF1
    AKARI --- BF2
    AKARI --- BM1
    AKARI -.- GRP
    GRP -.->|"mid game"| TEAM
    BULLY -.->|"chuyển phe?"| AKARI

    style AKARI fill:#ff4444,color:#fff
    style BF1 fill:#f87171,color:#fff
    style TEAM fill:#10b981,color:#fff
    style BULLY fill:#6b21a8,color:#fff
```

---

## Cách sử dụng

- **Edit trực tiếp** trong file này — Mermaid là text thuần
- **Xem đẹp** trên GitHub (tự render diagram)
- **AI đọc được** raw text → hiểu quan hệ nhân vật
- Thêm nhân vật: copy 1 dòng, đổi tên, nối mũi tên
- `---` = quan hệ 2 chiều, `-->` = 1 chiều, `-.->` = tiềm năng/chưa chắc
