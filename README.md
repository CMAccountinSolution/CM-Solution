<!doctype html>
<html lang="si">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CM Solutions | Professional Digital & Business Services</title>
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
      rel="stylesheet"
    />
    <style>
      :root {
        --primary: #0f172a;
        --accent: #2563eb;
        --whatsapp: #25d366;
        --call: #f97316;
        --bg: #f8fafc;
        --text-dark: #0f172a;
        --text-muted: #64748b;
        --border-yellow: #eab308;
        --radius: 16px;
      }

      * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: "Poppins", sans-serif;
      }

      body {
        background-color: var(--bg);
        color: var(--text-dark);
        line-height: 1.6;
      }

      header {
        background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
        color: white;
        padding: 4rem 1.5rem;
        text-align: center;
        border-bottom-left-radius: 30px;
        border-bottom-right-radius: 30px;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
      }

      header h1 {
        font-size: 2.8rem;
        font-weight: 700;
        margin-bottom: 0.5rem;
        background: linear-gradient(to right, #ffffff, #93c5fd);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
      }

      header p {
        color: #94a3b8;
        font-size: 1.15rem;
        font-weight: 300;
      }

      .contact-container {
        display: flex;
        justify-content: center;
        gap: 15px;
        margin-top: 2rem;
        flex-wrap: wrap;
      }

      .btn {
        padding: 12px 28px;
        border-radius: 50px;
        text-decoration: none;
        color: white;
        font-weight: 600;
        font-size: 0.95rem;
        display: inline-flex;
        align-items: center;
        gap: 8px;
        transition: all 0.3s ease;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
      }

      .btn-whatsapp {
        background-color: var(--whatsapp);
      }
      .btn-whatsapp:hover {
        background-color: #20ba5a;
        transform: translateY(-2px);
      }
      .btn-call {
        background-color: var(--call);
      }
      .btn-call:hover {
        background-color: #ea580c;
        transform: translateY(-2px);
      }

      .container {
        max-width: 1200px;
        margin: 3rem auto;
        padding: 0 1.5rem;
      }

      .section-header {
        text-align: center;
        margin-bottom: 2.5rem;
      }

      .section-header h2 {
        font-size: 2rem;
        color: var(--primary);
        font-weight: 700;
      }

      .section-header p {
        color: var(--text-muted);
      }

      .services-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
        gap: 1.8rem;
      }

      /* All Service Cards Highlighted Yellow */
      .service-card {
        background-color: #fef08a !important; /* Soft Bright Yellow */
        border: 2px solid var(--border-yellow) !important;
        border-radius: var(--radius);
        overflow: hidden;
        box-shadow: 0 8px 20px rgba(234, 179, 8, 0.25);
        transition: all 0.3s ease;
      }

      .service-card:hover {
        transform: translateY(-3px);
        box-shadow: 0 12px 25px rgba(234, 179, 8, 0.4);
      }

      .card-header {
        padding: 1.4rem 1.6rem;
        background-color: #fef08a !important;
        cursor: pointer;
        display: flex;
        justify-content: space-between;
        align-items: center;
        user-select: none;
      }

      .card-header h3 {
        font-size: 1.1rem;
        font-weight: 600;
        color: var(--primary);
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        gap: 6px;
      }

      .click-badge {
        display: inline-block;
        background-color: #dc2626;
        color: white;
        font-size: 0.72rem;
        font-weight: 700;
        padding: 3px 8px;
        border-radius: 20px;
        animation: pulse 1.5s infinite;
      }

      @keyframes pulse {
        0% {
          transform: scale(1);
        }
        50% {
          transform: scale(1.08);
        }
        100% {
          transform: scale(1);
        }
      }

      .arrow-icon {
        font-size: 0.8rem;
        color: var(--primary);
        background-color: #fef9c3;
        border: 1px solid #fde047;
        width: 28px;
        height: 28px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 50%;
        transition: transform 0.3s ease;
      }

      .card-body {
        display: none;
        padding: 1.5rem 1.6rem;
        background-color: #fffde7;
        border-top: 1px solid #fef08a;
      }

      .service-card.active .card-body {
        display: block;
      }

      .service-card.active .arrow-icon {
        transform: rotate(180deg);
        background-color: var(--primary);
        color: white;
      }

      .service-list {
        list-style: none;
        margin-bottom: 1.2rem;
      }

      .service-list li {
        padding: 0.55rem 0;
        border-bottom: 1px dashed #fef08a;
        font-size: 0.95rem;
        color: #475569;
        display: flex;
        align-items: center;
      }

      .service-list li::before {
        content: "•";
        color: var(--accent);
        font-weight: bold;
        font-size: 1.2rem;
        margin-right: 10px;
      }

      .price-tag {
        padding: 0.8rem 1.2rem;
        background: linear-gradient(135deg, #eff6ff 0%, #dbeafe 100%);
        color: var(--accent);
        font-weight: 600;
        text-align: center;
        border-radius: 12px;
        font-size: 0.95rem;
        border: 1px solid #bfdbfe;
      }

      footer {
        text-align: center;
        padding: 2.5rem 1rem;
        margin-top: 4rem;
        background-color: var(--primary);
        color: #64748b;
        font-size: 0.9rem;
      }
    </style>
  </head>
  <body>
    <header>
      <h1>CM Solutions</h1>
      <p>Your Trusted Partner for Professional Digital & Business Solutions</p>

      <div class="contact-container">
        <a
          href="https://wa.me/94713306364"
          class="btn btn-whatsapp"
          target="_blank"
        >
          WhatsApp: 071 330 6364
        </a>
        <a href="tel:+94713306364" class="btn btn-call">
          Call Now: 071 330 6364
        </a>
      </div>
    </header>

    <div class="container">
      <div class="section-header">
        <h2>Our Services</h2>
        <p>Select a category below to explore our services & pricing</p>
      </div>

      <div class="services-grid">
        <!-- 1. Typing & Document Services -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              ⌨️ Typing & Document Services
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Sinhala Typing</li>
              <li>English Typing</li>
              <li>Sinhala / English Typing</li>
              <li>Handwritten → Word</li>
              <li>PDF → Word</li>
              <li>Image → Word</li>
              <li>PDF → Excel</li>
              <li>Assignment Typing</li>
              <li>Business Letter Typing</li>
              <li>Application / Official Letter Typing</li>
              <li>Document Formatting</li>
              <li>Report Formatting</li>
            </ul>
            <div class="price-tag">Starting from Rs. 100 / page</div>
          </div>
        </div>

        <!-- 2. Excel & Data Entry Services -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              📊 Excel & Data Entry
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Data Entry</li>
              <li>Excel Data Entry</li>
              <li>Excel Table Creation</li>
              <li>Excel Formatting</li>
              <li>Excel Formulas</li>
              <li>Attendance Sheets</li>
              <li>Salary Sheets</li>
              <li>Stock Sheets</li>
              <li>Sales Sheets</li>
              <li>Expense Sheets</li>
              <li>Invoice Data Entry</li>
              <li>Product Data Entry</li>
              <li>Online Form Filling</li>
              <li>Data Collection</li>
            </ul>
            <div class="price-tag">Starting from Rs. 500</div>
          </div>
        </div>

        <!-- 3. CV & Professional Documents -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              📄 CV & Professional Documents
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Basic CV</li>
              <li>Professional CV</li>
              <li>CV Formatting</li>
              <li>Cover Letter</li>
              <li>Job Application</li>
              <li>Business Letters</li>
              <li>Official Documents</li>
              <li>Professional Reports</li>
            </ul>
            <div class="price-tag">Starting from Rs. 500</div>
          </div>
        </div>

        <!-- 4. Graphic Design -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              🎨 Graphic Design
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Canva Posters</li>
              <li>Facebook Posts</li>
              <li>Social Media Designs</li>
              <li>Business Cards</li>
              <li>Invitation Cards</li>
              <li>Certificates</li>
              <li>School Notices</li>
              <li>Menus</li>
              <li>Flyers</li>
              <li>Basic Logos</li>
            </ul>
            <div class="price-tag">Starting from Rs. 300</div>
          </div>
        </div>

        <!-- 5. Accounting & Bookkeeping -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              📈 Accounting & Bookkeeping
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Sales Recording</li>
              <li>Expense Recording</li>
              <li>Cash Book</li>
              <li>Basic Bookkeeping</li>
              <li>Monthly Accounts</li>
              <li>Stock Records</li>
              <li>Invoice Preparation</li>
              <li>Excel Accounting Sheets</li>
              <li>Basic Financial Reports</li>
            </ul>
            <div class="price-tag">Starting from Rs. 1,500</div>
          </div>
        </div>

        <!-- 6. Online & Digital Services -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              🌐 Online & Digital Services
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Online Form Filling</li>
              <li>Email Preparation</li>
              <li>Online Applications</li>
              <li>Web Research</li>
              <li>Data Collection</li>
              <li>Product Listing</li>
              <li>PDF Merge / Split</li>
              <li>PDF Conversion</li>
              <li>Document Scanning</li>
              <li>File Conversion</li>
            </ul>
            <div class="price-tag">Starting from Rs. 100</div>
          </div>
        </div>

        <!-- 7. Translation Services -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              🌎 Translation Services
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>Sinhala → English</li>
              <li>English → Sinhala</li>
              <li>Sinhala Document Translation</li>
              <li>English Document Translation</li>
              <li>Business Translation</li>
              <li>General Document Translation</li>
            </ul>
            <div class="price-tag">Starting from Rs. 300 / page</div>
          </div>
        </div>

        <!-- 8. Presentation Services -->
        <div class="service-card">
          <div class="card-header" onclick="toggleCard(this)">
            <h3>
              📊 Presentation Services
              <span class="click-badge">👈 Click This</span>
            </h3>
            <span class="arrow-icon">▼</span>
          </div>
          <div class="card-body">
            <ul class="service-list">
              <li>PowerPoint Presentations</li>
              <li>School Presentations</li>
              <li>Business Presentations</li>
              <li>Training Presentations</li>
              <li>Presentation Formatting</li>
              <li>Charts & Tables</li>
            </ul>
            <div class="price-tag">Starting from Rs. 1,000</div>
          </div>
        </div>
      </div>
    </div>

    <footer>
      <p>&copy; 2026 <strong>CM Solutions</strong>. All Rights Reserved.</p>
    </footer>

    <script>
      function toggleCard(headerElement) {
        var card = headerElement.parentElement;
        card.classList.toggle("active");
      }
    </script>
  </body>
</html>

