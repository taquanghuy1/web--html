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
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>MacBook Neo</title>
  <style>
    /* Body */
    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, sans-serif;
      background: linear-gradient(to bottom, #f5f5f7, #ffffff);
      color: #1d1d1f;
      text-align: center;
    }

    hr {
      border: none;
      border-top: 1px solid #eee;
      margin: 20px 0;
    }

    /* Navbar */
    a {
      text-decoration: none;
      color: #1d1d1f;
      font-size: 14px;
      transition: 0.3s;
    }
    a:hover {
      color: #0071e3;
    }

    /* Title & description */
    h1 {
      font-size: 60px;
      margin: 40px 0 10px 0;
      font-weight: 600;
      letter-spacing: -1px;
    }
    p {
      font-size: 22px;
      color: #6e6e73;
    }

    /* Buttons */
    button {
      padding: 12px 28px;
      border-radius: 28px;
      font-size: 14px;
      margin: 10px;
      cursor: pointer;
      border: none;
      transition: 0.3s;
      backdrop-filter: blur(6px);
    }
    button:first-child {
      background: linear-gradient(90deg, #0071e3, #42a1ff);
      color: white;
      box-shadow: 0 6px 20px rgba(0,0,0,0.2);
    }
    button:last-child {
      background: rgba(255,255,255,0.8);
      border: 1px solid #0071e3;
      color: #0071e3;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
    }
    button:hover {
      transform: translateY(-3px) scale(1.07);
      opacity: 0.9;
    }

    /* Image */
    img {
      margin-top: 50px;
      border-radius: 18px;
      box-shadow: 0 12px 40px rgba(0,0,0,0.25);
      transition: transform 0.4s, box-shadow 0.4s;
    }
    img:hover {
      transform: scale(1.05);
      box-shadow: 0 16px 50px rgba(0,0,0,0.35);
    }

    /* Select */
    select {
      padding: 6px 12px;
      border-radius: 6px;
      border: 1px solid #ccc;
      font-size: 14px;
      margin-right: 10px;
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
      button {
        padding: 10px 22px;
      }
    }
  </style>
</head>
<body>

  <!-- Banner -->
  <center>
    <table border="0" width="100%">
      <tr>
        <td align="center">
          Chọn quốc gia hoặc khu vực:
          <select>
            <option>Việt Nam</option>
            <option>USA</option>
          </select>
          <button>Tiếp tục</button>
        </td>
      </tr>
    </table>
  </center>

  <hr>

  <!-- Navbar -->
  <center>
    <table border="0">
      <tr>
        <td><a href="#">Store</a></td>
        <td>&nbsp;&nbsp;</td>
        <td><a href="#">Mac</a></td>
        <td>&nbsp;&nbsp;</td>
        <td><a href="#">iPad</a></td>
        <td>&nbsp;&nbsp;</td>
        <td><a href="#">iPhone</a></td>
        <td>&nbsp;&nbsp;</td>
        <td><a href="#">Watch</a></td>
        <td>&nbsp;&nbsp;</td>
        <td><a href="#">AirPods</a></td>
        <td>&nbsp;&nbsp;</td>
        <td><a href="#">Support</a></td>
      </tr>
    </table>
  </center>

  <hr>

  <!-- Hero -->
  <center>
    <h1>MacBook Neo</h1>
    <p>Amazing Mac. Surprising price.</p>

    <p>
      <button>Learn more</button>
      <button>Buy</button>
    </p>

    <img src="https://www.apple.com/v/macbook-air/y/images/overview/design/design_hero_static__e56c1v71mr6u_large.png" alt="MacBook" width="600">
  </center>

</body>
</html>
