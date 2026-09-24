# Seedance 2.0 API 日本語ガイド（seedance-2.0 / seedance2.0）

> 従量課金、最低 1 ドルから、OpenAI 互換エンドポイント。 **480P-input $0.04; 480P $0.066; 720P-input $0.0858**

**[模型页](https://go.apimart.ai/k-ff3568) · [实时价格](https://go.apimart.ai/k-e2b5b9) · [获取 API Key](https://go.apimart.ai/k-e08732)**

## 料金（快照 2026-09-24）

| 档位 | 单价 |
| --- | --- |
| `480P-input` | $0.04 |
| `480P` | $0.066 |
| `720P-input` | $0.0858 |
| `720P` | $0.142 |

按量计费、**$1 起充**，无订阅、无免费额度；每次任务响应返回 `cost` / `credits_cost`。

## 调用示例

```bash
curl --request POST --url https://api.apimart.ai/v1/videos/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"seedance-2.0","prompt":"海边悬崖的现代别墅，黄昏","size":"16:9","n":1}'
```

## 披露

本リポジトリはサードパーティ中継サービス APIMart の利用ガイドです。
