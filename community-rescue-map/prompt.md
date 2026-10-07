Bạn là chuyên gia thiết kế giao diện Web và Vibe Coding.

Hãy tạo trang `index.html` cho website:

**“Bản đồ Cứu trợ & Kết nối Cộng đồng”**

Mục tiêu của trang:

* Là trang chính của hệ thống.
* Giới thiệu ngắn gọn mục đích của Community Rescue.
* Hiển thị khu vực/bản đồ cứu trợ và các điểm đang cần hỗ trợ.
* Giúp người dùng nhanh chóng nhận biết loại nhu cầu: thực phẩm, y tế, nơi ở.
* Có lời kêu gọi người dùng đăng ký làm tình nguyện viên.
* Giao diện hiện đại, rõ ràng, dễ sử dụng và responsive.

## 1. CẤU TRÚC WEBSITE

Chỉ tạo trang:

`index.html`

Không tạo trang:

`requests.html`

Loại bỏ hoàn toàn chức năng và liên kết "Danh sách yêu cầu".

Website chỉ có 2 trang:

* `index.html`
* `volunteer.html`

Hai trang phải sử dụng chung một file:

`css/style.css`

Không tạo thêm file CSS riêng cho từng trang.

## 2. CÔNG NGHỆ BẮT BUỘC

Chỉ được sử dụng:

* HTML5
* CSS3
* Một file CSS external: `css/style.css`

TUYỆT ĐỐI KHÔNG sử dụng:

* JavaScript
* jQuery
* React
* Vue
* Bootstrap
* Tailwind
* Inline JavaScript
* JavaScript trong thẻ `<script>`
* CSS framework
* Thư viện UI bên ngoài
* Build tool
* npm
* API bản đồ bên ngoài

Không được tạo bất kỳ file `.js` nào.

## 3. SEMANTIC HTML

