# AdFlex ZNS — Tài liệu API

Tài liệu tích hợp cho đối tác, dựng bằng [Mintlify](https://mintlify.com).
Xuất bản tại **https://docs-zns.adflex.vn**

## Xem tại máy

```bash
npx mint@latest dev
```

Mở http://localhost:3000

## Cấu trúc

| Đường dẫn | Nội dung |
|---|---|
| `docs.json` | Cấu hình site: điều hướng, màu, logo |
| `index.mdx` · `authentication.mdx` | Trang mở đầu |
| `guides/` | Hướng dẫn tích hợp theo chủ đề |
| `logo/` | Wordmark và favicon |

## Tham chiếu API

Tab **API Reference** sinh tự động từ đặc tả OpenAPI mà ứng dụng phục vụ tại
`https://business.adflex.vn/openapi.json`. Đặc tả nằm cùng repo mã nguồn và có test
đối chiếu với route thật, nên không cần đồng bộ thủ công — deploy backend là trang
tham chiếu cập nhật theo.

Sửa endpoint thì sửa ở repo mã nguồn, không sửa ở đây.

## Kiểm tra trước khi push

```bash
npx mint@latest validate       # cấu hình + build
npx mint@latest broken-links   # liên kết nội bộ
```
