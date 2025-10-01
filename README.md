<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Công ty Bảo Vệ Thăng Long</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    :root {
      --navy: #001f3f;
      --gray: #f5f5f5;
      --white: #ffffff;
      --accent: #0077ff;
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: Arial, Helvetica, sans-serif;
      line-height: 1.6;
      color: #333;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    img {
      max-width: 100%;
      display: block;
    }

    /* Header */
    header {
      background: var(--navy);
      color: var(--white);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 2rem;
      flex-wrap: wrap;
    }
    header .logo {
      font-size: 1.5rem;
      font-weight: bold;
      letter-spacing: 1px;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 1.2rem;
    }
    nav a {
      color: var(--white);
      transition: color .3s;
    }
    nav a:hover {
      color: var(--accent);
    }

    /* Banner */
    .banner {
      background: url("https://images.unsplash.com/photo-1551641506-ee5bf4cb45f1?auto=format&fit=crop&w=1350&q=80") center/cover no-repeat;
      height: 60vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: var(--white);
      position: relative;
    }
    .banner::after {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(0, 31, 63, .65);
    }
    .banner h1 {
      font-size: 2.2rem;
      z-index: 2;
      position: relative;
      max-width: 800px;
      padding: 0 1rem;
    }

    /* Sections */
    section {
      padding: 4rem 2rem;
      max-width: 1100px;
      margin: auto;
    }
    h2 {
      text-align: center;
      margin-bottom: 2rem;
      color: var(--navy);
      font-size: 2rem;
    }

    /* About */
    .about p {
      margin-bottom: 1rem;
      text-align: justify;
    }

    /* Services */
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 1.5rem;
    }
    .service-card {
      background: var(--gray);
      padding: 1.5rem 1rem;
      border-radius: 6px;
      text-align: center;
      transition: transform .3s;
    }
    .service-card:hover {
      transform: translateY(-5px);
    }
    .service-card h3 {
      margin-bottom: .5rem;
      color: var(--navy);
    }

    /* Pricing */
    .pricing-flex {
      display: flex;
      gap: 2rem;
      justify-content: center;
      flex-wrap: wrap;
    }
    .price-card {
      background: var(--gray);
      border: 2px solid var(--navy);
      border-radius: 8px;
      padding: 2rem;
      width: 280px;
      text-align: center;
    }
    .price-card h3 {
      margin-bottom: 1rem;
      color: var(--navy);
    }
    .price-card .price {
      font-size: 2rem;
      color: var(--accent);
      margin-bottom: 1rem;
    }

    /* Contact */
    .contact-info {
      text-align: center;
      margin-bottom: 2rem;
    }
    .contact-info p {
      margin: .5rem 0;
    }
    .cta-button {
      display: inline-block;
      background: var(--navy);
      color: var(--white);
      padding: .9rem 2rem;
      border-radius: 4px;
      transition: background .3s;
    }
    .cta-button:hover {
      background: var(--accent);
    }

    /* Footer */
    footer {
      background: var(--navy);
      color: var(--white);
      text-align: center;
      padding: 1.5rem 1rem;
      font-size: .9rem;
    }

    /* Responsive tweaks */
    @media (max-width: 600px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }
      nav ul {
        flex-direction: column;
        margin-top: 1rem;
      }
      .banner h1 {
        font-size: 1.6rem;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="logo">Bảo Vệ Thăng Long</div>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#pricing">Pricing</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Banner -->
  <section id="home" class="banner">
    <h1>Trusted – Professional – Dedicated Security Services</h1>
  </section>

  <!-- About -->
  <section id="about" class="about">
    <h2>About Us</h2>
    <p>Công ty Bảo Vệ Thăng Long tự hào là đơn vị cung cấp dịch vụ bảo vệ chuyên nghiệp hàng đầu, uy tín trên thị trường. Với đội ngũ nhân viên được tuyển chọn kỹ lưỡng, huấn luyện bài bản và giàu kinh nghiệm, chúng tôi cam kết mang lại sự an toàn tuyệt đối cho con người, tài sản và thông tin của khách hàng.</p>
    <p><strong>Strengths:</strong> Đội ngũ bảo vệ chuyên nghiệp, quy trình quản lý chặt chẽ, công nghệ hỗ trợ hiện đại, chi phí hợp lý.</p>
    <p><strong>Commitments:</strong> An toàn 24/7, phản ứng nhanh, bảo mật thông tin, hợp đồng minh bạch, hỗ trợ khách hàng mọi lúc.</p>
  </section>

  <!-- Services -->
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="services-grid">
      <div class="service-card">
        <h3>Company Security</h3>
        <p>Bảo vệ nhà máy, văn phòng, khu công nghiệp.</p>
      </div>
      <div class="service-card">
        <h3>Construction Site Security</h3>
        <p>Bảo vệ công trường, thiết bị, vật liệu xây dựng.</p>
      </div>
      <div class="service-card">
        <h3>Event Security</h3>
        <p>Đảm bảo an ninh cho hội nghị, concert, lễ hội.</p>
      </div>
      <div class="service-card">
        <h3>Building Security</h3>
        <p>Bảo vệ chung cư, tòa nhà, trung tâm thương mại.</p>
      </div>
      <div class="service-card">
        <h3>Fixed Target Security</h3>
        <p>Can gác ngân hàng, showroom, cửa hàng trọng điểm.</p>
      </div>
    </div>
  </section>

  <!-- Pricing -->
  <section id="pricing" class="pricing">
    <h2>Packages & Pricing</h2>
    <div class="pricing-flex">
      <div class="price-card">
        <h3>12-hour shift</h3>
        <div class="price">7.5 million VND/month</div>
        <p>Phù hợp cửa hàng, văn phòng nhỏ.</p>
      </div>
      <div class="price-card">
        <h3>24-hour shift<br><small>(day work, night sleep)</small></h3>
        <div class="price">10 million VND/month</div>
        <p>Phù hợp kho bãi, công trường, tòa nhà.</p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <div class="contact-info">
      <p><strong>Phone:</strong> 0901 234 567</p>
      <p><strong>Zalo:</strong> 0901 234 567</p>
      <p><strong>Email:</strong> info@baovethanglong.vn</p>
      <p><strong>Address:</strong> 123 Đường Thăng Long, Quận Tây Hồ, TP. Hà Nội</p>
    </div>
    <div style="text-align:center;">
      <a href="tel:0901234567" class="cta-button">Contact Now</a>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    © 2025 Công ty Bảo Vệ Thăng Long – "Strong Security – Lasting Trust"
  </footer>

</body>
</html>
