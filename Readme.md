# AI sử dụng chat GPT 
# Prompt đã sử dụng Hãy viết CSS cho một trang HTML (dùng table và thẻ center, không thay đổi HTML) để giao diện giống landing page Apple với các yêu cầu sau:
# Kết quả
```
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
```