Phải sử dụng Semantic HTML5 phù hợp, bao gồm khi cần:

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<aside>`
* `<footer>`

Không sử dụng `<div>` cho mọi thành phần một cách máy móc.

Cấu trúc HTML phải có ý nghĩa rõ ràng, dễ đọc và dễ bảo trì.

## 4. HEADER

Tạo Header gồm:

* Logo/icon Community Rescue.
* Tên website.
* Mô tả ngắn.
* Navigation.

Navigation chỉ gồm:

* Bản đồ
* Đăng ký tình nguyện viên

Thiết lập:

`Bản đồ` → `index.html`

`Đăng ký tình nguyện viên` → `volunteer.html`

Không được xuất hiện liên kết:

`Danh sách yêu cầu`

Header sử dụng Flexbox.

Trên mobile, navigation phải tự điều chỉnh phù hợp với màn hình nhỏ.

## 5. INTRO / HERO SECTION

Tạo Hero Section nổi bật.

Nội dung phải được AI tự sinh nhưng phải phù hợp với chủ đề cứu trợ cộng đồng.

Hero nên có:

* Eyebrow text.
* Tiêu đề chính.
* Đoạn mô tả.
* CTA chính.
* CTA phụ nếu phù hợp.
* Hình ảnh hoặc khu vực minh họa bản đồ bằng HTML/CSS.

CTA chính dẫn đến:

`volunteer.html`

Không sử dụng JavaScript cho CTA.

## 6. INTRO ANIMATION

Khi trang vừa được tải:

Header và Hero phải xuất hiện có chuyển động.

Yêu cầu:

* Header: Fade-in.
* Hero: Fade-in + Slide-up.
* Các thành phần bên trong Hero có thể xuất hiện lần lượt bằng animation-delay.

Chỉ sử dụng:

* `opacity`
* `transform`
* `translate()`
* `scale()`

Không sử dụng:

* `top`
* `left`
* `right`
* `bottom`

để tạo animation.

Ví dụ có thể sử dụng:

`transform: translateY(...)`

và:

`opacity: 0 → 1`

Animation phải nhẹ, tự nhiên và không gây cảm giác chậm.

## 7. MASTER PROMPT VỀ CHUYỂN ĐỘNG

Trong quá trình xây dựng CSS animation, hãy áp dụng nguyên tắc:

“Điều chỉnh cubic-bezier cho từng loại chuyển động để animation có cảm giác tự nhiên, không máy móc; sử dụng easing có gia tốc và giảm tốc hợp lý, ưu tiên chuyển động ngắn, mượt và tinh tế thay vì hiệu ứng quá mạnh.”

Ưu tiên sử dụng:

`cubic-bezier(...)`

phù hợp với từng nhóm animation.

Không sử dụng một easing duy nhất cho toàn bộ website nếu không cần thiết.

## 8. KHU VỰC BẢN ĐỒ CỨU TRỢ

Tạo một khu vực bản đồ mô phỏng bằng HTML + CSS.

Không sử dụng Google Maps API hoặc bất kỳ API bản đồ nào.

Có thể sử dụng:

* CSS background
* CSS Grid
* các đường phố mô phỏng
* marker
* card thông tin

Tạo các marker theo loại:

* Thực phẩm
* Y tế
* Nơi ở

Mỗi loại có màu nhận diện riêng.

Ví dụ:

* Thực phẩm → đỏ/cam
* Y tế → xanh dương
* Nơi ở → xanh lá

AI tự sinh dữ liệu mẫu phù hợp.

Không cần dữ liệu thực tế.

## 9. INTERACTIVE CARD / MENU

Tạo các Card giới thiệu các loại hỗ trợ hoặc hoạt động cộng đồng.

Card phải có hiệu ứng tương tác bằng CSS.

Có thể sử dụng:

* Hover
* Transform
* Scale
* TranslateY
* Box-shadow
* Flip bằng CSS nếu thực sự phù hợp

Không sử dụng JavaScript.

Khi hover:

* Card nâng nhẹ.
* Shadow thay đổi.
* Nội dung được nhấn mạnh.
* Có transition mượt.

Không làm hiệu ứng quá mạnh gây khó chịu.

## 10. SCROLL REVELATION

Yêu cầu ban đầu của đề bài đề cập thư viện AOS.

Tuy nhiên trang này bị ràng buộc:

“CHỈ HTML + EXTERNAL CSS, KHÔNG JAVASCRIPT.”

Do AOS là thư viện JavaScript nên KHÔNG được sử dụng AOS.

Thay thế AOS bằng CSS Animation hoặc CSS Scroll-Driven Animation nếu trình duyệt hỗ trợ.

Mục tiêu vẫn phải đạt được:

* Section xuất hiện mượt khi người dùng cuộn.
* Có hiệu ứng fade-in.
* Có thể kết hợp translateY.
* Không sử dụng JavaScript.

Không được thêm `<script>` chỉ để triển khai AOS.

## 11. MICRO-INTERACTIONS

Tất cả CTA và button phải có trạng thái:

* Normal
* Hover
* Active
* Focus

Ví dụ:

Hover:

* thay đổi màu nhẹ
* translateY nhẹ
* shadow thay đổi

Active:

* button giảm nhẹ kích thước bằng `transform: scale()`
* tạo cảm giác người dùng vừa nhấn nút

Không dùng JavaScript.

## 12. FLEXBOX VÀ CSS GRID

Bắt buộc thể hiện rõ việc sử dụng:

Flexbox cho:

* Header
* Navigation
* Button group
* Legend
* Một số layout ngang

CSS Grid cho:

* Khu vực card
* Thống kê
* Các khu vực nội dung chính
* Responsive layout

Không sử dụng layout bằng hàng loạt `position: absolute`.

`position: absolute` chỉ được sử dụng khi thực sự cần thiết, ví dụ marker trên bản đồ mô phỏng.

## 13. DESIGN SYSTEM

File `css/style.css` phải có Design System bằng CSS Variables trong `:root`.

Bao gồm tối thiểu:

* Màu chính
* Màu phụ
* Màu nền
* Màu chữ
* Màu từng loại cứu trợ
* Khoảng cách
* Border radius
* Box shadow
* Transition
* Font family

Các component phải ưu tiên sử dụng CSS Variables thay vì viết màu và khoảng cách lặp lại.

## 14. RESPONSIVE

Website phải responsive.

Thiết kế tối thiểu cho:

* Desktop
* Tablet
* Mobile

Sử dụng Media Query.

Trên mobile:

* Header thu gọn.
* Navigation phù hợp.
* Hero chuyển sang một cột.
* Card chuyển sang một cột.
* Bản đồ vẫn dễ quan sát.
* CTA dễ bấm bằng ngón tay.
* Không xuất hiện horizontal scrollbar.

## 15. UX

Ưu tiên:

* Nội dung dễ đọc.
* CTA rõ ràng.
* Phân cấp thông tin tốt.
* Khoảng trắng hợp lý.
* Màu sắc có ý nghĩa.
* Animation hỗ trợ định hướng người dùng.

Không dùng animation chỉ để trang “trông nhiều hiệu ứng”.

Animation phải phục vụ UX.

## 16. HIỆU NĂNG

Tuyệt đối không sử dụng:

`top`

`left`

`right`

`bottom`

để tạo chuyển động.

Animation chỉ ưu tiên:

`transform`

`opacity`

Hạn chế animation quá dài.

Không tạo quá nhiều animation chạy đồng thời.

Không sử dụng video background hoặc tài nguyên nặng.

## 17. ACCESSIBILITY

Sử dụng:

* `alt` phù hợp nếu có hình ảnh.
* `aria-label` khi cần.
* Semantic HTML.
* Focus state cho button và link.
* Màu chữ đủ tương phản.
* Có hỗ trợ `prefers-reduced-motion`.

Nếu người dùng bật giảm chuyển động, giảm hoặc tắt các animation không cần thiết.

## 18. TỰ SINH NỘI DUNG

AI tự sinh toàn bộ nội dung mẫu phù hợp với website.

Không sử dụng nội dung vô nghĩa như:

“Lorem ipsum”.

Nội dung phải bằng tiếng Việt và phù hợp với chủ đề cứu trợ cộng đồng.

## 19. COMMENT SAU MỖI DÒNG LỆNH

Đây là yêu cầu quan trọng để phục vụ việc học.

Mỗi dòng HTML và CSS quan trọng phải có comment giải thích ý nghĩa.

Ví dụ:

```html
<header class="site-header">
<!-- Tạo khu vực Header semantic cho website -->
```

```css
display: flex;
/* Sử dụng Flexbox để sắp xếp các phần tử theo hàng hoặc cột */
```

Không giải thích lan man.

Comment phải ngắn gọn, chính xác và dễ hiểu đối với sinh viên.

## 20. OUTPUT

Chỉ xuất:

1. Nội dung hoàn chỉnh của `index.html`.

Không tạo JavaScript.

Không tạo CSS inline.

Không tạo file CSS riêng.

Không tạo `requests.html`.

Cuối code ghi chú ngắn:

* Semantic HTML được sử dụng ở đâu.
* Flexbox được sử dụng ở đâu.
* Grid được sử dụng ở đâu.
* Responsive được triển khai ở đâu.
* Design System nằm ở đâu.
* Animation nằm ở đâu.
* Vì sao không sử dụng AOS.


Bạn là chuyên gia thiết kế giao diện Web và Vibe Coding.

Hãy tạo trang:

`volunteer.html`

cho website:

**“Bản đồ Cứu trợ & Kết nối Cộng đồng”**

Đây là trang đăng ký tình nguyện viên.

Trang phải đồng bộ hoàn toàn với `index.html` và sử dụng chung:

`css/style.css`

## 1. CÔNG NGHỆ BẮT BUỘC

CHỈ được sử dụng:

* HTML5
* CSS3
* External CSS

File CSS dùng chung:

`css/style.css`

TUYỆT ĐỐI KHÔNG sử dụng:

* JavaScript
* jQuery
* React
* Vue
* Bootstrap
* Tailwind
* JavaScript library
* CSS framework
* Inline JavaScript
* `<script>`
* File `.js`

Không tạo thêm CSS riêng cho trang này.

## 2. SEMANTIC HTML

Sử dụng Semantic HTML5 phù hợp:

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<aside>`
* `<form>`
* `<fieldset>`
* `<legend>`
* `<label>`
* `<footer>`

