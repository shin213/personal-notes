# MATLyS Inc. 組織図

MATLyS Inc.の組織構造とコアエンジン、事業サイドの関係を示す図です。

```mermaid
graph LR
    %% 会社全体
    M[MATLyS Inc.]

    %% コアエンジン
    subgraph CORE["MATLyS ONE<br/>コアAI/データサイエンスエンジン"]
        F[古川]
        K[海里]
        Mu[村上]
    end

    %% 事業側
    subgraph BIZ["事業サイド"]
        SLS[営業部隊]
        SWE["SWEチーム<br/>(自社開発チーム)"]
    end

    %% 階層関係
    M --> CORE
    M --> BIZ

    %% 役割・フロー
    SLS -- 案件獲得 --> SWE
    SWE -- "「MATLyS ONE」のAPI提供依頼" --> CORE
    CORE -- "API提供/共通基盤機能" --> SWE
```

## 概要

- **MATLyS ONE**: コアAI/データサイエンスエンジン（古川、海里、村上で構成）
- **事業サイド**: 営業部隊とSWEチーム（自社開発チーム）
- **関係性**: 営業部隊が案件を獲得 → SWEチームが実装 → COREからAPI提供を受ける
