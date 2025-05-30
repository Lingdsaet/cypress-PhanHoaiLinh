# cypress-PhanHoaiLinh
Dưới đây là nội dung mẫu file `README.md` cho bài kiểm thử **giỏ hàng và thanh toán** bằng **Cypress** tại trang [https://www.saucedemo.com](https://www.saucedemo.com):

---

```markdown
#  E2E Testing - SauceDemo Cart & Checkout (Cypress)

##  Mô tả dự án

Dự án này sử dụng **Cypress** để kiểm thử End-to-End (E2E) các chức năng chính trên trang [SauceDemo](https://www.saucedemo.com), bao gồm:

- Đăng nhập
- Thêm/xóa sản phẩm khỏi giỏ hàng
- Sắp xếp sản phẩm theo giá
- Quy trình thanh toán (checkout)

## Cấu trúc thư mục

```

/cypress

└── /e2e

└── cart\_spec.cy.js   # Chứa các kịch bản kiểm thử chính

````

##  Hướng dẫn cài đặt và chạy kiểm thử

### 1. Cài đặt Cypress

```bash
npm init -y
npm install cypress --save-dev
````

### 2. Mở giao diện Cypress

```bash
npx cypress open
```

Chọn E2E Testing → Chọn trình duyệt → Chạy file `cart_spec.cy.js`

---

##  Các kịch bản kiểm thử

| Kịch bản         | Mô tả                                                                 |
| ---------------- | --------------------------------------------------------------------- |
| Đăng nhập        | Đăng nhập bằng tài khoản `standard_user`                              |
| Thêm sản phẩm    | Nhấn "Add to cart" cho sản phẩm đầu tiên                              |
| Xóa sản phẩm     | Nhấn "Remove", kiểm tra giỏ hàng không còn sản phẩm                   |
| Sắp xếp sản phẩm | Sắp xếp theo giá tăng dần (`low to high`)                             |
| Thanh toán       | Thêm sản phẩm → Checkout → Nhập thông tin → Chuyển đến trang xác nhận |

---

## Thông tin đăng nhập mẫu

* **Username:** `standard_user`
* **Password:** `secret_sauce`

---

##  Công nghệ sử dụng

* [Cypress](https://www.cypress.io/)
---

##  Ghi chú

* Nếu muốn quan sát từng bước chậm lại, có thể thêm `cy.wait(1000)` sau mỗi thao tác hoặc cấu hình trong `cypress.config.js`.

---

##  Liên hệ

Người thực hiện: **Phan Hoài Linh**
MSSV: `BIT220096`

---

```


