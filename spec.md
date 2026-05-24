# 珊瑚礁の頁 — design-seasidebookshop-sangosho Spec

**Status:** Approved  
**Author:** torifo  
**Created:** 2026-05-24  
**Updated:** 2026-05-24

## 1. Overview

### Problem Statement
南の島の書店サイトは、観光写真や土産物の印象が強くなりやすく、島の子どもや地元の読書体験が見えにくい。

### Goal
「珊瑚礁の頁」という架空書店を、旅人と島の子どもが同じ棚を見られる場所として実装する。絵本、民話、海図、自然観察を中心に、明るく親しみやすいUIを作る。

### Non-Goals
- 高級リゾート表現
- 観光土産EC
- 写真だけで成立させるランディングページ

## 2. User Stories

| ID | Persona | Want to | So that |
|---|---|---|---|
| US-01 | 親子連れ | 絵本や読み聞かせを知りたい | 子どもと立ち寄れる |
| US-02 | 旅人 | 海図や自然観察の本を見たい | 島を理解しながら旅できる |
| US-03 | 地元客 | 民話や日用品も見たい | 日常の店として使える |

## 3. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | 島形ヒーロー画像とピン表示 | P0 |
| FR-02 | 棚4分類 | P0 |
| FR-03 | 島の午後プログラム | P1 |
| FR-04 | 小さな市3分類 | P1 |
| FR-05 | 860px以下で1カラム化 | P0 |

## 4. Architecture

```text
index.html
├── nav
├── section.hero
├── section.shelf
├── section.map
├── section.market
└── footer
```

## 5. Design System

```css
--lime:  #fff8df;
--reef:  #1f8c8d;
--coral: #e66f5b;
--leaf:  #4f8a55;
--ink:   #233a35;
--sky:   #cdeee8;
```

## 6. Testing Strategy

| Layer | Scenarios |
|---|---|
| Desktop | 島形画像、ピン位置、棚4列 |
| Mobile | 島形画像の角丸化、棚1列化 |
| Accessibility | ピンと本文の読みやすさ |
