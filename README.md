# WebSupmit — Professional Website Generator

WebSupmit là công cụ tạo website tĩnh chạy trực tiếp trên GitHub Pages. Người dùng chỉ cần điền các thông tin cơ bản, chọn phong cách hiển thị, xem trước theo thời gian thực và xuất ra một file index.html độc lập.

## Mục tiêu

- Không cần cài Node.js, framework hay backend.
- Không cần biết code để tạo một website giới thiệu chuyên nghiệp.
- Website xuất ra là HTML/CSS thuần, responsive và có thể chạy ở bất kỳ static hosting nào.
- Phù hợp cho portfolio cá nhân, landing page sản phẩm và website doanh nghiệp nhỏ.

## Tính năng

- 3 chế độ: Portfolio, Doanh nghiệp, Landing Page.
- Form nhập tên thương hiệu, headline, giới thiệu, liên hệ, ảnh/logo và liên kết xã hội.
- Dịch vụ và dự án nhập nhanh theo cú pháp: Tên | Mô tả.
- Bật/tắt từng section: Giới thiệu, Dịch vụ, Dự án, Liên hệ.
- Chọn màu nhấn, giao diện sáng/tối và phong cách font.
- Hỗ trợ tiếng Việt và tiếng Anh.
- Preview Desktop, Tablet, Mobile.
- Tự động lưu cấu hình vào localStorage.
- Nhập / xuất cấu hình JSON.
- Sao chép HTML hoặc tải trực tiếp index.html.
- Website đầu ra có SEO title, meta description, responsive layout và prefers-reduced-motion.
- Không phụ thuộc CDN hoặc thư viện JavaScript bên ngoài.

## Sử dụng

1. Mở WebSupmit trên GitHub Pages.
2. Chọn loại website.
3. Điền thông tin cá nhân hoặc doanh nghiệp.
4. Nhập các dịch vụ và dự án.
5. Chọn màu, giao diện và font.
6. Xem trước trên Desktop / Tablet / Mobile.
7. Nhấn Tải index.html.
8. Đưa file index.html vào một repository GitHub và bật GitHub Pages.

## Bật GitHub Pages cho repository này

Vào Settings → Pages → Build and deployment, chọn Deploy from a branch, sau đó chọn branch main và thư mục root (/).

Sau khi Pages được bật, địa chỉ dự kiến là:
https://base27-cvnss.github.io/websupmit/

## Cấu trúc

- index.html — toàn bộ ứng dụng WebSupmit.
- README.md — tài liệu.
- LICENSE — giấy phép MIT.
- .nojekyll — đảm bảo GitHub Pages phục vụ file tĩnh trực tiếp.

## Kiến trúc

WebSupmit dùng mô hình:

Form cấu hình → State JSON → Renderer → Live Preview → Static HTML Export

Cấu hình được giữ ở dạng JSON. Renderer dựng HTML từ dữ liệu đã escape và chỉ chấp nhận các URL an toàn phổ biến như HTTP(S), mailto, tel, anchor và đường dẫn tương đối.

## Hướng phát triển

Các bản sau có thể bổ sung:
- nhiều template hơn;
- upload ảnh và chuyển thành data URL;
- kéo-thả thứ tự section;
- export ZIP gồm assets;
- schema.org / Open Graph nâng cao;
- preset cho CV, doanh nghiệp, sản phẩm, nhà hàng, bất động sản, WebGIS;
- GitHub API để tạo repository và publish trực tiếp;
- thư viện template cộng đồng.

## Tham khảo thiết kế

Ý tưởng trải nghiệm "một website tĩnh có thể triển khai rất nhanh bằng GitHub Pages" được tham khảo từ dự án MIT:
https://github.com/Blandskron/portafolio-gratis-github-pages

WebSupmit được xây dựng lại như một website generator tổng quát, không sao chép nội dung portfolio mẫu.

## License

MIT License.
