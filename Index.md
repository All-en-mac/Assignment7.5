HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SaaSify — Modern Flexbox Landing Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- SECTION 1: Navigation Bar -->
    <header class="navbar-container">
        <div class="logo">
            <a href="#">SaaSify</a>
        </div>
        <nav>
            <ul class="nav-links">
                <li><a href="#features">Features</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="nav-btn">
            <a href="#cta" class="btn btn-secondary">Get Started</a>
        </div>
    </header>

    <!-- SECTION 2: Hero Section -->
    <section class="hero-section">
        <div class="hero-container">
            <div class="hero-text">
                <span class="badge">Next-Gen Analytics</span>
                <h1>Scale Your Business With Intelligence</h1>
                <p>Automate workflows, track real-time metrics, and empower your team to reach new heights with our all-in-one SaaS platform.</p>
                <div class="hero-actions">
                    <a href="#cta" class="btn btn-primary">Start Free Trial</a>
                    <a href="#features" class="btn btn-outline">Learn More</a>
                </div>
            </div>
            <div class="hero-image">
                <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&w=800&q=80" alt="Dashboard Illustration">
            </div>
        </div>
    </section>

    <!-- SECTION 3: 3 Feature Cards Section -->
    <section id="features" class="features-section">
        <div class="section-header">
            <h2>Powerful Features Built For Growth</h2>
            <p>Everything you need to manage, scale, and optimize your digital workflows.</p>
        </div>

        <div class="features-container">
            <!-- Feature Card 1 -->
            <div class="feature-card">
                <div class="feature-icon">⚡</div>
                <h3>Lightning Fast</h3>
                <p>Optimized architecture ensures sub-second load times and seamless real-time data synchronization across all devices.</p>
            </div>

            <!-- Feature Card 2 -->
            <div class="feature-card">
                <div class="feature-icon">🔒</div>
                <h3>Enterprise Security</h3>
                <p>Bank-grade encryption, role-based access control, and absolute compliance keep your corporate data fully protected.</p>
            </div>

            <!-- Feature Card 3 -->
            <div class="feature-card">
                <div class="feature-icon">📈</div>
                <h3>Advanced Analytics</h3>
                <p>Gain deep operational insights with customizable reporting dashboards tailored to drive intelligent decision-making.</p>
            </div>
        </div>
    </section>

    <!-- SECTION 4: Call-to-Action (CTA) Section -->
    <section id="cta" class="cta-section">
        <div class="cta-container">
            <h2>Ready to Transform Your Workflow?</h2>
            <p>Join thousands of growing companies scaling their productivity with SaaSify today.</p>
            <a href="#" class="btn btn-primary-light">Get Started for Free</a>
        </div>
    </section>

    <!-- SECTION 5: Footer -->
    <footer class="footer-section">
        <div class="footer-container">
            <div class="footer-col">
                <h3>SaaSify</h3>
                <p>Empowering global teams with scalable tools and modern workflow architecture.</p>
            </div>
            <div class="footer-col">
                <h4>Product</h4>
                <ul>
                    <li><a href="#">Features</a></li>
                    <li><a href="#">Security</a></li>
                    <li><a href="#">Roadmap</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>Company</h4>
                <ul>
                    <li><a href="#">About Us</a></li>
                    <li><a href="#">Careers</a></li>
                    <li><a href="#">Press Kit</a></li>
                </ul>
            </div>
            <div class="footer-col">
                <h4>Legal</h4>
                <ul>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms of Service</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2026 SaaSify Inc. All rights reserved. Built with HTML & CSS Flexbox.</p>
        </div>
    </footer>

</body>
</html>


CSS
/* ==========================================
   Global Resets & Typography Variables
   ========================================== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: #f8fafc;
    color: #1e293b;
    line-height: 1.6;
}

/* ==========================================
   1. Navbar Section (Flexbox)
   ========================================== */
.navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #ffffff;
    padding: 1.25rem 5%;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo a {
    font-size: 1.5rem;
    font-weight: 700;
    color: #0f172a;
    text-decoration: none;
}

.nav-links {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-links a {
    text-decoration: none;
    color: #64748b;
    font-weight: 500;
    transition: color 0.2s ease;
}

.nav-links a:hover {
    color: #2563eb;
}

/* ==========================================
   2. Hero Section (Side-by-Side Flexbox)
   ========================================== */
.hero-section {
    padding: 6rem 5%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #f8fafc 0%, #edf2f7 100%);
}

.hero-container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    gap: 4rem;
    max-width: 1200px;
    width: 100%;
}

