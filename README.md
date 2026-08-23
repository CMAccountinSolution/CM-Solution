<!doctype html>
<html lang="si">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CM Solutions | Professional Digital & Business Solutions</title>
    <!-- Google Fonts -->
    <link
      href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&family=Noto+Sans+Sinhala:wght@400;500;600;700&display=swap"
      rel="stylesheet"
    />
    <!-- FontAwesome Icons -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
    />

    <style>
      :root {
        --primary: #0f172a;
        --primary-light: #1e293b;
        --accent: #3b82f6;
        --accent-glow: rgba(59, 130, 246, 0.4);
        --whatsapp: #25d366;
        --call: #ff6b00;
        --bg: #090d16;
        --card-bg: rgba(30, 41, 59, 0.7);
        --card-hover: rgba(51, 65, 85, 0.8);
        --text-main: #f8fafc;
        --text-muted: #94a3b8;
        --border: rgba(255, 255, 255, 0.1);
        --gold: #f59e0b;
        --radius-lg: 24px;
        --radius-md: 16px;
      }

      * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: "Outfit", "Noto Sans Sinhala", sans-serif;
        scroll-behavior: smooth;
      }

      body {
        background-color: var(--bg);
        color: var(--text-main);
        line-height: 1.6;
        overflow-x: hidden;
        background-image:
          radial-gradient(
            at 0% 0%,
            rgba(59, 130, 246, 0.15) 0px,
            transparent 50%
          ),
          radial-gradient(
            at 100% 100%,
            rgba(245, 158, 11, 0.1) 0px,
            transparent 50%
          );
        background-attachment: fixed;
        padding-bottom: 80px; /* Space for mobile floating bar */
      }

      /* Top Bar */
      .top-nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.2rem 2rem;
        max-width: 1300px;
        margin: 0 auto;
        border-bottom: 1px solid var(--border);
      }

      .brand {
        display: flex;
        align-items: center;
        gap: 12px;
        text-decoration: none;
      }

      .brand-logo {
        width: 45px;
        height: 45px;
        background: linear-gradient(135deg, var(--accent), #1d4ed8);
        border-radius: 12px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-weight: 800;
        font-size: 1.3rem;
        box-shadow: 0 0 15px var(--accent-glow);
      }

      .brand-text h2 {
        color: var(--text-main);
        font-size: 1.4rem;
        font-weight: 700;
        letter-spacing: 0.5px;
      }

      .brand-text p {
        color: var(--text-muted);
        font-size: 0.75rem;
      }

      /* Hero Section */
      .hero {
        text-align: center;
        padding: 4rem 1.5rem 3rem;
        max-width: 900px;
        margin: 0 auto;
        position: relative;
      }

      .badge {
        display: inline-flex;
        align-items: center;
        gap: 8px;
        background: rgba(59, 130, 246, 0.1);
        border: 1px solid rgba(59, 130, 246, 0.3);
        color: var(--accent);
        padding: 6px 16px;
        border-radius: 50px;
        font-size: 0.85rem;
        font-weight: 600;
        margin-bottom: 1.5rem;
      }

      .hero h1 {
        font-size: 3rem;
        font-weight: 800;
        line-height: 1.2;
        margin-bottom: 1.2rem;
        background: linear-gradient(135deg, #ffffff 30%, #94a3b8 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }

      .hero h1 span {
        background: linear-gradient(135deg, #60a5fa, #3b82f6);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }

      .hero p {
        color: var(--text-muted);
        font-size: 1.1rem;
        margin-bottom: 2rem;
      }

      /* Action Buttons */
      .cta-group {
        display: flex;
        justify-content: center;
        gap: 16px;
        flex-wrap: wrap;
      }

      .btn {
        padding: 14px 32px;
        border-radius: 50px;
        text-decoration: none;
        font-weight: 600;
        font-size: 1rem;
        display: inline-flex;
        align-items: center;
        gap: 10px;
        transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        cursor: pointer;
        border: none;
      }

      .btn-whatsapp {
        background: linear-gradient(135deg, #25d366, #128c7e);
        color: white;
        box-shadow: 0 4px 20px rgba(37, 211, 102, 0.3);
      }

      .btn-whatsapp:hover {
        transform: translateY(-3px);
        box-shadow: 0 8px 25px rgba(37, 211, 102, 0.5);
      }

      .btn-call {
        background: linear-gradient(135deg, #ff6b00, #ff8800);
        color: white;
        box-shadow: 0 4px 20px rgba(255, 107, 0, 0.3);
      }

      .btn-call:hover {
        transform: translateY(-3px);
        box-shadow: 0 8px 25px rgba(255, 107, 0, 0.5);
      }

      /* Search & Filter Controls */
      .controls-container {
        max-width: 1200px;
        margin: 2rem auto;
        padding: 0 1.5rem;
      }

      .search-box {
        position: relative;
        max-width: 600px;
        margin: 0 auto 2rem;
      }

      .search-box input {
        width: 100%;
        padding: 16px 20px 16px 50px;
        background: var(--card-bg);
        border: 1px solid var(--border);
        border-radius: 50px;
        color: white;
        font-size: 1rem;
        backdrop-filter: blur(10px);
        outline: none;
        transition: all 0.3s ease;
      }

      .search-box input:focus {
        border-color: var(--accent);
        box-shadow: 0 0 20px var(--accent-glow);
      }

      .search-box i {
        position: absolute;
        left: 20px;
        top: 50%;
        transform: translateY(-50%);
        color: var(--text-muted);
      }

      /* Filter Tabs */
      .filter-tabs {
        display: flex;
        justify-content: center;
        gap: 10px;
        flex-wrap: wrap;
        margin-bottom: 2.5rem;
      }

      .tab-btn {
        padding: 8px 20px;
        background: rgba(255, 255, 255, 0.05);
        border: 1px solid var(--border);
        border-radius: 30px;
        color: var(--text-muted);
        font-size: 0.9rem;
        cursor: pointer;
        transition: all 0.3s ease;
      }

      .tab-btn.active,
      .tab-btn:hover {
        background: var(--accent);
        color: white;
        border-color: var(--accent);
        box-shadow: 0 0 15px var(--accent-glow);
      }

      /* Services Grid */
      .services-grid {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 1.5rem;
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
        gap: 2rem;
      }

      .service-card {
        background: var(--card-bg);
        border: 1px solid var(--border);
        border-radius: var(--radius-lg);
        padding: 2rem;
        backdrop-filter: blur(12px);
        transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        position: relative;
        overflow: hidden;
      }

      .service-card::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 4px;
        background: linear-gradient(90deg, var(--accent), var(--gold));
        opacity: 0;
        transition: opacity 0.3s ease;
      }

      .service-card:hover {
        transform: translateY(-8px);
        background: var(--card-hover);
        border-color: rgba(255, 255, 255, 0.2);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
      }

      .service-card:hover::before {
        opacity: 1;
      }

      .card-icon {
        width: 55px;
        height: 55px;
        background: rgba(59, 130, 246, 0.1);
        border-radius: var(--radius-md);
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 1.5rem;
        color: var(--accent);
        margin-bottom: 1.5rem;
        border: 1px solid rgba(59, 130, 246, 0.2);
      }

      .card-title {
        font-size: 1.3rem;
        font-weight: 700;
        margin-bottom: 1rem;
        color: var(--text-main);
      }

      .service-list {
        list-style: none;
        margin-bottom: 1.8rem;
      }

      .service-list li {
        font-size: 0.95rem;
        color: var(--text-muted);
        margin-bottom: 0.6rem;
        display: flex;
        align-items: center;
        gap: 10px;
      }

      .service-list li i {
        color: var(--accent);
        font-size: 0.8rem;
      }

      .card-footer {
        border-top: 1px solid var(--border);
        padding-top: 1.2rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
      }

      .price-label {
        font-size: 0.8rem;
        color: var(--text-muted);
        display: block;
      }

      .price-value {
        font-size: 1.1rem;
        font-weight: 700;
        color: var(--gold);
      }

      .order-btn {
        background: rgba(255, 255, 255, 0.05);
        border: 1px solid var(--border);
        color: var(--text-main);
        padding: 8px 16px;
        border-radius: 30px;
        text-decoration: none;
        font-size: 0.85rem;
        font-weight: 600;
        transition: all 0.3s ease;
      }

      .service-card:hover .order-btn {
        background: var(--accent);
        border-color: var(--accent);
        color: white;
      }

      /* Floating Contact Bar for Mobile */
      .mobile-floating-bar {
        position: fixed;
        bottom: 20px;
        left: 50%;
        transform: translateX(-50%);
        background: rgba(15, 23, 42, 0.9);
        border: 1px solid var(--border);
        backdrop-filter: blur(15px);
        padding: 8px 16px;
        border-radius: 50px;
        display: flex;
        gap: 12px;
        z-index: 1000;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
      }

      .float-btn {
        padding: 10px 20px;
        border-radius: 30px;
        color: white;
        text-decoration: none;
        font-weight: 600;
        font-size: 0.85rem;
        display: flex;
        align-items: center;
        gap: 8px;
      }

      /* Footer */
      footer {
        text-align: center;
        padding: 4rem 1.5rem 2rem;
        border-top: 1px solid var(--border);
        margin-top: 5rem;
        color: var(--text-muted);
        font-size: 0.9rem;
      }

      footer strong {
        color: var(--text-main);
      }

      /* Responsive Design */
      @media (max-width: 768px) {
        .hero h1 {
          font-size: 2.2rem;
        }
        .top-nav {
          justify-content: center;
        }
        .cta-group {
          width: 100%;
        }
        .btn {
          width: 100%;
          justify-content: center;
        }
        .services-grid {
          grid-template-columns: 1fr;
        }
      }
    </style>
  </head>
  <body>
    <!-- Header -->
    <nav class="top-nav">
      <a href="#" class="brand">
        <div class="brand-logo">CM</div>
        <div class="brand-text">
          <h2>CM Solutions</h2>
          <p>Digital & Business Services</p>
        </div>
      </a>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
      <div class="badge">
        <i class="fa-solid fa-bolt"></i> Fast & Professional Service
      </div>
      <h1>
        ඔබේ සියලුම <span>ඩිජිටල් සහ ව්‍යාපාරික</span> අවශ්‍යතා එකම තැනකින්
      </h1>
      <p>
        ලේඛන සකස් කිරීම්, දත්ත ඇතුලත් කිරීම්, නිර්මාණකරණය ඇතුළු සියලුම සේවාවන්
        විශ්වාසවන්තව ඉටු කරවා ගන්න.
      </p>

      <div class="cta-group">
        <a
          href="https://wa.me/94764635887?text=Hi%20CM%20Solutions,%20I%20need%20more%20info"
          class="btn btn-whatsapp"
          target="_blank"
        >
          <i class="fa-brands fa-whatsapp"></i> WhatsApp: 076 463 5887
        </a>
        <a href="tel:+94764635887" class="btn btn-call">
          <i class="fa-solid fa-phone"></i> Call Now: 076 463 5887
        </a>
      </div>
    </section>

    <!-- Search & Filters -->
    <div class="controls-container">
      <div class="search-box">
        <i class="fa-solid fa-magnifying-glass"></i>
        <input
          type="text"
          id="searchInput"
          onkeyup="searchServices()"
          placeholder="ඔබට අවශ්‍ය සේවාව මෙහි සූචනය කරන්න (Search)..."
        />
      </div>

      <div class="filter-tabs">
        <button class="tab-btn active" onclick="filterCategory('all')">
          සියල්ල (All)
        </button>
        <button class="tab-btn" onclick="filterCategory('typing')">
          Typing
        </button>
        <button class="tab-btn" onclick="filterCategory('excel')">
          Excel & Data
        </button>
        <button class="tab-btn" onclick="filterCategory('cv')">
          CV & Letters
        </button>
        <button class="tab-btn" onclick="filterCategory('design')">
          Graphic Design
        </button>
        <button class="tab-btn" onclick="filterCategory('accounts')">
          Accounts
        </button>
      </div>
    </div>

    <!-- Services Grid -->
    <main class="services-grid" id="servicesContainer">
      <!-- 1. Typing Services -->
      <div class="service-card" data-category="typing">
        <div>
          <div class="card-icon"><i class="fa-solid fa-keyboard"></i></div>
          <h3 class="card-title">Typing & Documents</h3>
          <ul class="service-list">
            <li><i class="fa-solid fa-check"></i> Sinhala & English Typing</li>
            <li>
              <i class="fa-solid fa-check"></i> Handwritten / Image / PDF to
              Word
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Assignment & Report Typing
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Official Letters & Applications
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Professional Document Formatting
            </li>
          </ul>
        </div>
        <div class="card-footer">
          <div>
            <span class="price-label">ගාස්තුව ආරම්භය</span>
            <span class="price-value">Rs. 100 / page</span>
          </div>
          <a
            href="https://wa.me/94764635887?text=I%20am%20interested%20in%20Typing%20Services"
            class="order-btn"
            target="_blank"
            >Order Now</a
          >
        </div>
      </div>

      <!-- 2. Excel & Data Entry -->
      <div class="service-card" data-category="excel">
        <div>
          <div class="card-icon"><i class="fa-solid fa-file-excel"></i></div>
          <h3 class="card-title">Excel & Data Entry</h3>
          <ul class="service-list">
            <li>
              <i class="fa-solid fa-check"></i> Advanced Excel Formatting &
              Formulas
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Attendance, Salary & Stock
              Sheets
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Sales, Expense & Invoice Entry
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Online Form Filling & Web
              Research
            </li>
            <li><i class="fa-solid fa-check"></i> Bulk Data Collection</li>
          </ul>
        </div>
        <div class="card-footer">
          <div>
            <span class="price-label">ගාස්තුව ආරම්භය</span>
            <span class="price-value">Rs. 500</span>
          </div>
          <a
            href="https://wa.me/94764635887?text=I%20am%20interested%20in%20Excel%20Services"
            class="order-btn"
            target="_blank"
            >Order Now</a
          >
        </div>
      </div>

      <!-- 3. CV & Professional -->
      <div class="service-card" data-category="cv">
        <div>
          <div class="card-icon"><i class="fa-solid fa-file-user"></i></div>
          <h3 class="card-title">CV & Professional Documents</h3>
          <ul class="service-list">
            <li>
              <i class="fa-solid fa-check"></i> Professional CV & Resume Design
            </li>
            <li><i class="fa-solid fa-check"></i> Custom Cover Letters</li>
            <li><i class="fa-solid fa-check"></i> Job Applications</li>
            <li>
              <i class="fa-solid fa-check"></i> Business Proposals & Letters
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Executive Document Styling
            </li>
          </ul>
        </div>
        <div class="card-footer">
          <div>
            <span class="price-label">ගාස්තුව ආරම්භය</span>
            <span class="price-value">Rs. 500</span>
          </div>
          <a
            href="https://wa.me/94764635887?text=I%20need%20a%20Professional%20CV"
            class="order-btn"
            target="_blank"
            >Order Now</a
          >
        </div>
      </div>

      <!-- 4. Graphic Design -->
      <div class="service-card" data-category="design">
        <div>
          <div class="card-icon">
            <i class="fa-solid fa-wand-magic-sparkles"></i>
          </div>
          <h3 class="card-title">Graphic Design</h3>
          <ul class="service-list">
            <li>
              <i class="fa-solid fa-check"></i> Social Media Posts & Flyers
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Business Cards & Invitations
            </li>
            <li><i class="fa-solid fa-check"></i> Basic Logos & Menu Cards</li>
            <li>
              <i class="fa-solid fa-check"></i> School Notices & Certificates
            </li>
            <li><i class="fa-solid fa-check"></i> Canva Designs</li>
          </ul>
        </div>
        <div class="card-footer">
          <div>
            <span class="price-label">ගාස්තුව ආරම්භය</span>
            <span class="price-value">Rs. 300</span>
          </div>
          <a
            href="https://wa.me/94764635887?text=I%20need%20Graphic%20Design%20Services"
            class="order-btn"
            target="_blank"
            >Order Now</a
          >
        </div>
      </div>

      <!-- 5. Accounting -->
      <div class="service-card" data-category="accounts">
        <div>
          <div class="card-icon"><i class="fa-solid fa-chart-line"></i></div>
          <h3 class="card-title">Accounting & Bookkeeping</h3>
          <ul class="service-list">
            <li><i class="fa-solid fa-check"></i> Sales & Expense Recording</li>
            <li>
              <i class="fa-solid fa-check"></i> Cash Book & Monthly Accounts
            </li>
            <li><i class="fa-solid fa-check"></i> Stock Management Records</li>
            <li><i class="fa-solid fa-check"></i> Invoice Preparation</li>
            <li>
              <i class="fa-solid fa-check"></i> Financial Statements (Basic)
            </li>
          </ul>
        </div>
        <div class="card-footer">
          <div>
            <span class="price-label">ගාස්තුව ආරම්භය</span>
            <span class="price-value">Rs. 1,500</span>
          </div>
          <a
            href="https://wa.me/94764635887?text=I%20need%20Accounting%20Services"
            class="order-btn"
            target="_blank"
            >Order Now</a
          >
        </div>
      </div>

      <!-- 6. Online & Translation -->
      <div class="service-card" data-category="typing">
        <div>
          <div class="card-icon"><i class="fa-solid fa-language"></i></div>
          <h3 class="card-title">Translation & Digital</h3>
          <ul class="service-list">
            <li>
              <i class="fa-solid fa-check"></i> Sinhala ↔️ English Translation
            </li>
            <li>
              <i class="fa-solid fa-check"></i> Online Form Filling &
              Applications
            </li>
            <li><i class="fa-solid fa-check"></i> PDF Conversions & Merging</li>
            <li><i class="fa-solid fa-check"></i> PowerPoint Presentations</li>
            <li>
              <i class="fa-solid fa-check"></i> Document Scanning & Cleanup
            </li>
          </ul>
        </div>
        <div class="card-footer">
          <div>
            <span class="price-label">ගාස්තුව ආරම්භය</span>
            <span class="price-value">Rs. 300 / page</span>
          </div>
          <a
            href="https://wa.me/94764635887?text=I%20need%20Translation/Digital%20Services"
            class="order-btn"
            target="_blank"
            >Order Now</a
          >
        </div>
      </div>
    </main>

    <!-- Mobile Quick Navigation Floating Bar -->
    <div class="mobile-floating-bar">
      <a
        href="https://wa.me/94764635887"
        class="float-btn"
        style="background: var(--whatsapp)"
        target="_blank"
      >
        <i class="fa-brands fa-whatsapp"></i> WhatsApp
      </a>
      <a
        href="tel:+94764635887"
        class="float-btn"
        style="background: var(--call)"
      >
        <i class="fa-solid fa-phone"></i> Call
      </a>
    </div>

    <!-- Footer -->
    <footer>
      <p>&copy; 2026 <strong>CM Solutions</strong>. All Rights Reserved.</p>
      <p style="font-size: 0.8rem; margin-top: 5px">
        Designed for High-Performance Digital Services
      </p>
    </footer>

    <!-- JavaScript for Dynamic Interactions -->
    <script>
      // Search Filter Functionality
      function searchServices() {
        let input = document.getElementById("searchInput").value.toLowerCase();
        let cards = document.getElementsByClassName("service-card");

        for (let i = 0; i < cards.length; i++) {
          let cardText = cards[i].innerText.toLowerCase();
          if (cardText.includes(input)) {
            cards[i].style.display = "flex";
          } else {
            cards[i].style.display = "none";
          }
        }
      }

      // Category Tab Filter Functionality
      function filterCategory(category) {
        let cards = document.getElementsByClassName("service-card");
        let buttons = document.getElementsByClassName("tab-btn");

        // Toggle active class on buttons
        for (let btn of buttons) {
          btn.classList.remove("active");
        }
        event.currentTarget.classList.add("active");

        // Show/Hide Cards
        for (let card of cards) {
          if (
            category === "all" ||
            card.getAttribute("data-category") === category
          ) {
            card.style.display = "flex";
          } else {
            card.style.display = "none";
          }
        }
      }
    </script>
  </body>
</html>
