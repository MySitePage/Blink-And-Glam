<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BLINK & GLAM BY ELLY | Premium Lash Studio Namibia</title>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;500;600;700&family=Montserrat:wght@200;300;400;500;600;700;800&family=Dancing+Script:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* ===== CUSTOM PROPERTIES ===== */
        :root {
            /* Color Palette - Dark Grey & Gold Theme */
            --rich-black: #0A0A0A;
            --jet-black: #121212;
            --eerie-black: #1A1A1A;
            --dark-charcoal: #222222;
            --gunmetal: #2A2A2A;
            --dark-slate: #333333;
            
            --dark-gold: #8B6914;
            --antique-gold: #C9A227;
            --golden-yellow: #D4AF37;
            --light-gold: #E6D6A8;
            --pale-gold: #F5E8C8;
            
            --pure-white: #FFFFFF;
            --snow-white: #F8F8F8;
            --platinum: #E8E8E8;
            --silver: #D0D0D0;
            --light-gray: #B8B8B8;
            --medium-gray: #888888;
            --dark-gray: #585858;
            
            /* Shadows & Effects */
            --shadow-soft: 0 4px 6px rgba(0, 0, 0, 0.1);
            --shadow-medium: 0 10px 20px rgba(0, 0, 0, 0.2);
            --shadow-hard: 0 20px 40px rgba(0, 0, 0, 0.3);
            --shadow-gold: 0 10px 30px rgba(212, 175, 55, 0.15);
            --shadow-gold-hard: 0 20px 50px rgba(212, 175, 55, 0.25);
            
            /* Gradients */
            --gradient-dark: linear-gradient(135deg, var(--rich-black) 0%, var(--jet-black) 100%);
            --gradient-gold: linear-gradient(135deg, var(--dark-gold) 0%, var(--golden-yellow) 50%, var(--light-gold) 100%);
            --gradient-overlay: linear-gradient(rgba(10, 10, 10, 0.9), rgba(18, 18, 18, 0.95));
            --gradient-text: linear-gradient(90deg, var(--golden-yellow), var(--light-gold));
            
            /* Transitions */
            --transition-fast: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
            --transition-normal: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            --transition-slow: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            --transition-very-slow: all 0.8s cubic-bezier(0.4, 0, 0.2, 1);
            
            /* Borders & Radius */
            --radius-small: 8px;
            --radius-medium: 15px;
            --radius-large: 25px;
            --radius-xlarge: 40px;
            --radius-circle: 50%;
            
            /* Spacing */
            --space-xs: 5px;
            --space-sm: 10px;
            --space-md: 20px;
            --space-lg: 40px;
            --space-xl: 60px;
            --space-xxl: 100px;
            
            /* Typography Scale */
            --text-xs: 0.75rem;
            --text-sm: 0.875rem;
            --text-base: 1rem;
            --text-lg: 1.125rem;
            --text-xl: 1.25rem;
            --text-2xl: 1.5rem;
            --text-3xl: 1.875rem;
            --text-4xl: 2.25rem;
            --text-5xl: 3rem;
            --text-6xl: 3.75rem;
            --text-7xl: 4.5rem;
            --text-8xl: 6rem;
        }
        
        /* ===== RESET & BASE STYLES ===== */
        *, *::before, *::after {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html {
            font-size: 16px;
            scroll-behavior: smooth;
            scroll-padding-top: 100px;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--rich-black);
            color: var(--snow-white);
            line-height: 1.7;
            font-weight: 400;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        
        /* ===== TYPOGRAPHY ===== */
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Cormorant Garamond', serif;
            font-weight: 700;
            line-height: 1.2;
            color: var(--golden-yellow);
            margin-bottom: var(--space-md);
        }
        
        h1 {
            font-size: var(--text-8xl);
            letter-spacing: -1px;
            line-height: 1;
        }
        
        h2 {
            font-size: var(--text-6xl);
            letter-spacing: -0.5px;
        }
        
        h3 {
            font-size: var(--text-4xl);
        }
        
        h4 {
            font-size: var(--text-2xl);
        }
        
        p {
            margin-bottom: var(--space-md);
            font-size: var(--text-lg);
            color: var(--silver);
        }
        
        a {
            color: inherit;
            text-decoration: none;
            transition: var(--transition-normal);
        }
        
        ul, ol {
            list-style-position: inside;
            margin-bottom: var(--space-md);
        }
        
        li {
            margin-bottom: var(--space-sm);
            color: var(--silver);
        }
        
        /* ===== REUSABLE COMPONENTS ===== */
        .container {
            max-width: 1600px;
            margin: 0 auto;
            padding: 0 var(--space-lg);
        }
        
        .section {
            padding: var(--space-xxl) 0;
            position: relative;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: var(--space-xl);
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 150px;
            height: 3px;
            background: var(--gradient-gold);
            border-radius: 3px;
        }
        
        .section-subtitle {
            text-align: center;
            font-size: var(--text-xl);
            color: var(--light-gray);
            max-width: 800px;
            margin: 0 auto var(--space-xl);
        }
        
        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 18px 45px;
            border-radius: var(--radius-xlarge);
            font-weight: 700;
            font-size: var(--text-lg);
            letter-spacing: 1.5px;
            text-transform: uppercase;
            transition: var(--transition-normal);
            position: relative;
            overflow: hidden;
            border: 2px solid transparent;
            gap: 12px;
        }
        
        .btn-primary {
            background: var(--gradient-gold);
            color: var(--rich-black);
            border: 2px solid var(--golden-yellow);
        }
        
        .btn-primary:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-gold-hard);
            color: var(--rich-black);
        }
        
        .btn-secondary {
            background: transparent;
            color: var(--golden-yellow);
            border: 2px solid var(--golden-yellow);
        }
        
        .btn-secondary:hover {
            background: var(--golden-yellow);
            color: var(--rich-black);
            transform: translateY(-5px);
            box-shadow: var(--shadow-gold);
        }
        
        .card {
            background: var(--eerie-black);
            border-radius: var(--radius-large);
            overflow: hidden;
            border: 1px solid var(--gunmetal);
            transition: var(--transition-normal);
            position: relative;
        }
        
        .card:hover {
            transform: translateY(-15px);
            box-shadow: var(--shadow-hard);
            border-color: var(--golden-yellow);
        }
        
        /* ===== HEADER ===== */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(10, 10, 10, 0.95);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(212, 175, 55, 0.1);
            transition: var(--transition-slow);
            padding: var(--space-md) 0;
        }
        
        .header.scrolled {
            padding: var(--space-sm) 0;
            background: rgba(10, 10, 10, 0.98);
            box-shadow: var(--shadow-medium);
        }
        
        .header-container {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }
        
        .logo {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
        }
        
        .logo-main {
            font-family: 'Dancing Script', cursive;
            font-size: var(--text-5xl);
            font-weight: 700;
            color: var(--golden-yellow);
            line-height: 1;
            letter-spacing: 2px;
        }
        
        .logo-sub {
            font-size: var(--text-sm);
            color: var(--light-gray);
            letter-spacing: 4px;
            text-transform: uppercase;
            margin-top: 5px;
            font-weight: 500;
        }
        
        .nav {
            display: flex;
            align-items: center;
            gap: var(--space-xl);
        }
        
        .nav-link {
            position: relative;
            font-weight: 600;
            font-size: var(--text-base);
            letter-spacing: 1.5px;
            text-transform: uppercase;
            color: var(--platinum);
            padding: var(--space-sm) 0;
        }
        
        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--gradient-gold);
            transition: var(--transition-normal);
        }
        
        .nav-link:hover {
            color: var(--golden-yellow);
        }
        
        .nav-link:hover::after {
            width: 100%;
        }
        
        .nav-link.active {
            color: var(--golden-yellow);
        }
        
        .nav-link.active::after {
            width: 100%;
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: var(--golden-yellow);
            font-size: var(--text-2xl);
            cursor: pointer;
            padding: var(--space-sm);
        }
        
        /* ===== HERO SECTION ===== */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            padding-top: 120px;
            background: var(--gradient-dark);
            position: relative;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(circle at 20% 50%, rgba(212, 175, 55, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(139, 105, 20, 0.05) 0%, transparent 50%),
                radial-gradient(circle at 40% 80%, rgba(201, 162, 39, 0.08) 0%, transparent 50%);
            z-index: 1;
        }
        
        .hero-content {
            max-width: 1200px;
            text-align: center;
            position: relative;
            z-index: 2;
        }
        
        .hero-title {
            font-size: var(--text-8xl);
            margin-bottom: var(--space-md);
            text-shadow: 0 5px 30px rgba(0, 0, 0, 0.8);
            background: var(--gradient-text);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: titleGlow 3s ease-in-out infinite alternate;
        }
        
        @keyframes titleGlow {
            0% {
                text-shadow: 0 5px 30px rgba(212, 175, 55, 0.2);
            }
            100% {
                text-shadow: 0 5px 50px rgba(212, 175, 55, 0.4);
            }
        }
        
        .hero-subtitle {
            font-size: var(--text-3xl);
            color: var(--light-gold);
            margin-bottom: var(--space-xl);
            letter-spacing: 3px;
            text-transform: uppercase;
            font-weight: 300;
        }
        
        .hero-divider {
            width: 200px;
            height: 3px;
            background: var(--gradient-gold);
            margin: var(--space-xl) auto;
            position: relative;
            border-radius: 3px;
        }
        
        .hero-divider::before {
            content: '✦';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: var(--rich-black);
            color: var(--golden-yellow);
            padding: 0 var(--space-md);
            font-size: var(--text-xl);
        }
        
        .hero-location {
            font-size: var(--text-xl);
            color: var(--medium-gray);
            margin-bottom: var(--space-xl);
            letter-spacing: 2px;
        }
        
        .hero-cta {
            display: flex;
            gap: var(--space-md);
            justify-content: center;
            flex-wrap: wrap;
            margin-top: var(--space-xl);
        }
        
        /* ===== SERVICES SECTION ===== */
        .services {
            background: var(--gradient-dark);
            position: relative;
        }
        
        .services::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--golden-yellow), transparent);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
            gap: var(--space-xl);
            margin-top: var(--space-xl);
        }
        
        .service-card {
            padding: var(--space-xl);
            transition: var(--transition-normal);
        }
        
        .service-card:hover {
            transform: translateY(-20px);
        }
        
        .service-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: var(--space-lg);
            padding-bottom: var(--space-md);
            border-bottom: 1px solid var(--gunmetal);
        }
        
        .service-name {
            font-size: var(--text-3xl);
            margin-bottom: 0;
        }
        
        .service-price {
            font-size: var(--text-4xl);
            font-weight: 800;
            color: var(--light-gold);
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.5);
        }
        
        .service-description {
            font-size: var(--text-lg);
            color: var(--light-gray);
            margin-bottom: var(--space-lg);
            line-height: 1.8;
        }
        
        .service-features {
            display: flex;
            flex-wrap: wrap;
            gap: var(--space-sm);
            margin-top: var(--space-lg);
        }
        
        .service-feature {
            background: rgba(212, 175, 55, 0.1);
            color: var(--light-gold);
            padding: 8px 20px;
            border-radius: 50px;
            font-size: var(--text-sm);
            border: 1px solid rgba(212, 175, 55, 0.2);
            transition: var(--transition-fast);
        }
        
        .service-feature:hover {
            background: rgba(212, 175, 55, 0.2);
            transform: translateY(-2px);
        }
        
        /* ===== POLICY SECTION ===== */
        .policy {
            background: var(--gradient-dark);
            position: relative;
        }
        
        .policy::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--golden-yellow), transparent);
        }
        
        .policy-container {
            background: var(--eerie-black);
            border-radius: var(--radius-large);
            padding: var(--space-xxl);
            border: 1px solid var(--gunmetal);
            position: relative;
            overflow: hidden;
        }
        
        .policy-container::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: var(--gradient-gold);
        }
        
        .policy-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: var(--space-lg);
            margin-top: var(--space-xl);
        }
        
        .policy-item {
            display: flex;
            align-items: flex-start;
            gap: var(--space-md);
            padding: var(--space-lg);
            background: var(--rich-black);
            border-radius: var(--radius-medium);
            border-left: 4px solid var(--golden-yellow);
            transition: var(--transition-normal);
        }
        
        .policy-item:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-medium);
            border-left-color: var(--light-gold);
        }
        
        .policy-icon {
            color: var(--golden-yellow);
            font-size: var(--text-2xl);
            min-width: 40px;
            padding-top: 5px;
        }
        
        .policy-content h3 {
            font-size: var(--text-xl);
            margin-bottom: var(--space-sm);
            color: var(--light-gold);
        }
        
        .policy-content p {
            font-size: var(--text-base);
            color: var(--silver);
            margin-bottom: 0;
        }
        
        .policy-note {
            background: rgba(212, 175, 55, 0.1);
            border: 1px solid rgba(212, 175, 55, 0.3);
            border-radius: var(--radius-medium);
            padding: var(--space-xl);
            margin-top: var(--space-xxl);
            text-align: center;
        }
        
        .policy-note h4 {
            color: var(--golden-yellow);
            font-size: var(--text-2xl);
            margin-bottom: var(--space-md);
        }
        
        .policy-note p {
            color: var(--light-gold);
            font-size: var(--text-lg);
        }
        
        /* ===== CONTACT SECTION ===== */
        .contact {
            background: var(--gradient-dark);
            position: relative;
        }
        
        .contact::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--golden-yellow), transparent);
        }
        
        .contact-container {
            background: rgba(10, 10, 10, 0.9);
            border-radius: var(--radius-large);
            padding: var(--space-xxl);
            border: 1px solid rgba(212, 175, 55, 0.2);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
        }
        
        .contact-title {
            color: var(--golden-yellow);
            margin-bottom: var(--space-md);
        }
        
        .contact-subtitle {
            color: var(--light-gray);
            font-size: var(--text-xl);
            margin-bottom: var(--space-xl);
            max-width: 700px;
        }
        
        .contact-number {
            font-size: var(--text-6xl);
            font-weight: 800;
            color: var(--light-gold);
            text-align: center;
            margin: var(--space-xl) 0;
            text-shadow: 0 5px 20px rgba(0, 0, 0, 0.5);
            letter-spacing: 2px;
        }
        
        .contact-details {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: var(--space-xl);
            margin-top: var(--space-xxl);
        }
        
        .contact-detail {
            text-align: center;
            padding: var(--space-xl);
            background: rgba(26, 26, 26, 0.7);
            border-radius: var(--radius-medium);
            border: 1px solid var(--gunmetal);
            transition: var(--transition-normal);
        }
        
        .contact-detail:hover {
            transform: translateY(-10px);
            border-color: var(--golden-yellow);
            box-shadow: var(--shadow-medium);
        }
        
        .contact-detail i {
            font-size: var(--text-4xl);
            color: var(--golden-yellow);
            margin-bottom: var(--space-lg);
        }
        
        .contact-detail h3 {
            font-size: var(--text-xl);
            color: var(--light-gold);
            margin-bottom: var(--space-sm);
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        
        .contact-detail p {
            color: var(--silver);
            font-size: var(--text-lg);
            margin-bottom: 0;
        }
        
        /* ===== FOOTER ===== */
        .footer {
            background: var(--rich-black);
            padding: var(--space-xxl) 0 var(--space-xl);
            border-top: 1px solid var(--gunmetal);
            position: relative;
        }
        
        .footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, var(--golden-yellow), transparent);
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: var(--space-xl);
            margin-bottom: var(--space-xxl);
        }
        
        .footer-column h3 {
            font-size: var(--text-2xl);
            color: var(--golden-yellow);
            margin-bottom: var(--space-lg);
        }
        
        .footer-column p {
            color: var(--silver);
            font-size: var(--text-base);
            margin-bottom: var(--space-md);
        }
        
        .social-links {
            display: flex;
            gap: var(--space-md);
            margin-top: var(--space-lg);
        }
        
        .social-link {
            width: 50px;
            height: 50px;
            border-radius: var(--radius-circle);
            background: var(--eerie-black);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--golden-yellow);
            font-size: var(--text-xl);
            border: 1px solid var(--gunmetal);
            transition: var(--transition-normal);
        }
        
        .social-link:hover {
            background: var(--golden-yellow);
            color: var(--rich-black);
            transform: translateY(-5px);
            box-shadow: var(--shadow-gold);
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: var(--space-xl);
            border-top: 1px solid var(--gunmetal);
        }
        
        .copyright {
            color: var(--medium-gray);
            font-size: var(--text-base);
        }
        
        /* ===== RESPONSIVE DESIGN ===== */
        @media (max-width: 1600px) {
            .container {
                max-width: 1400px;
            }
            
            h1 {
                font-size: var(--text-7xl);
            }
            
            h2 {
                font-size: var(--text-5xl);
            }
        }
        
        @media (max-width: 1200px) {
            .container {
                max-width: 1000px;
                padding: 0 var(--space-md);
            }
            
            h1 {
                font-size: var(--text-6xl);
            }
            
            h2 {
                font-size: var(--text-4xl);
            }
            
            .services-grid {
                grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            }
        }
        
        @media (max-width: 992px) {
            .container {
                max-width: 800px;
            }
            
            h1 {
                font-size: var(--text-5xl);
            }
            
            h2 {
                font-size: var(--text-3xl);
            }
            
            .nav {
                gap: var(--space-lg);
            }
            
            .nav-link {
                font-size: var(--text-sm);
            }
            
            .services-grid {
                grid-template-columns: 1fr;
            }
            
            .policy-grid {
                grid-template-columns: 1fr;
            }
            
            .contact-number {
                font-size: var(--text-4xl);
            }
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 0 var(--space-md);
            }
            
            h1 {
                font-size: var(--text-4xl);
            }
            
            h2 {
                font-size: var(--text-2xl);
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .nav {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background: var(--rich-black);
                flex-direction: column;
                align-items: center;
                justify-content: flex-start;
                padding-top: var(--space-xl);
                transition: var(--transition-normal);
                z-index: 999;
            }
            
            .nav.active {
                left: 0;
            }
            
            .nav-link {
                font-size: var(--text-xl);
                padding: var(--space-md) 0;
            }
            
            .hero-subtitle {
                font-size: var(--text-xl);
            }
            
            .policy-container {
                padding: var(--space-xl);
            }
            
            .contact-number {
                font-size: var(--text-3xl);
            }
            
            .footer-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
            
            .social-links {
                justify-content: center;
            }
        }
        
        @media (max-width: 576px) {
            h1 {
                font-size: var(--text-3xl);
            }
            
            h2 {
                font-size: var(--text-xl);
            }
            
            .btn {
                padding: 15px 30px;
                font-size: var(--text-base);
            }
            
            .service-card {
                padding: var(--space-lg);
            }
            
            .service-name {
                font-size: var(--text-2xl);
            }
            
            .service-price {
                font-size: var(--text-3xl);
            }
            
            .policy-container {
                padding: var(--space-lg);
            }
            
            .contact-container {
                padding: var(--space-xl);
            }
            
            .contact-number {
                font-size: var(--text-2xl);
            }
        }
    </style>