.hero-text {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.badge {
    background-color: #dbeafe;
    color: #1d4ed8;
    font-size: 0.8rem;
    font-weight: 600;
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    margin-bottom: 1.25rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
}

.hero-text h1 {
    font-size: 3rem;
    font-weight: 800;
    color: #0f172a;
    line-height: 1.2;
    margin-bottom: 1.25rem;
}

.hero-text p {
    font-size: 1.125rem;
    color: #475569;
    margin-bottom: 2rem;
}

.hero-actions {
    display: flex;
    gap: 1rem;
}

.hero-image {
    flex: 1;
    display: flex;
    justify-content: center;
}

.hero-image img {
    width: 100%;
    max-width: 550px;
    border-radius: 12px;
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
}

/* ==========================================
   3. Feature Cards Section (Responsive Row)
   ========================================== */
.features-section {
    padding: 6rem 5%;
    background-color: #ffffff;
}

.section-header {
    text-align: center;
    max-width: 600px;
    margin: 0 auto 4rem auto;
}

.section-header h2 {
    font-size: 2.25rem;
    font-weight: 700;
    color: #0f172a;
    margin-bottom: 0.75rem;
}

.section-header p {
    color: #64748b;
    font-size: 1.1rem;
}

.features-container {
    display: flex;             /* Flexbox activation */
    flex-wrap: wrap;           /* Wrap cards on smaller widths */
    justify-content: center;   /* Center align row items */
    gap: 2rem;                 /* Consistent gap spacing */
    max-width: 1200px;
    margin: 0 auto;
}

.feature-card {
    flex: 1 1 300px;           /* Grow, shrink, base width for responsive wrapping */
    max-width: 380px;
    background-color: #f8fafc;
    border: 1px solid #e2e8f0;
    padding: 2.5rem 2rem;
    border-radius: 12px;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
    display: flex;
    flex-direction: column;
}

.feature-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 12px 25px rgba(0, 0, 0, 0.08);
}

.feature-icon {
    font-size: 2rem;
    background-color: #dbeafe;
    color: #2563eb;
    width: 60px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px;
    margin-bottom: 1.5rem;
}

.feature-card h3 {
    font-size: 1.25rem;
    font-weight: 600;
    color: #0f172a;
    margin-bottom: 0.75rem;
}

.feature-card p {
    color: #64748b;
    font-size: 0.95rem;
}

/* ==========================================
   4. Call-to-Action Section
   ========================================== */
.cta-section {
    padding: 5rem 5%;
    background-color: #2563eb;
    color: #ffffff;
    text-align: center;
}

.cta-container {
    max-width: 700px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.cta-container h2 {
    font-size: 2.5rem;
    font-weight: 800;
    margin-bottom: 1rem;
}

.cta-container p {
    font-size: 1.125rem;
    opacity: 0.9;
    margin-bottom: 2rem;
}

/* ==========================================
   5. Footer Section
   ========================================== */
.footer-section {
    background-color: #0f172a;
    color: #94a3b8;
    padding: 4rem 5% 2rem 5%;
}

.footer-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 3rem;
    max-width: 1200px;
    margin: 0 auto 3rem auto;
}

.footer-col {
    flex: 1 1 200px;
    display: flex;
    flex-direction: column;
}

.footer-col h3, .footer-col h4 {
    color: #ffffff;
    margin-bottom: 1.25rem;
}

.footer-col h3 {
    font-size: 1.5rem;
}

.footer-col p {
    font-size: 0.9rem;
}

.footer-col ul {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
}

.footer-col ul li a {
    text-decoration: none;
    color: #94a3b8;
    font-size: 0.9rem;
    transition: color 0.2s ease;
}

.footer-col ul li a:hover {
    color: #ffffff;
}

.footer-bottom {
    max-width: 1200px;
    margin: 0 auto;
    border-top: 1px solid #1e293b;
    padding-top: 1.5rem;
    text-align: center;
    font-size: 0.85rem;
}

/* ==========================================
   Shared Button Styles
   ========================================== */
.btn {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.2s ease;
    text-align: center;
}

.btn-primary {
    background-color: #2563eb;
    color: #ffffff;
}

.btn-primary:hover {
    background-color: #1d4ed8;
}

.btn-primary-light {
    background-color: #ffffff;
    color: #2563eb;
}

.btn-primary-light:hover {
    background-color: #f1f5f9;
}

.btn-secondary {
    color: #2563eb;
    background-color: transparent;
    padding: 0.5rem 1rem;
}

.btn-secondary:hover {
    background-color: #f1f5f9;
}

.btn-outline {
    background-color: transparent;
    color: #475569;
    border: 1px solid #cbd5e1;
}

.btn-outline:hover {
    background-color: #f1f5f9;
    color: #0f172a;
}

/* ==========================================
   Responsive Media Queries (Mobile Adaptation)
   ========================================== */
@media (max-width: 900px) {
    .navbar-container {
        flex-direction: column;
        gap: 1rem;
        padding: 1rem;
    }

    .nav-links {
        gap: 1.25rem;
    }

    .hero-container {
        flex-direction: column;
        text-align: center;
        gap: 2.5rem;
    }

    .hero-text {
        align-items: center;
    }

    .hero-text h1 {
        font-size: 2.25rem;
    }

    .hero-actions {
        justify-content: center;
        flex-wrap: wrap;
    }

    .cta-container h2 {
        font-size: 2rem;
    }
}