Không dùng `<div>` thay thế toàn bộ Semantic HTML.

## 3. HEADER

Header phải giống hệ thống `index.html`.

Navigation chỉ có:

* Bản đồ
* Đăng ký tình nguyện viên

Link:

`index.html`

và:

`volunteer.html`

Không có:

`requests.html`

Trang hiện tại phải đánh dấu:

`Đăng ký tình nguyện viên`

bằng class:

`active`

## 4. HERO SECTION

Tạo phần giới thiệu trang đăng ký.

AI tự sinh nội dung tiếng Việt phù hợp.

Nội dung nên thể hiện:

* Tình nguyện viên có thể hỗ trợ cộng đồng.
* Các kỹ năng/hình thức hỗ trợ.
* Lời kêu gọi đăng ký.

Không sử dụng Lorem ipsum.

## 5. INTRO ANIMATION

Khi trang được tải:

Header và Hero phải xuất hiện bằng animation.

Header:

* Fade-in

Hero:

* Fade-in
* Slide-up

Chỉ sử dụng:

`opacity`

và:

`transform: translate()`

Không sử dụng:

`top`

`left`

`right`

`bottom`

để tạo animation.

## 6. FORM ĐĂNG KÝ

Tạo form đăng ký tình nguyện viên.

Form phải có các trường phù hợp, ví dụ:

