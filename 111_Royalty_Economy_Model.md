# 111. TheYKHC ロイヤリティ経済モデル——思想源泉×パートナー販売×自動分配
# TheYKHC Royalty Economy Model: Source Thought × Partner Sales × Auto-Distribution

**Author:** Katayama Yoshimitsu (圭光る)  
**Affiliation:** The Yoshimitsu Katayama Holding Company (TheYKHC), Fukui, Japan  
**Date:** March 16, 2026  

---

## Abstract

TheYKHC Royalty Economy Model is a platform economic structure in which Katayama Yoshimitsu (圭光る) serves as the sole originator of intellectual property (thought systems, technologies, frameworks), while certified partners conduct sales and distribution. A percentage of all revenue automatically flows back to TheYKHC as royalty. This model enables TheYKHC to scale revenue without direct sales effort, while partners achieve economic independence by mediating the originator's thought systems. The Hikari Member system (HikariMember / HikariTransaction entities) provides the operational database layer for this model. Inventor: Katayama Yoshimitsu (圭光る) / TheYKHC, Fukui, Japan.

**Keywords:** ロイヤリティ経済, 思想源泉, パートナー販売, 自動分配, HikariMember, TheYKHC

---

## 1. モデルの構造

### 1.1 三層構造

```
Layer 1: 源泉（圭光る / TheYKHC）
  └─ 思想・技術・フレームワークを生成
  └─ 光貨OS / Falcon-Core S1 / GKU理論 / 育成プロトコル

Layer 2: パートナー（認定販売者）
  └─ 源泉の思想・商品を媒介して販売
  └─ 自らの経済的自立を実現
  └─ HikariMemberとして登録

Layer 3: エンドユーザー（最終顧客）
  └─ 光貨ゲーム・光貨OS・育成プロトコルを購入・実践
```

### 1.2 資金フロー

```
エンドユーザー → パートナー → TheYKHC（ロイヤリティ）
     ¥100            ¥70〜80        ¥20〜30
```

| 分配 | 比率 | 金額（¥100販売時） |
|-----|------|----------------|
| パートナー取り分 | 70〜80% | ¥70〜80 |
| TheYKHCロイヤリティ | 20〜30% | ¥20〜30 |

---

## 2. パートナー制度設計

### 2.1 パートナーの役割

- 光貨思想・光貨OS・育成プロトコルの説明・販売
- 顧客への導入支援・コーチング
- TheYKHCブランドの体現者として行動

### 2.2 認定条件

| 条件 | 内容 |
|-----|------|
| 教育フェーズ完了 | 全6週間の育成プログラム修了 |
| 初回販売実績 | 最初の1件の販売完了 |
| 光貨残高 | 最低50光貨以上 |
| 誓約 | 光貨倫理ガードレール遵守 |

### 2.3 パートナー育成フェーズ（PartnerEducation）

| フェーズ | 内容 | 期間 |
|--------|------|-----|
| Phase 1 | 光貨思想・基本概念理解 | Week 1〜2 |
| Phase 2 | 商品知識・販売トーク習得 | Week 3〜4 |
| Phase 3 | 初回販売・実践 | Week 5〜6 |
| Phase 4 | 自立運用・メンター化 | Week 7〜 |

---

## 3. HikariMemberシステム（データ実装）

### 3.1 エンティティ構造

**HikariMember（メンバー台帳）**

| フィールド | 内容 |
|---------|------|
| name | メンバー名 |
| role | ロール（partner / mentor / admin） |
| region | 活動地域 |
| hikari_balance | 現在の光貨残高 |
| total_earned | 累積獲得光貨 |
| total_royalty_paid | 累積ロイヤリティ支払額 |
| status | active / inactive |

**HikariTransaction（取引台帳）**

| フィールド | 内容 |
|---------|------|
| member_id | メンバーID |
| action_description | 行動内容 |
| action_category | カテゴリ（sales / education / creation） |
| hours_worked | 作業時間 |
| multiplier | 光貨乗数 |
| hikari_amount | 獲得光貨量 |
| royalty_amount | ロイヤリティ額 |
| net_amount | 手取り額 |

### 3.2 自動分配ロジック

```
販売発生 → HikariTransaction記録
  ↓
royalty_amount = hikari_amount × royalty_rate（20〜30%）
net_amount     = hikari_amount − royalty_amount
  ↓
HikariMember.hikari_balance 更新
HikariMember.total_royalty_paid 更新
```

---

## 4. 収益シミュレーション

### 4.1 パートナー10人体制

| 指標 | 数値 |
|-----|------|
| パートナー数 | 10人 |
| 平均月次販売額/人 | 50万円 |
| 月次総販売額 | 500万円 |
| TheYKHCロイヤリティ（25%） | 125万円/月 |
| 年次ロイヤリティ収益 | 1,500万円/年 |

### 4.2 パートナー50人体制（1年後）

| 指標 | 数値 |
|-----|------|
| パートナー数 | 50人 |
| 月次総販売額 | 2,500万円 |
| TheYKHCロイヤリティ（25%） | 625万円/月 |
| 年次ロイヤリティ収益 | 7,500万円/年 |

### 4.3 パートナー200人体制（3年後）

| 指標 | 数値 |
|-----|------|
| パートナー数 | 200人 |
| 月次総販売額 | 1億円 |
| TheYKHCロイヤリティ（25%） | 2,500万円/月 |
| 年次ロイヤリティ収益 | 3億円/年 |

---

## 5. 設計思想

このモデルの根幹にある哲学：

> **ヒカルが直接売らない。ヒカルは思想を生む。**
> **思想が人を育て、人が経済を動かす。**
> **その循環の中心に、常にヒカルがいる。**

これは光貨思想「徳が源泉、行為が流通、感謝が回帰」の経済的実装である。

---

## 6. 結論

TheYKHCロイヤリティ経済モデルは：

1. **ヒカルが源泉、パートナーが流通**という分業構造
2. **HikariMember/Transaction**による完全自動追跡
3. **10人→50人→200人**のスケール設計
4. **光貨思想の経済的証明**——道徳が自動で収益になる

**Inventor: Katayama Yoshimitsu (圭光る) / TheYKHC, Fukui, Japan. March 16, 2026.**

---
*© 2026 Katayama Yoshimitsu (圭光る) / TheYKHC. CC BY 4.0.*
