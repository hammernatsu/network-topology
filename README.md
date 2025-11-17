# network-topology

## 網路拓撲圖

```
ISP (機櫃)
  ↓
UCG-Ultra (書房) - 主要網關
  ↓
US-8-PoE (書房) - 主交換機
  ├─ U6-Pro (客廳沙發) - PoE 供電
  ├─ USW-Flex-Mini (客廳電視櫃) - 客廳區域擴充
  └─ USW-Lite-8-PoE (書房) - 書房區域擴充
      └─ U6-Lite (書房) - PoE 供電
```

## 設備清單

### 核心網路設備

| 設備型號 | 位置 | 功能 | 備註 |
|---------|------|------|------|
| UCG-Ultra (UniFi Cloud Gateway Ultra) | 書房 | 主要網關/路由器 | 核心控制器 |
| US-8-PoE | 書房 | 8埠 PoE 主交換機 | 連接 UCG-Ultra |
| USW-Lite-8-PoE | 書房 | 8埠 PoE 交換機 | 書房區域擴充 |
| USW-Flex-Mini | 客廳電視櫃 | 5埠交換機 | 客廳區域擴充 |

### 無線存取點 (AP)

| 設備型號 | 位置 | 規格 | 供電方式 |
|---------|------|------|---------|
| U6-Pro | 客廳沙發 | WiFi 6 | PoE (US-8-PoE) |
| U6-Lite | 書房 | WiFi 6 | PoE (USW-Lite-8-PoE) |

---

**文件版本**: 1.0  
**更新日期**: 2025-11-17  
**維護者**: Hammer