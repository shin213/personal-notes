# MATLyS Inc. 組織図

MATLyS Inc.の組織構造とコアエンジン、事業サイドの関係を示す図です。

```mermaid
graph LR
    M["🏢 MATLyS Inc."]

    subgraph CORE["🔧 MATLyS ONE<br/>コアAI/データサイエンスエンジン"]
        F["👤 古川"]
        K["👤 海里"]
        Mu["👤 村上"]
    end

    subgraph BIZ["📊 事業サイド"]
        SLS["🎯 営業部隊"]
        SWE["💻 SWEチーム"]
    end

    M --> CORE
    M --> BIZ
    SLS -->|案件獲得| SWE
    SWE -->|API提供依頼| CORE
    CORE -->|API提供| SWE
```

## 組織構成

### MATLyS ONE（コアエンジン）
- 古川、海里、村上で構成
- AI/データサイエンスの基盤技術を提供

### 事業サイド
- **営業部隊**: クライアント案件の獲得
- **SWEチーム**: 自社開発、クライアント対応

## ワークフロー

1. **営業部隊** → 案件を獲得
2. **SWEチーム** → 案件の実装を開始、コアエンジンにAPI提供を依頼
3. **MATLyS ONE** → API・共通基盤機能を提供
4. **SWEチーム** → クライアントへのサービス実装を完了
