<html lang="en"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Miller Family Dental Care — Kokomo, IN</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet">

    <style>

        /* DESIGN TOKENS & RESPONSIVE VARIABLES */

        :root {

            --primary: #1e1b4b;       /* Deep Indigo / Slate Blue from Logo */

            --primary-light: #2e2a72;

            --accent: #52b788;        /* Teal / Mint Green from Logo */

            --accent-hover: #409a71;

            --accent-light: #eef9f3;   /* Soft highlight tint */

            --text-dark: #1f2937;     /* High-contrast body text */

            --text-muted: #4b5563;    /* Secondary gray */

            --bg-light: #f9fafb;      /* Crisp off-white panels */

            --white: #ffffff;

            --warning: #de3c3c;       /* Urgent alert accents */

            --warning-light: #fdf2f2;

            --max-width: 1140px;

            --section-padding: 100px;

            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);

        }



        * {

            margin: 0;

            padding: 0;

            box-sizing: border-box;

        }



        html {

            scroll-behavior: smooth;

        }



        body {

            font-family: 'Inter', system-ui, -apple-system, sans-serif;

            color: var(--text-dark);

            line-height: 1.6;

            background-color: var(--white);

            -webkit-font-smoothing: antialiased;

        }



        /* CORE UTILITY LAYOUTS */

        .container {

            width: 100%;

            max-width: var(--max-width);

            margin: 0 auto;

            padding: 0 24px;

        }



        .btn {

            display: inline-block;

            background-color: var(--accent);

            color: var(--white);

            padding: 14px 28px;

            border-radius: 6px;

            font-weight: 500;

            text-decoration: none;

            transition: var(--transition);

            text-align: center;

            border: none;

            cursor: pointer;

            font-size: 1rem;

        }



        .btn:hover {

            background-color: var(--accent-hover);

            transform: translateY(-2px);

            box-shadow: 0 8px 20px rgba(82, 183, 136, 0.25);

        }



        .btn-outline {

            background-color: transparent;

            color: var(--primary);

            border: 2px solid var(--primary);

        }



        .btn-outline:hover {

            background-color: var(--primary);

            color: var(--white);

            box-shadow: 0 8px 20px rgba(30, 27, 75, 0.15);

        }



        .btn-white {

            background-color: var(--white);

            color: var(--primary);

        }

        .btn-white:hover {

            background-color: #f3f4f6;

            box-shadow: 0 8px 20px rgba(255, 255, 255, 0.15);

        }

        /* PREMIUM FLOATING STICKY NAVIGATION BAR */

        header {

            background-color: rgba(255, 255, 255, 0.95);

            backdrop-filter: blur(8px);

            -webkit-backdrop-filter: blur(8px);

            border-bottom: 1px solid #f3f4f6;

            position: sticky;

            top: 0;

            z-index: 1000;

            box-shadow: 0 4px 20px rgba(0,0,0,0.02);

        }



        .nav-container {

            display: flex;

            justify-content: space-between;

            align-items: center;

            height: 90px;

        }



        .logo-area {

            display: flex;

            align-items: center;

        }



        .logo-img {

            height: 65px;

            width: auto;

            object-fit: contain;

        }



        /* Nav links layout */

        .nav-menu {

            display: flex;

            align-items: center;

            gap: 32px;

            list-style: none;

        }



        .nav-link {

            color: var(--text-dark);

            text-decoration: none;

            font-weight: 500;

            font-size: 0.95rem;

            transition: var(--transition);

        }



        .nav-link:hover {

            color: var(--accent);

        }



        .nav-link-btn {

            background-color: var(--primary);

            color: var(--white);

            padding: 10px 20px;

            border-radius: 6px;

        }



        .nav-link-btn:hover {

            background-color: var(--primary-light);

            color: var(--white);

        }



        /* CONTEXTUAL VISUAL SECTIONS & BREAKS */

        section {

            padding: var(--section-padding) 0;

            position: relative;

        }



        .section-bg {

            background-color: var(--bg-light);

        }



        /* Clean geometric separator line instead of block borders */

        .section-separator {

            height: 1px;

            background: linear-gradient(to right, rgba(0,0,0,0), #e5e7eb, rgba(0,0,0,0));

            width: 100%;

        }



        .section-header {

            max-width: 650px;

            margin-bottom: 64px;

        }



        .section-header h2 {

            font-size: 2.5rem;

            color: var(--primary);

            margin-bottom: 16px;

            font-weight: 700;

            letter-spacing: -0.5px;

        }



        .section-header p {

            color: var(--text-muted);

            font-size: 1.1rem;

        }



        /* HERO INTRODUCTION HEADER */

        .hero {

            padding: 80px 0;

            background-color: var(--white);

        }



        .hero-grid {

            display: grid;

            grid-template-columns: 1.1fr 0.9fr;

            gap: 64px;

            align-items: center;

        }



        .hero-tagline {

            color: var(--accent);

            text-transform: uppercase;

            letter-spacing: 2px;

            font-weight: 700;

            font-size: 0.9rem;

            margin-bottom: 16px;

        }



        .hero h1 {

            font-size: 3.4rem;

            color: var(--primary);

            line-height: 1.15;

            margin-bottom: 24px;

            font-weight: 700;

            letter-spacing: -1px;

        }



        .hero p {

            font-size: 1.15rem;

            color: var(--text-muted);

            margin-bottom: 40px;

            max-width: 540px;

        }



        .hero-actions {

            display: flex;

            gap: 16px;

        }



        .hero-image-container {

            height: 560px;

            width: 100%;

            border-radius: 16px;

            overflow: hidden;

            box-shadow: 0 30px 60px -15px rgba(0, 0, 0, 0.08);

        }



        .hero-img {

            width: 100%;

            height: 100%;

            object-fit: cover;

            object-position: center 25%;

        }



        /* PRIORITY CLINICAL EMERGENCY ALERTS */

        .emergency-banner {

            background-color: var(--warning-light);

            border-left: 4px solid var(--warning);

            padding: 24px;

            border-radius: 8px;

            margin-bottom: 60px;

            display: flex;

            align-items: center;

            gap: 20px;

            box-shadow: 0 4px 12px rgba(222, 60, 60, 0.03);

        }



        .emergency-icon {

            background-color: var(--warning);

            color: var(--white);

            width: 40px;

            height: 40px;

            border-radius: 50%;

            display: flex;

            align-items: center;

            justify-content: center;

            flex-shrink: 0;

            font-weight: 700;

            font-size: 1.2rem;

        }



        .emergency-text h4 {

            color: var(--warning);

            font-size: 1.15rem;

            font-weight: 700;

            margin-bottom: 4px;

        }



        .emergency-text p {

            color: #7f1d1d;

            font-size: 1rem;

        }



        /* CLINICAL OPERATIONS SERVICES CARD GRID */

        .services-grid {

            display: grid;

            grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));

            gap: 32px;

        }



        .service-card {

            background: var(--white);

            padding: 44px;

            border-radius: 16px;

            transition: var(--transition);

            border: 1px solid #eaeaea;

            box-shadow: 0 4px 20px rgba(0,0,0,0.01);

        }



        .service-card:hover {

            transform: translateY(-8px);

            box-shadow: 0 24px 40px rgba(0, 0, 0, 0.06);

            border-color: var(--accent);

        }



        .service-icon-box {

            width: 60px;

            height: 60px;

            background-color: var(--accent-light);

            border-radius: 12px;

            display: flex;

            align-items: center;

            justify-content: center;

            margin-bottom: 28px;

            color: var(--accent);

        }



        .service-icon-box svg {

            width: 30px;

            height: 30px;

            fill: currentColor;

        }



        .service-card h3 {

            font-size: 1.4rem;

            color: var(--primary);

            margin-bottom: 16px;

            font-weight: 700;

        }



        .service-card p {

            color: var(--text-muted);

            font-size: 0.95rem;

            line-height: 1.65;

        }



        /* FULL WIDTH BANNER MODULATORS */

        .patient-welcome-banner {

            background-color: var(--primary);

            color: var(--white);

            padding: 90px 0;

            position: relative;

            overflow: hidden;

        }



        .patient-welcome-banner::before {

            content: '';

            position: absolute;

            top: -50%;

            right: -10%;

            width: 600px;

            height: 600px;

            background: radial-gradient(circle, rgba(82,183,136,0.18) 0%, rgba(0,0,0,0) 70%);

            border-radius: 50%;

            pointer-events: none;

        }



        .banner-flex {

            display: flex;

            justify-content: space-between;

            align-items: center;

            gap: 64px;

        }



        .banner-content {

            max-width: 660px;

        }



        .banner-content h2 {

            font-size: 2.6rem;

            margin-bottom: 18px;

            color: var(--white);

            font-weight: 700;

            letter-spacing: -0.5px;

        }



        .banner-content p {

            color: rgba(255, 255, 255, 0.85);

            font-size: 1.15rem;

            margin-bottom: 28px;

        }



        .banner-meta {

            border-top: 1px solid rgba(255, 255, 255, 0.15);

            padding-top: 28px;

        }



        .banner-meta h4 {

            color: var(--accent);

            font-size: 1.15rem;

            margin-bottom: 8px;

            font-weight: 600;

        }



        .banner-meta p {

            margin-bottom: 0;

            font-size: 1rem;

            color: rgba(255, 255, 255, 0.8);

        }



        .banner-action {

            flex-shrink: 0;

        }



        /* TWO-COLUMN VALUEPROP & SCHEDULING WRAPPERS */

        .split-grid {

            display: grid;

            grid-template-columns: 1fr 1fr;

            gap: 80px;

            align-items: start;

        }



        .feature-list {

            list-style: none;

        }



        .feature-item {

            margin-bottom: 36px;

            display: flex;

            gap: 20px;

        }



        .feature-checkbox {

            width: 26px;

            height: 26px;

            background-color: var(--accent-light);

            color: var(--accent);

            border-radius: 50%;

            display: flex;

            align-items: center;

            justify-content: center;

            flex-shrink: 0;

            margin-top: 2px;

        }



        .feature-checkbox svg {

            width: 14px;

            height: 14px;

            fill: currentColor;

        }



        .feature-item h4 {

            font-size: 1.2rem;

            color: var(--primary);

            margin-bottom: 6px;

            font-weight: 700;

        }



        .feature-item p {

            color: var(--text-muted);

            font-size: 1rem;

        }



        /* SCHEDULING INTAKE SUBMISSION COMPONENT */

        .form-container {

            background: var(--white);

            padding: 52px;

            border-radius: 16px;

            box-shadow: 0 30px 60px rgba(0, 0, 0, 0.04);

            border: 1px solid #e5e7eb;

        }



        .form-container h3 {

            font-size: 1.7rem;

            color: var(--primary);

            margin-bottom: 10px;

            font-weight: 700;

        }



        .form-container p {

            color: var(--text-muted);

            font-size: 1rem;

            margin-bottom: 32px;

        }



        .form-group {

            margin-bottom: 24px;

        }



        .form-group label {

            display: block;

            font-size: 0.85rem;

            font-weight: 600;

            color: var(--primary);

            margin-bottom: 8px;

            text-transform: uppercase;

            letter-spacing: 0.5px;

        }



        .form-control {

            width: 100%;

            padding: 14px 18px;

            border: 1px solid #d1d5db;

            border-radius: 6px;

            font-family: inherit;

            font-size: 1rem;

            color: var(--text-dark);

            transition: var(--transition);

            background-color: #fafafa;

        }



        .form-control:focus {

            outline: none;

            border-color: var(--accent);

            background-color: var(--white);

            box-shadow: 0 0 0 4px rgba(82, 183, 136, 0.15);

        }



        select.form-control {

            appearance: none;

            background-image: url("data:image/svg+xml;charset=UTF-8,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='none' stroke='%234b5563' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3e%3cpolyline points='6 9 12 15 18 9'%3e%3c/polyline%3e%3c/shadow%3e");

            background-repeat: no-repeat;

            background-position: right 18px center;

            background-size: 16px;

            padding-right: 44px;

        }



        textarea.form-control {

            resize: vertical;

            min-height: 110px;

        }



        /* REGIONAL FACILITY LOGISTICS MAP FRAME */

        .contact-layout {

            display: grid;

            grid-template-columns: 1fr 1.2fr;

            gap: 64px;

        }



        .info-pane {

            display: flex;

            flex-direction: column;

            justify-content: flex-start;

        }



        .info-block {

            margin-bottom: 40px;

        }



        .info-block h3 {

            font-size: 0.85rem;

            text-transform: uppercase;

            letter-spacing: 1.5px;

            color: var(--accent);

            margin-bottom: 12px;

            font-weight: 700;

        }



        .info-block p, .info-block a {

            font-size: 1.15rem;

            color: var(--text-dark);

            text-decoration: none;

        }



        .info-block a {

            color: var(--primary);

            font-weight: 600;

            transition: var(--transition);

        }



        .info-block a:hover {

            color: var(--accent);

            text-decoration: underline;

        }



        .map-pane {

            width: 100%;

            height: 490px;

            border-radius: 12px;

            overflow: hidden;

            border: 1px solid #e5e7eb;

            box-shadow: 0 20px 40px rgba(0,0,0,0.02);

        }



        .map-pane iframe {

            width: 100%;

            height: 100%;

            border: 0;

        }



        /* SYSTEM GLOBAL FOOTER CONTAINER */

        footer {

            background-color: var(--primary);

            color: rgba(255, 255, 255, 0.8);

            padding: 80px 0 40px;

            font-size: 0.95rem;

        }



        .footer-grid {

            display: flex;

            justify-content: space-between;

            align-items: flex-start;

            padding-bottom: 48px;

            border-bottom: 1px solid rgba(255, 255, 255, 0.1);

            margin-bottom: 32px;

        }



        .footer-brand {

            max-width: 380px;

        }



        .footer-brand h3 {

            color: var(--white);

            font-size: 1.6rem;

            margin-bottom: 12px;

            font-weight: 700;

        }



        .footer-brand p {

            font-style: italic;

            opacity: 0.75;

            margin-bottom: 24px;

        }



        /* Facebook Branding Interface Link Component */

        .fb-link-btn {

            display: inline-flex;

            align-items: center;

            gap: 12px;

            background-color: #1877f2;

            color: var(--white);

            padding: 12px 24px;

            border-radius: 6px;

            text-decoration: none;

            font-weight: 600;

            font-size: 0.95rem;

            transition: var(--transition);

        }



        .fb-link-btn:hover {

            background-color: #166fe5;

            transform: translateY(-2px);

            box-shadow: 0 8px 20px rgba(24, 119, 242, 0.3);

        }



        .fb-link-btn svg {

            width: 20px;

            height: 20px;

            fill: currentColor;

        }



        .footer-resources {

            max-width: 520px;

        }



        .footer-resources h4 {

            color: var(--white);

            margin-bottom: 16px;

            font-weight: 600;

            font-size: 1.15rem;

        }



        .footer-resources p {

            margin-bottom: 10px;

            line-height: 1.6;

        }



        .footer-meta {

            display: flex;

            justify-content: space-between;

            align-items: center;

            opacity: 0.55;

            font-size: 0.85rem;

        }



        /* ADAPTIVE DISPLAYS RESPONSIVE GRID CONFIGS */

        @media (max-width: 968px) {

            header {

                position: relative;

            }



            .nav-menu {

                display: none;

            }



            .hero-grid, .split-grid, .contact-layout, .banner-flex {

                grid-template-columns: 1fr;

                gap: 48px;

            }



            .banner-flex {

                align-items: flex-start;

            }



            .hero-image-container {

                height: 420px;

                order: -1;

            }



            .hero {

                padding: 40px 0 80px;

            }



            .hero h1 {

                font-size: 2.8rem;

            }



            section {

                padding: 70px 0;

            }



            .footer-grid {

                flex-direction: column;

                gap: 40px;

            }



            .footer-meta {

                flex-direction: column;

                align-items: flex-start;

                gap: 12px;

            }

        }



        @media (max-width: 480px) {

            .nav-container {

                flex-direction: column;

                justify-content: center;

                height: auto;

                padding: 24px 0;

                gap: 16px;

            }



            .hero h1 {

                font-size: 2.2rem;

            }

            

            .form-container {

                padding: 36px 24px;

            }

        }

    </style>