</head>
<body>
    <!-- HEADER -->
    <header class="header" id="header">
        <div class="container header-container">
            <a href="#" class="logo">
                <div class="logo-main">Blink & Glam</div>
                <div class="logo-sub">by Elly</div>
            </a>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav class="nav" id="nav">
                <a href="#home" class="nav-link active">Home</a>
                <a href="#services" class="nav-link">Services</a>
                <a href="#policy" class="nav-link">Policy</a>
                <a href="#contact" class="nav-link">Contact</a>
                <a href="tel:0816228731" class="btn btn-secondary">Book Now</a>
            </nav>
        </div>
    </header>

    <!-- MAIN CONTENT -->
    <main>
        <!-- HERO SECTION -->
        <section class="hero" id="home">
            <div class="container">
                <div class="hero-content">
                    <h1 class="hero-title">Premium Lash Artistry</h1>
                    <div class="hero-divider"></div>
                    <p class="hero-subtitle">Luxury Eyelash Extensions Studio</p>
                    <p class="hero-location">Windhoek, Namibia</p>
                    
                    <div class="hero-cta">
                        <a href="#contact" class="btn btn-primary">
                            <i class="fas fa-calendar-check"></i> Book Appointment
                        </a>
                        <a href="#services" class="btn btn-secondary">
                            <i class="fas fa-list-alt"></i> View Services
                        </a>
                    </div>
                </div>
            </div>
        </section>

        <!-- SERVICES SECTION -->
        <section class="section services" id="services">
            <div class="container">
                <h2 class="section-title">Premium Lash Services</h2>
                <p class="section-subtitle">
                    Experience the finest lash extensions in Windhoek. Each service is performed with precision using premium products and techniques.
                </p>
                
                <div class="services-grid">
                    <!-- Service 1 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Cluster Lashes</h3>
                            <div class="service-price">N$100</div>
                        </div>
                        <p class="service-description">
                            Perfect for beginners or those seeking a subtle enhancement. Cluster lashes are lightweight groupings applied to give the appearance of fuller lashes without the commitment of individual extensions.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Quick Application</span>
                            <span class="service-feature">Lightweight</span>
                            <span class="service-feature">Temporary Option</span>
                            <span class="service-feature">Perfect for Events</span>
                        </div>
                    </div>
                    
                    <!-- Service 2 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Yy Lashes</h3>
                            <div class="service-price">N$150</div>
                        </div>
                        <p class="service-description">
                            The YY technique creates a beautiful, wispy effect by attaching two extensions in a Y-formation to a single natural lash. This method adds significant volume while maintaining a feathery, natural appearance.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Wispy Effect</span>
                            <span class="service-feature">Volume & Length</span>
                            <span class="service-feature">Feathery Appearance</span>
                            <span class="service-feature">Dramatic Yet Natural</span>
                        </div>
                    </div>
                    
                    <!-- Service 3 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">W Lashes</h3>
                            <div class="service-price">N$160</div>
                        </div>
                        <p class="service-description">
                            W lashes create a stunning cat-eye effect that elongates and lifts the eyes. This technique involves placing shorter lashes at the inner corner and gradually increasing length toward the outer corner.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Cat-Eye Effect</span>
                            <span class="service-feature">Eye-Lifting</span>
                            <span class="service-feature">Glamorous</span>
                            <span class="service-feature">Almond-Shaped Eyes</span>
                        </div>
                    </div>
                    
                    <!-- Service 4 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Clover Lashes</h3>
                            <div class="service-price">N$170</div>
                        </div>
                        <p class="service-description">
                            Our signature clover technique creates unique, multi-dimensional fans that resemble a four-leaf clover. This advanced method provides maximum volume while maintaining an incredibly lightweight feel.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Maximum Volume</span>
                            <span class="service-feature">Multi-Dimensional</span>
                            <span class="service-feature">Lightweight Feel</span>
                            <span class="service-feature">Signature Technique</span>
                        </div>
                    </div>
                    
                    <!-- Service 5 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Classic Lashes</h3>
                            <div class="service-price">N$180</div>
                        </div>
                        <p class="service-description">
                            The timeless 1:1 extension technique applies a single extension to each natural lash. This method enhances your natural lashes with added length and curl while maintaining a completely natural appearance.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">1:1 Application</span>
                            <span class="service-feature">Natural Enhancement</span>
                            <span class="service-feature">Everyday Wear</span>
                            <span class="service-feature">Timeless Look</span>
                        </div>
                    </div>
                    
                    <!-- Service 6 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">10D Volume Lashes</h3>
                            <div class="service-price">N$200</div>
                        </div>
                        <p class="service-description">
                            Our most luxurious service featuring ultra-fine extensions handcrafted into 10D fans. Each fan contains ten ultra-lightweight extensions applied to a single natural lash, creating incredible volume without heaviness.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Ultra Volume</span>
                            <span class="service-feature">Handcrafted Fans</span>
                            <span class="service-feature">Luxury Service</span>
                            <span class="service-feature">Most Dramatic</span>
                        </div>
                    </div>
                    
                    <!-- Service 7 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Foreign Work Refill</h3>
                            <div class="service-price">N$100</div>
                        </div>
                        <p class="service-description">
                            Expert refill service for extensions applied at another studio. We carefully assess the existing work, remove any grown-out or damaged extensions, and apply fresh extensions to restore fullness.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Expert Assessment</span>
                            <span class="service-feature">Careful Refill</span>
                            <span class="service-feature">Restoration</span>
                            <span class="service-feature">Quality Check</span>
                        </div>
                    </div>
                    
                    <!-- Service 8 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Own Work Refill</h3>
                            <div class="service-price">N$80</div>
                        </div>
                        <p class="service-description">
                            Maintenance refill for extensions originally applied by us. We maintain the integrity of our work by carefully removing grown-out extensions and applying fresh ones to keep your lashes looking full and beautiful.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Maintenance Service</span>
                            <span class="service-feature">Consistent Quality</span>
                            <span class="service-feature">Fresh Appearance</span>
                            <span class="service-feature">2-3 Week Interval</span>
                        </div>
                    </div>
                    
                    <!-- Service 9 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">Professional Removal</h3>
                            <div class="service-price">N$50</div>
                        </div>
                        <p class="service-description">
                            Safe, professional removal of lash extensions using specialized adhesive remover that gently breaks down the bond without damaging your natural lashes. Never attempt to remove extensions at home.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Safe Removal</span>
                            <span class="service-feature">No Damage</span>
                            <span class="service-feature">Professional Grade</span>
                            <span class="service-feature">Lash Health</span>
                        </div>
                    </div>
                    
                    <!-- Service 10 -->
                    <div class="card service-card">
                        <div class="service-header">
                            <h3 class="service-name">House Calls</h3>
                            <div class="service-price">N$40</div>
                        </div>
                        <p class="service-description">
                            Luxury mobile service bringing our studio experience to your location. We provide all professional equipment, sterilization protocols, and premium products in the comfort of your home.
                        </p>
                        <div class="service-features">
                            <span class="service-feature">Mobile Service</span>
                            <span class="service-feature">Convenience</span>
                            <span class="service-feature">Privacy</span>
                            <span class="service-feature">Full Studio Setup</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- POLICY SECTION -->
        <section class="section policy" id="policy">
            <div class="container">
                <h2 class="section-title">Studio Policy & Guidelines</h2>
                <p class="section-subtitle">
                    To ensure the best experience for all clients, please review our studio policies before booking your appointment.
                </p>
                
                <div class="policy-container">
                    <div class="policy-grid">
                        <!-- Policy 1 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-money-check-alt"></i>
                            </div>
                            <div class="policy-content">
                                <h3>50% Deposit Required</h3>
                                <p>A non-refundable 50% deposit is required at the time of booking to secure your appointment. This deposit will be applied toward your total service cost. The deposit guarantees your reserved time slot and covers preparation and materials allocated for your appointment.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 2 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-calendar-check"></i>
                            </div>
                            <div class="policy-content">
                                <h3>By Secured Appointment Only</h3>
                                <p>All services are exclusively by secured appointment. We do not accept walk-ins to ensure we can provide focused, uninterrupted, and quality service to each client. Appointments can be made via phone call or direct message, with confirmation sent once deposit is received.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 3 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-user-friends"></i>
                            </div>
                            <div class="policy-content">
                                <h3>No Extra Accompany Allowed</h3>
                                <p>Due to the intimate size of our studio and to maintain a calm, relaxing environment for all clients, we cannot accommodate extra persons during appointments. This policy ensures optimal focus during the procedure and respects the privacy and comfort of all clients.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 4 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-clock"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Punctuality Appreciated</h3>
                                <p>Please arrive at your scheduled time. Late arrivals may result in shortened service time to accommodate following appointments. If you are more than 15 minutes late without prior notice, your appointment may be rescheduled and deposit forfeited.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 5 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-eye-slash"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Removal Notification Required</h3>
                                <p>Kindly indicate when booking if you require removal service. Additional time will be scheduled to ensure proper, safe removal without rushing. Attempting to remove extensions at home can damage natural lashes, so professional removal is strongly recommended.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 6 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-ban"></i>
                            </div>
                            <div class="policy-content">
                                <h3>48-Hour Cancellation Policy</h3>
                                <p>Cancellations within 48 hours of your appointment will forfeit the deposit. Rescheduling requires at least 24-hour notice to transfer your deposit to a new appointment time. No-shows without communication will forfeit deposit and may require full prepayment for future bookings.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 7 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-syringe"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Health & Safety Protocols</h3>
                                <p>All tools are sterilized between clients, and disposable items are used whenever possible. Please arrive with clean, makeup-free eyes. If you have any eye infections, recent surgeries, or medical conditions affecting your eyes, please reschedule for your safety.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 8 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-allergies"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Patch Testing & Allergies</h3>
                                <p>First-time clients are recommended to schedule a patch test 48 hours before their full appointment if you have sensitive skin or known allergies. While allergic reactions are rare, this precaution ensures your safety and comfort during the procedure.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 9 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-hand-holding-usd"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Payment Methods</h3>
                                <p>We accept cash and electronic transfers. Full payment is due at the conclusion of your service. Prices are subject to change, but you will be charged the rate quoted at the time of booking. Gratuities are appreciated but never expected.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 10 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-child"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Age Requirement</h3>
                                <p>Clients must be at least 16 years old to receive lash extensions. Minors (16-17 years) must be accompanied by a parent or guardian who must remain present during the consultation and provide written consent for the procedure.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 11 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-home"></i>
                            </div>
                            <div class="policy-content">
                                <h3>House Call Specifics</h3>
                                <p>House calls require a clean, well-lit workspace with access to an electrical outlet. Travel fee applies outside standard service area. Full payment is required at time of service for house calls. Cancellation policy for house calls is 72 hours due to travel preparation.</p>
                            </div>
                        </div>
                        
                        <!-- Policy 12 -->
                        <div class="policy-item">
                            <div class="policy-icon">
                                <i class="fas fa-heart"></i>
                            </div>
                            <div class="policy-content">
                                <h3>Aftercare Responsibility</h3>
                                <p>Proper aftercare is essential for lash retention and health. You will receive detailed aftercare instructions. Failure to follow aftercare guidelines may affect the longevity of your extensions and could impact eligibility for refill pricing.</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="policy-note">
                        <h4>Important Note</h4>
                        <p>By booking an appointment, you acknowledge that you have read, understood, and agree to all studio policies. We reserve the right to refuse service to anyone who does not comply with these guidelines. Your safety, comfort, and satisfaction are our top priorities.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- CONTACT SECTION -->
        <section class="section contact" id="contact">
            <div class="container">
                <div class="contact-container">
                    <h2 class="contact-title">Book Your Appointment</h2>
                    <p class="contact-subtitle">
                        Experience the luxury of premium lash extensions in our Windhoek studio. Contact us directly to schedule your appointment. 
                        All bookings require a 50% deposit to secure your preferred time. We recommend booking 2-3 weeks in advance for optimal availability.
                    </p>
                    
                    <div class="contact-number">081 622 8731</div>
                    
                    <div class="text-center">
                        <a href="tel:0816228731" class="btn btn-primary">
                            <i class="fas fa-phone-alt"></i> Call Now to Book
                        </a>
                    </div>
                    
                    <div class="contact-details">
                        <div class="contact-detail">
                            <i class="fas fa-map-marker-alt"></i>
                            <h3>Studio Location</h3>
                            <p>Windhoek, Namibia</p>
                            <p style="color: var(--light-gold); margin-top: 10px; font-size: 0.95rem;">Private studio by appointment only</p>
                        </div>
                        
                        <div class="contact-detail">
                            <i class="fas fa-clock"></i>
                            <h3>Operating Hours</h3>
                            <p>Monday - Saturday: 9AM - 6PM</p>
                            <p style="color: var(--light-gold); margin-top: 10px; font-size: 0.95rem;">By secured appointment only</p>
                        </div>
                        
                        <div class="contact-detail">
                            <i class="fas fa-calendar-alt"></i>
                            <h3>Booking Requirements</h3>
                            <p>50% deposit required</p>
                            <p style="color: var(--light-gold); margin-top: 10px; font-size: 0.95rem;">48-hour cancellation policy applies</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- FOOTER -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>BLINK & GLAM BY ELLY</h3>
                    <p>Premium eyelash extension studio in Windhoek, Namibia. Specializing in custom lash artistry with attention to detail, client comfort, and exceptional results.</p>
                    <div class="social-links">
                        <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="social-link"><i class="fab fa-whatsapp"></i></a>
                        <a href="#" class="social-link"><i class="fas fa-envelope"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul style="list-style: none; padding: 0;">
                        <li><a href="#home" style="color: var(--golden-yellow);">Home</a></li>
                        <li><a href="#services" style="color: var(--golden-yellow);">Services</a></li>
                        <li><a href="#policy" style="color: var(--golden-yellow);">Policy</a></li>
                        <li><a href="#contact" style="color: var(--golden-yellow);">Contact</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Contact Info</h3>
                    <p><i class="fas fa-phone" style="color: var(--golden-yellow);"></i> 081 622 8731</p>
                    <p><i class="fas fa-map-marker-alt" style="color: var(--golden-yellow);"></i> Windhoek, Namibia</p>
                    <p><i class="fas fa-clock" style="color: var(--golden-yellow);"></i> By Appointment Only</p>
                    <p><i class="fas fa-money-check" style="color: var(--golden-yellow);"></i> 50% Deposit Required</p>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p class="copyright">
                    &copy; 2025 BLINK & GLAM BY ELLY. All rights reserved.<br>
                    Premium Eyelash Extensions Studio | Certified Technician | Professional Lash Artist
                </p>
            </div>
        </div>
    </footer>

    <script>
        // Header Scroll Effect
        window.addEventListener('scroll', function() {
            const header = document.getElementById('header');
            if (window.scrollY > 100) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const nav = document.getElementById('nav');
        
        mobileMenuBtn.addEventListener('click', function() {
            nav.classList.toggle('active');
            mobileMenuBtn.innerHTML = nav.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });

        // Close mobile menu when clicking a link
        document.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', function() {
                nav.classList.remove('active');
                mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });

        // Smooth Scrolling for Navigation Links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 100,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Set active navigation link based on scroll position
        window.addEventListener('scroll', function() {
            const sections = document.querySelectorAll('section[id]');
            const scrollPosition = window.scrollY + 150;
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                const sectionId = section.getAttribute('id');
                
                if (scrollPosition >= sectionTop && scrollPosition < sectionTop + sectionHeight) {
                    document.querySelectorAll('.nav-link').forEach(link => {
                        link.classList.remove('active');
                        if (link.getAttribute('href') === `#${sectionId}`) {
                            link.classList.add('active');
                        }
                    });
                }
            });
        });

        // Add hover effect to cards
        document.querySelectorAll('.card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-20px) scale(1.02)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0) scale(1)';
            });
        });

        // Current year for copyright
        document.querySelectorAll('.copyright').forEach(el => {
            el.innerHTML = el.innerHTML.replace('2025', new Date().getFullYear());
        });
    </script>
</body>
</html>
