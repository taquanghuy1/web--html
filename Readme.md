# AI sử dụng chat GPT 
# Prompt đã sử dụng hãy viết CSS để áp dụng cho trang HTML sau (KHÔNG thay đổi HTML, chỉ thêm CSS trong thẻ <style>)
-Trang đang dùng thẻ <table> và <center>, giữ nguyên cấu trúc
-Thiết kế giống landing page của Apple (MacBook)
-Nền toàn trang màu xám rất nhạt (#f5f5f7)
-Font chữ sử dụng system font của Apple (-apple-system, BlinkMacSystemFont,...)
-Navbar nằm ngang, chữ nhỏ gọn, khoảng cách đều, hover đổi màu xanh (#0071e3)
-Tiêu đề "MacBook Neo" lớn (50–60px), đậm, căn giữa
-Dòng mô tả nhỏ hơn, màu xám (#6e6e73), căn giữa
Hai nút:
-"Learn more": nền xanh gradient, chữ trắng, bo tròn
-"Buy": nền trắng, viền xanh, chữ xanh, bo tròn
-Nút có hiệu ứng hover (giảm opacity hoặc đổi màu nhẹ)
-Ảnh MacBook nằm giữa phía dưới, có khoảng cách với nội dung trên
-Bo góc nhẹ cho ảnh
-Khoảng cách giữa các phần thoáng, giống phong cách Apple
-Có responsive cơ bản (màn hình nhỏ thì chữ và ảnh nhỏ lại)
# Kết quả
AI đã sinh ra CSS giúp giao diện:

Căn giữa toàn bộ nội dung
Hiển thị giống phong cách Apple
Nút bấm đẹp, hiện đại
Bố cục rõ ràng, dễ nhìn
# ra kết quả 
<style>
  body {
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
    background: #f5f5f7;
    color: #1d1d1f;
  }

  /* Banner */
  select {
    padding: 6px 10px;
    border-radius: 6px;
    border: 1px solid #ccc;
    font-size: 14px;
  }

  hr {
    border: none;
    border-top: 1px solid #e5e5e5;
    margin: 10px 0;
  }

  /* Navbar */
  a {
    text-decoration: none;
    color: #1d1d1f;
    font-size: 13px;
    transition: 0.3s;
  }

  a:hover {
    color: #0071e3;
  }

  /* Hero */
  h1 {
    font-size: 58px;
    margin-top: 50px;
    margin-bottom: 10px;
    font-weight: 600;
    letter-spacing: -1px;
  }

  p {
    font-size: 22px;
    color: #6e6e73;
    margin-top: 0;
  }

  /* Buttons */
  button {
    padding: 10px 22px;
    border-radius: 22px;
    font-size: 14px;
    cursor: pointer;
    transition: all 0.3s ease;
  }

  /* Learn more */
  button:first-of-type {
    background: linear-gradient(90deg, #0071e3, #42a1ff);
    color: white;
    border: none;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  }

  /* Buy */
  button:last-of-type {
    background: transparent;
    border: 1px solid #0071e3;
    color: #0071e3;
  }

  /* Hover effects */
  button:hover {
    transform: scale(1.05);
    opacity: 0.9;
  }

  /* Image */
  img {
    margin-top: 40px;
    border-radius: 14px;
    transition: transform 0.4s ease;
  }

  img:hover {
    transform: scale(1.03);
  }

  /* Responsive */
  @media (max-width: 768px) {
    h1 {
      font-size: 36px;
    }

    p {
      font-size: 18px;
    }

    img {
      width: 90%;
    }
  }
</style>