</head>

<body>



    <!-- FLOATING STICKY NAVIGATION BAR CONTAINER -->

    <header>

        <div class="container nav-container">

            <div class="logo-area">

                <img class="logo-img" src="miller-dental-logo.png" alt="Miller Family Dental Care" onerror="this.style.display='none'; this.nextElementSibling.style.display='block';">

                <span style="display:none; font-weight:700; font-size:1.5rem; color:var(--primary);">Miller Family Dental Care</span>

            </div>

            

            <!-- Quick Anchor Links -->

            <ul class="nav-menu">

                <li><a href="#services" class="nav-link">Services</a></li>

                <li><a href="#why-choose-us" class="nav-link">Why Choose Us</a></li>

                <li><a href="#location" class="nav-link">Location</a></li>

                <li><a href="#appointment" class="nav-link nav-link-btn">Request Appointment</a></li>

            </ul>

        </div>

    </header>



    <!-- INTRODUCTORY BANNER HERO SCREEN -->

    <section class="hero">

        <div class="container hero-grid">

            <div class="hero-content">

                <p class="hero-tagline">Proudly Serving Our Kokomo Community</p>

                <h1>Compassionate care.<br>Practical solutions.<br>Lasting smiles.</h1>

                <p>Welcome to Miller Family Dental Care. We provide comprehensive, patient-centered dental services for all ages. Our practice combines gentle care, advanced technology, and a comfortable office environment to help your family maintain healthy, confident smiles.</p>

                <div class="hero-actions">

                    <a href="#appointment" class="btn">Request Appointment</a>

                    <a href="#services" class="btn btn-outline">Explore Our Services</a>

                </div>

            </div>

            <div class="hero-image-container">

                <img class="hero-img" src="patient-smile-header.png" alt="Happy Patient Smile at Miller Family Dental Care">

            </div>

        </div>

    </section>



    <div class="section-separator"></div>



    <!-- SERVICES CLUSTERS WITH SYSTEM SVG ICON PACKS -->

    <section id="services" class="section-bg">

        <div class="container">

            

            <!-- Priority Dental Urgent Assistance Alert Bar -->

            <div class="emergency-banner">

                <div class="emergency-icon">!</div>

                <div class="emergency-text">

                    <h4>Dental Emergency Care Available</h4>

                    <p>Experiencing a severe toothache or broken tooth? We provide same-day or next-available priority appointments. Call us immediately at <strong>765.456.3015</strong>.</p>

                </div>

            </div>



            <div class="section-header">

                <h2>Our Dental Services</h2>

                <p>From routine prevention to advanced structural corrective therapies, our clinical operations are tailored completely around your lifestyle and oral health goals.</p>

            </div>

            

            <div class="services-grid">

                <!-- Service Item 1 -->

                <div class="service-card">

                    <div class="service-icon-box">

                        <svg viewBox="0 0 24 24"><path d="M12,2A3,3 0 0,0 9,5C9,6.05 9.47,7 10.22,7.63C10.05,8.7 9.87,10.74 10.5,12.33C11.08,13.78 12.16,14.67 13.5,14.93V19A1,1 0 0,0 14.5,20A1,1 0 0,0 15.5,19V14.93C16.84,14.67 17.92,13.78 18.5,12.33C19.13,10.74 18.95,8.7 18.78,7.63C19.53,7 20,6.05 20,5A3,3 0 0,0 17,2A3,3 0 0,0 14,5C14,6.05 14.47,7 15.22,7.63C15.09,8.44 14.94,10 15.3,11.16C15.5,11.77 15.93,12.24 16.5,12.44V19C16.5,20.1 15.6,21 14.5,21C13.4,21 12.5,20.1 12.5,19V12.44C13.07,12.24 13.5,11.77 13.7,11.16C14.06,10 13.91,8.44 13.78,7.63C14.53,7 15,6.05 15,5A3,3 0 0,0 12,2M7,7A1,1 0 0,0 6,8A1,1 0 0,0 7,9A1,1 0 0,0 8,8A1,1 0 0,0 7,7M4,10A1,1 0 0,0 3,11A1,1 0 0,0 4,12A1,1 0 0,0 5,11A1,1 0 0,0 4,10M5,14A1,1 0 0,0 4,15A1,1 0 0,0 5,16A1,1 0 0,0 6,15A1,1 0 0,0 5,14Z"></path></svg>

                    </div>

                    <h3>Preventive Care</h3>

                    <p>Routine cleanings, comprehensive oral exams, targeted dental sealants, and personalized home-care guidance designed to intercept decay and gum disease before they start.</p>

                </div>

                <!-- Service Item 2 -->

                <div class="service-card">

                    <div class="service-icon-box">

                        <svg viewBox="0 0 24 24"><path d="M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M12,4A8,8 0 0,1 20,12A8,8 0 0,1 12,20A8,8 0 0,1 4,12A8,8 0 0,1 12,4M11,7V13H13V7H11M11,15V17H13V15H11Z"></path></svg>

                    </div>

                    <h3>Restorative Dentistry</h3>

                    <p>High-tier fillings, durable crowns, bridges, and full-mouth rehabilitations focused on rebuilding long-term structural function and natural appearance.</p>

                </div>

                <!-- Service Item 3 -->

                <div class="service-card">

                    <div class="service-icon-box">

                        <svg viewBox="0 0 24 24"><path d="M11.5,8C11.5,10 10,11.5 8,11.5C6,11.5 4.5,10 4.5,8C4.5,6 6,4.5 8,4.5C10,4.5 11.5,6 11.5,8M19,11.5C17.62,11.5 16.5,12.62 16.5,14C16.5,15.38 17.62,16.5 19,16.5C20.38,16.5 21.5,15.38 21.5,14C21.5,12.62 20.38,11.5 19,11.5M19.5,4C19.5,5.1 18.6,6 17.5,6C16.4,6 15.5,5.1 15.5,4C15.5,2.9 16.4,2 17.5,2C18.6,2 19.5,2.9 19.5,4M14,15.5C12.34,15.5 11,16.84 11,18.5C11,20.16 12.34,21.5 14,21.5C15.66,21.5 17,20.16 17,18.5C17,16.84 15.66,15.5 14,15.5Z"></path></svg>

                    </div>

                    <h3>Cosmetic Dentistry</h3>

                    <p>Professional teeth whitening, custom porcelain veneers, and direct cosmetic bonding to enhance, balance, and reveal your ideal smile aesthetic.</p>

                </div>

                <!-- Service Item 4 -->

                <div class="service-card">

                    <div class="service-icon-box">

                        <svg viewBox="0 0 24 24"><path d="M19 3H5C3.9 3 3 3.9 3 5V19C3 20.1 3.9 21 5 21H19C20.1 21 21 20.1 21 19V5C21 3.9 20.1 3 19 3M17 12H13V17H11V12H7V10H17V12Z"></path></svg>

                    </div>

                    <h3>Dental Implants</h3>

                    <p>Single-tooth dental implants and robust implant-supported bridge restorations providing premium, biocompatible long-term tooth replacement options.</p>

                </div>

                <!-- Service Item 5 -->

                <div class="service-card">

                    <div class="service-icon-box">

                        <svg viewBox="0 0 24 24"><path d="M12,2A3,3 0 0,1 15,5A3,3 0 0,1 12,8A3,3 0 0,1 9,5A3,3 0 0,1 12,2M11,22V17H9V12A2,2 0 0,1 11,10H13A2,2 0 0,1 15,12V17H13V22H11Z"></path></svg>

                    </div>

                    <h3>Pediatric Dentistry</h3>

                    <p>Gentle care tailored explicitly for children. Focuses on setting up positive preventive memories, growth milestone assessments, and protective early home guidance.</p>

                </div>

                <!-- Service Item 6 -->

                <div class="service-card">

                    <div class="service-icon-box">

                        <svg viewBox="0 0 24 24"><path d="M12,2C11.31,2 10.64,2.13 10.03,2.38C7.57,3.38 6,5.83 6,8.5C6,11.84 8.04,14.36 11,14.89V21A1,1 0 0,0 12,22A1,1 0 0,0 13,21V14.89C15.96,14.36 18,11.84 18,8.5C18,5.83 16.43,3.38 13.97,2.38C13.36,2.13 12.69,2 12,2Z"></path></svg>

                    </div>

                    <h3>Periodontal Care</h3>

                    <p>Advanced diagnosis and treatment of active gum disease, including precision scaling and root planing alongside proactive long-term tissue maintenance protocols.</p>

                </div>

            </div>

        </div>

    </section>



    <!-- REASSURING FULL WIDTH WELCOME ACCENT BLOCK -->

    <section class="patient-welcome-banner">

        <div class="container banner-flex">

            <div class="banner-content">

                <h2>Welcoming New Patients &amp; Families</h2>

                <p>We make transitioning to a new dental office simple and transparent. Your initial reservation involves an extensive systemic check, detailed digital X-rays as required, and an open, zero-pressure treatment discussion with Dr. Paul Miller.</p>

                

                <div class="banner-meta">

                    <h4>Insurance &amp; Financing Transparency</h4>

                    <p>We work in-network with <strong>Delta Dental</strong> and file claims directly for you. Uninsured? Ask our team about our flexible financing paths or join our exclusive <strong>In-House Member Program</strong>.</p>

                </div>

            </div>

            <div class="banner-action">

                <a href="#appointment" class="btn btn-white">Request Registration Info</a>

            </div>

        </div>

    </section>



    <!-- INTAKE RESERVATION FORM SCREEN -->

    <section id="why-choose-us">

        <div class="container split-grid">

            

            <!-- Value Prop Accordions -->

            <div class="feature-pane">

                <div class="section-header" style="margin-bottom: 40px;">

                    <h2>Why Choose Us</h2>

                    <p>We approach family dentistry differently, blending clinical modern tools with individual respect and continuous medical education.</p>

                </div>

                <ul class="feature-list">

                    <li class="feature-item">

                        <div class="feature-checkbox">

                            <svg viewBox="0 0 24 24"><path d="M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"></path></svg>

                        </div>

                        <div>

                            <h4>Experienced Team</h4>

                            <p>Dr. Paul Miller and our supporting hygienists stand dedicated to evidence-based conservative treatments and ongoing clinical safety training.</p>

                        </div>

                    </li>

                    <li class="feature-item">

                        <div class="feature-checkbox">

                            <svg viewBox="0 0 24 24"><path d="M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"></path></svg>

                        </div>

                        <div>

                            <h4>Patient Comfort</h4>

                            <p>Relax within modern operatory treatment rooms featuring ergonomic patient seating and dental sedation paths for anxious individuals.</p>

                        </div>

                    </li>

                    <li class="feature-item">

                        <div class="feature-checkbox">

                            <svg viewBox="0 0 24 24"><path d="M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"></path></svg>

                        </div>

                        <div>

                            <h4>Advanced Technology</h4>

                            <p>Utilizing high-definition digital X-rays, intraoral cameras, and modern sterilization stations for highly accurate diagnosis and optimal care safety.</p>

                        </div>

                    </li>

                    <li class="feature-item">

                        <div class="feature-checkbox">

                            <svg viewBox="0 0 24 24"><path d="M21,7L9,19L3.5,13.5L4.91,12.09L9,16.17L19.59,5.59L21,7Z"></path></svg>

                        </div>

                        <div>

                            <h4>Personalized Treatment</h4>

                            <p>We design specific treatment paths scaled dynamically around your unique oral health criteria, schedule preferences, and personal financial framework.</p>

                        </div>

                    </li>

                </ul>

            </div>

            

            <!-- Online Appointment Request Intake Form Block -->

            <div class="form-container" id="appointment">

                <h3>Online Appointment Request</h3>

                <p>Submit your preferred times below. Our front desk team will contact you shortly to confirm your reservation details.</p>


                <form action="https://api.web3forms.com/submit" method="POST">
                    <input type="hidden" name="access_key" value="b7557e9b-c049-412a-bac1-6c18924f15dc">
                    <div class="form-group">
                        <label for="name">Full Name</label>
                        <input type="text" name="name" class="form-control" placeholder="John Doe" required="">
                    </div>

                    <div class="form-row" style="display: grid; grid-template-columns: 1fr 1fr; gap: 16px;">
                        <div class="form-group">
                            <label for="form-phone">Phone Number</label>
                            <input type="tel" name="phone" id="form-phone" class="form-control" placeholder="(765) 555-0123" required="">

                        </div>

                        <div class="form-group">
                            <label for="form-email">Email Address</label>
                            <input  type="email" name="email" id="form-email" class="form-control" placeholder="john@example.com" required="">
                        </div>
                    </div>

                    <div class="form-group">
                        <label for="service-type">Desired Service</label>
                        <select name="service" id="service-type" class="form-control">
                            <option value="routine-cleaning">Routine Cleaning &amp; Exam</option>
                            <option value="pediatric">New Patient Visit</option>
                            <option value="emergency">Emergency Dental Visit</option>
                            <option value="cosmetic">Cosmetic / Whitening Consultation</option>
                            <option value="other">Other Dental Inquiry</option>
                        </select>
                    </div>

                    <div class="form-group">
                        <label for="message">Additional Notes or Preferred Availability</label>
                        <textarea id="message" name="message" class="form-control" placeholder="e.g., Tuesday mornings preferred, questions about dental insurance, etc."></textarea>
                    </div>

                    <button type="submit" class="btn" style="width: 100%; padding: 16px;">Submit Scheduling Request</button>
                </form>
            </div>

        </div>
    </section>

    <div class="section-separator"></div>
    <!-- GEOGRAPHIC LOGISTICS & HOUR MATRICES -->

    <section class="section-bg" id="location">

        <div class="container contact-layout">

            <div class="info-pane">

                <div class="section-header" style="margin-bottom: 32px;">

                    <h2>Get In Touch</h2>

                    <p>Have a question or ready to schedule your appointment? Reach out via phone, email, or stop by our clean, accessible facility.</p>

                </div>

                

                <div class="info-block">

                    <h3>Office Location</h3>

                    <p>200 S Dixon Rd.<br>Kokomo, IN 46901</p>

                </div>



                <div class="info-block">

                    <h3>Hours of Operation</h3>

                    <p>Monday – Thursday: 8:30 AM – 5:00 PM</p>

                </div>



                <div class="info-block">

                    <h3>Direct Communication</h3>

                    <p style="margin-bottom: 8px;">Phone: <a href="tel:7654563015">765.456.3015</a></p>

                    <p>Email: <a href="mailto:millerfamilydentalcare@gmail.com">millerfamilydentalcare@gmail.com</a></p>

                </div>

            </div>

            

            <!-- Safe Native Google Map Layer -->

            <div class="map-pane">

                <iframe title="Miller Family Dental Care Location Map" src="https://maps.google.com/maps?q=200%20S%20Dixon%20Rd,%20Kokomo,%20IN%2046901&amp;t=&amp;z=15&amp;ie=UTF8&amp;iwloc=&amp;output=embed" allowfullscreen="" loading="lazy">

                </iframe>

            </div>

        </div>

    </section>



    <!-- COMPREHENSIVE MEDICAL BRAND FOOTER -->

    <footer>

        <div class="container">

            <div class="footer-grid">

                <div class="footer-brand">

                    <h3>Miller Family Dental Care</h3>

                    <p>Compassionate care. Practical solutions. Lasting smiles.</p>

                    

                    <!-- Direct Dynamic Facebook Button link -->

                    <a href="https://www.facebook.com/paulandbrittamiller/" target="_blank" rel="noopener noreferrer" class="fb-link-btn">

                        <svg viewBox="0 0 24 24"><path d="M22 12c0-5.52-4.48-10-10-10S2 6.48 2 12c0 4.84 3.44 8.87 8 9.8V15H8v-3h2V9.5C10 7.57 11.57 6 13.5 6H16v3h-2c-.55 0-1 .45-1 1v2h3v3h-3v6.95c4.56-.93 8-4.96 8-9.8z"></path></svg>

                        Follow Us on Facebook

                    </a>

                </div>

                

                <div class="footer-resources">

                    <h4>Patient Quick Resources</h4>

                    <p>• New Patient Registration Forms are available at the front desk for streamlined check-in.</p>

                    <p>• Dental emergencies are prioritized during regular office hours.</p>

                </div>

            </div>

            <div class="footer-meta">

                <p>© Miller Family Dental Care. All Rights Reserved. Comforting families across Kokomo, Indiana since 1979.</p>

                <p style="opacity: 0.7;">Dr. Paul Miller, DDS</p>

            </div>

        </div>

    </footer>
</body></html>