* Họ và tên
* Số điện thoại
* Email
* Địa chỉ/khu vực hoạt động
* Hình thức hỗ trợ
* Kỹ năng
* Thời gian có thể hỗ trợ
* Nội dung giới thiệu hoặc ghi chú

Sử dụng HTML5 validation.

Ví dụ:

`required`

`type="email"`

`type="tel"`

Không dùng JavaScript để kiểm tra form.

## 7. FIELDSET

Các nhóm thông tin liên quan phải được tổ chức bằng:

`<fieldset>`

và:

`<legend>`

để tăng tính semantic và accessibility.

## 8. SUPPORT OPTIONS

Tạo nhóm lựa chọn hình thức hỗ trợ.

Ví dụ:

* Hỗ trợ thực phẩm
* Hỗ trợ y tế
* Hỗ trợ nơi ở
* Vận chuyển
* Hỗ trợ thông tin
* Hỗ trợ khác

Có thể sử dụng checkbox.

Thiết kế checkbox rõ ràng và dễ thao tác trên mobile.

## 9. INTERACTIVE CARD

Bên cạnh form, tạo một số Card mô tả:

* Vì sao nên tham gia?
* Bạn có thể hỗ trợ gì?
* Quy trình tham gia.

Các Card phải có CSS Hover Effect.

Khi hover:

* translateY nhẹ
* shadow thay đổi
* transition mượt

Có thể sử dụng Flip Card bằng CSS nếu phù hợp.

Không sử dụng JavaScript.

## 10. MICRO-INTERACTIONS

Nút:

`Đăng ký tình nguyện`

phải có:

* Normal
* Hover
* Active
* Focus

Hover có thể:

* đổi màu
* translateY
* thay đổi shadow

Active có thể:

`transform: scale(...)`

để tạo phản hồi khi click.

Không sử dụng JavaScript.

## 11. SCROLL REVELATION

Đề bài có yêu cầu AOS.

Tuy nhiên:

AOS là thư viện JavaScript.

Trang này bắt buộc:

“CHỈ HTML + EXTERNAL CSS, KHÔNG JAVASCRIPT.”

Vì vậy KHÔNG được sử dụng AOS.

Thay thế bằng:

* CSS Animation
* CSS Scroll-Driven Animation nếu trình duyệt hỗ trợ

Mục tiêu:

* Section xuất hiện khi người dùng cuộn.
* Fade-in.
* Slide-up.
* Chuyển động nhẹ.

Không thêm `<script>` để giả lập AOS.

## 12. MASTER PROMPT VỀ CUBIC-BEZIER

Áp dụng nguyên tắc:

“Điều chỉnh cubic-bezier cho các chuyển động để tạo cảm giác tự nhiên và chuyên nghiệp. Animation phải có gia tốc và giảm tốc hợp lý, thời gian vừa đủ để người dùng cảm nhận nhưng không làm chậm thao tác.”

Ưu tiên:

`transform`

`opacity`

`cubic-bezier(...)`

Không sử dụng animation quá mạnh.

## 13. FLEXBOX

Sử dụng Flexbox cho các khu vực phù hợp:

* Header
* Navigation
* Button group
* Các nhóm lựa chọn
* Các hàng nội dung nhỏ

## 14. CSS GRID

Sử dụng CSS Grid cho:

* Layout form + aside
* Card
* Nhóm thông tin
* Responsive layout

Trên desktop có thể dùng hai cột.

Trên mobile chuyển thành một cột.

## 15. DESIGN SYSTEM

Không tạo Design System riêng.

Sử dụng Design System chung trong:

`css/style.css`

Các CSS Variables tối thiểu gồm:

* Colors
* Typography
* Spacing
* Border radius
* Shadows
* Transition
* Animation timing

Không hard-code quá nhiều giá trị lặp lại.

## 16. RESPONSIVE

Trang phải hoạt động tốt trên:

* Desktop
* Tablet
* Mobile

Trên mobile:

* Form chuyển một cột.
* Aside chuyển xuống dưới hoặc lên trên tùy UX.
* Input rộng toàn màn hình.
* Button đủ lớn để thao tác bằng ngón tay.
* Không có horizontal scrollbar.
* Navigation dễ sử dụng.

## 17. ACCESSIBILITY

Bắt buộc:

* Mỗi input phải có `<label>`.
* Sử dụng `for` và `id` chính xác.
* Sử dụng `fieldset` và `legend` cho nhóm lựa chọn.
* Focus state rõ ràng.
* Đảm bảo độ tương phản.
* Hỗ trợ `prefers-reduced-motion`.

## 18. HIỆU NĂNG

Không sử dụng:

`top`

`left`

`right`

`bottom`

để tạo chuyển động.

Chuyển động chỉ ưu tiên:

`transform`

`opacity`

Không tạo animation quá dài.

Không tạo quá nhiều animation chạy cùng lúc.

Không sử dụng thư viện animation JavaScript.

## 19. COMMENT SAU MỖI DÒNG LỆNH

Đây là yêu cầu bắt buộc.

Mỗi dòng HTML và CSS quan trọng phải có comment ngắn giải thích ý nghĩa.

Ví dụ:

```html
<form class="volunteer-form">
<!-- Tạo biểu mẫu để người dùng đăng ký làm tình nguyện viên -->
```

```css
display: grid;
/* Sử dụng CSS Grid để chia bố cục form thành các khu vực */
```

Comment phải:

* Ngắn.
* Dễ hiểu.
* Đúng với chức năng của dòng lệnh.
* Phù hợp với sinh viên đang học HTML/CSS.

## 20. TỰ SINH NỘI DUNG

AI tự tạo nội dung tiếng Việt phù hợp với chủ đề.

Không sử dụng Lorem ipsum.

Không sao chép nội dung từ website khác.

## 21. OUTPUT

Chỉ xuất:

1. Nội dung hoàn chỉnh của `volunteer.html`.

Không xuất JavaScript.

Không tạo file CSS mới.

Không tạo `requests.html`.

Không sử dụng AOS.

Trang phải sử dụng:

`css/style.css`

làm CSS external dùng chung với `index.html`.

Cuối code ghi chú ngắn:

* Semantic HTML được sử dụng ở đâu.
* Flexbox được sử dụng ở đâu.
* Grid được sử dụng ở đâu.
* Responsive được triển khai ở đâu.
* Design System được dùng từ đâu.
* Animation được triển khai như thế nào.
* Vì sao không sử dụng AOS.
