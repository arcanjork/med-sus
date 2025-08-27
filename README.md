<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MedSUS - Triagem Médica Inteligente do Sistema Único de Saúde</title>
    <meta name="description" content="Plataforma de triagem médica inteligente do SUS com tecnologia avançada para orientação preliminar e gestão eficiente de recursos de saúde pública.">
    <meta name="keywords" content="SUS, triagem médica, saúde pública, sistema único de saúde, telemedicina, diagnóstico preliminar">
    <meta name="author" content="MedSUS">
    <meta name="robots" content="index, follow">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://medsus.gov.br/">
    <meta property="og:title" content="MedSUS - Triagem Médica Inteligente do SUS">
    <meta property="og:description" content="Plataforma de triagem médica inteligente do SUS com tecnologia avançada para orientação preliminar e gestão eficiente de recursos.">
    <meta property="og:image" content="https://medsus.gov.br/images/og-image.jpg">
    <meta property="og:locale" content="pt_BR">
    
    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://medsus.gov.br/">
    <meta property="twitter:title" content="MedSUS - Triagem Médica Inteligente do SUS">
    <meta property="twitter:description" content="Plataforma de triagem médica inteligente do SUS com tecnologia avançada para orientação preliminar.">
    <meta property="twitter:image" content="https://medsus.gov.br/images/twitter-image.jpg">
    
    <!-- Favicon -->
    <link rel="icon" type="image/x-icon" href="/favicon.ico">
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
    
    <!-- Preload critical resources -->
    <link rel="preload" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
    <noscript><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"></noscript>
    
    <!-- JSON-LD Schema -->
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "Organization",
        "name": "MedSUS",
        "description": "Plataforma de triagem médica inteligente do Sistema Único de Saúde",
        "url": "https://medsus.gov.br",
        "logo": "https://medsus.gov.br/images/logo.png",
        "contactPoint": {
            "@type": "ContactPoint",
            "telephone": "136",
            "contactType": "customer service",
            "availableLanguage": "Portuguese"
        },
        "sameAs": [
            "https://www.facebook.com/medsus",
            "https://www.twitter.com/medsus"
        ]
    }
    </script>
    
    <style>
        /* CSS Custom Properties */
        :root {
            --brand-primary: #0ea5e9;
            --brand-secondary: #e63946;
            --accent-color: #ffd700;
            --bg-primary: #ffffff;
            --bg-secondary: #f8f9fa;
            --bg-tertiary: #e9ecef;
            --text-primary: #212529;
            --text-secondary: #6c757d;
            --text-light: #ffffff;
            --border-color: #dee2e6;
            --shadow-sm: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075);
            --shadow-md: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
            --shadow-lg: 0 1rem 3rem rgba(0, 0, 0, 0.175);
            --border-radius: 0.375rem;
            --border-radius-lg: 0.5rem;
            --border-radius-xl: 1rem;
            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            --font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        /* Dark mode support */
        @media (prefers-color-scheme: dark) {
            :root {
                --bg-primary: #1a1a1a;
                --bg-secondary: #2d2d2d;
                --bg-tertiary: #404040;
                --text-primary: #ffffff;
                --text-secondary: #b3b3b3;
                --border-color: #404040;
            }
        }

        /* Reset and base styles */
        *, *::before, *::after {
            box-sizing: border-box;
        }

        * {
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-family);
            line-height: 1.6;
            color: var(--text-primary);
            background-color: var(--bg-primary);
            overflow-x: hidden;
        }

        /* Skip link */
        .skip-link {
            position: absolute;
            top: -40px;
            left: 6px;
            background: var(--brand-primary);
            color: var(--text-light);
            padding: 8px;
            text-decoration: none;
            border-radius: var(--border-radius);
            z-index: 9999;
            font-weight: 600;
        }

        .skip-link:focus {
            top: 6px;
        }

        /* Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem;
        }

        /* Utility classes */
        .sr-only {
            position: absolute;
            width: 1px;
            height: 1px;
            padding: 0;
            margin: -1px;
            overflow: hidden;
            clip: rect(0, 0, 0, 0);
            white-space: nowrap;
            border: 0;
        }

        .focus-visible:focus-visible {
            outline: 2px solid var(--brand-primary);
            outline-offset: 2px;
        }

        /* Top Bar */
        .top-bar {
            background: linear-gradient(135deg, var(--brand-primary) 0%, #1e40af 100%);
            color: var(--text-light);
            padding: 0.5rem 0;
            font-size: 0.875rem;
        }

        .top-bar .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .top-links {
            display: flex;
            gap: 1.5rem;
            flex-wrap: wrap;
        }

        .top-links a {
            color: var(--text-light);
            text-decoration: none;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .top-links a:hover,
        .top-links a:focus-visible {
            opacity: 0.8;
            text-decoration: underline;
        }

        .top-buttons {
            display: flex;
            gap: 1rem;
            align-items: center;
        }

        .btn-text {
            color: var(--text-light);
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            padding: 0.25rem 0.5rem;
            border-radius: var(--border-radius);
        }

        .btn-text:hover,
        .btn-text:focus-visible {
            background: rgba(255, 255, 255, 0.1);
            text-decoration: none;
        }

        .btn-outline-sm {
            color: var(--text-light);
            text-decoration: none;
            border: 1px solid var(--text-light);
            padding: 0.375rem 1rem;
            border-radius: 1.25rem;
            font-size: 0.8125rem;
            font-weight: 500;
            transition: var(--transition);
        }

        .btn-outline-sm:hover,
        .btn-outline-sm:focus-visible {
            background: var(--text-light);
            color: var(--brand-primary);
            text-decoration: none;
        }

        /* Header */
        .main-header {
            background: var(--bg-primary);
            box-shadow: var(--shadow-md);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 1rem;
            min-height: 100px;
            gap: 2rem;
        }

        .logo {
            text-decoration: none;
            display: flex;
            align-items: center;
            flex-shrink: 0;
        }

        .logo svg {
            width: 240px;
            height: auto;
        }

        /* Navigation */
        .main-nav {
            display: flex;
            gap: 1.5rem;
            list-style: none;
            flex: 1;
            justify-content: center;
        }

        .main-nav a {
            text-decoration: none;
            color: var(--text-primary);
            font-weight: 500;
            padding: 0.75rem 1rem;
            position: relative;
            transition: var(--transition);
            border-radius: var(--border-radius);
            white-space: nowrap;
        }

        .main-nav a:hover,
        .main-nav a:focus-visible {
            color: var(--brand-secondary);
            background: rgba(230, 57, 70, 0.1);
        }

        .main-nav a[aria-current="page"] {
            color: var(--brand-secondary);
            background: rgba(230, 57, 70, 0.1);
        }

        .main-nav a[aria-current="page"]::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80%;
            height: 2px;
            background: var(--brand-secondary);
            border-radius: 1px;
        }

        /* Header actions */
        .header-actions {
            display: flex;
            gap: 1rem;
            align-items: center;
        }

        .btn-icon {
            background: none;
            border: none;
            font-size: 1.125rem;
            color: var(--text-secondary);
            cursor: pointer;
            padding: 0.75rem;
            border-radius: 50%;
            transition: var(--transition);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .btn-icon:hover,
        .btn-icon:focus-visible {
            background: var(--bg-secondary);
            color: var(--brand-secondary);
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--brand-secondary) 0%, #dc2626 100%);
            color: var(--text-light);
            border: none;
            padding: 0.75rem 1.25rem;
            border-radius: 1.5rem;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 0.5rem;
            text-decoration: none;
            font-size: 0.875rem;
        }

        .btn-primary:hover,
        .btn-primary:focus-visible {
            transform: translateY(-2px);
            box-shadow: 0 0.5rem 1rem rgba(230, 57, 70, 0.3);
            text-decoration: none;
            color: var(--text-light);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.25rem;
            cursor: pointer;
            padding: 0.75rem;
            color: var(--text-primary);
            border-radius: var(--border-radius);
        }

        .mobile-menu-btn:hover,
        .mobile-menu-btn:focus-visible {
            background: var(--bg-secondary);
        }

        /* Search Bar */
        .search-section {
            background: linear-gradient(135deg, var(--bg-secondary) 0%, var(--bg-tertiary) 100%);
            padding: 1.5rem 0;
            border-bottom: 1px solid var(--border-color);
        }

        .search-form {
            display: flex;
            align-items: center;
            background: var(--bg-primary);
            border-radius: 3rem;
            padding: 0.375rem;
            box-shadow: var(--shadow-lg);
            max-width: 50rem;
            margin: 0 auto;
            border: 1px solid var(--border-color);
        }

        .search-icon {
            color: var(--text-secondary);
            margin-left: 1.25rem;
            margin-right: 1rem;
            font-size: 1rem;
        }

        .search-input {
            flex: 1;
            border: none;
            outline: none;
            padding: 1rem 0;
            font-size: 1rem;
            background: transparent;
            color: var(--text-primary);
        }

        .search-input::placeholder {
            color: var(--text-secondary);
        }

        .search-submit {
            margin: 0;
            border-radius: 2.5rem;
            padding: 1rem 1.5rem;
            white-space: nowrap;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: var(--text-light);
            padding: 5rem 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="20" cy="20" r="2" fill="rgba(255,255,255,0.1)"/><circle cx="80" cy="40" r="1" fill="rgba(255,255,255,0.1)"/><circle cx="40" cy="80" r="1.5" fill="rgba(255,255,255,0.1)"/></svg>');
            animation: float 20s infinite linear;
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: clamp(2rem, 5vw, 3.5rem);
            font-weight: 700;
            margin-bottom: 1.25rem;
            line-height: 1.2;
        }

        .hero h1 .highlight {
            color: var(--accent-color);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero-subtitle {
            font-size: clamp(1rem, 2.5vw, 1.3rem);
            margin-bottom: 2.5rem;
            opacity: 0.9;
            max-width: 37.5rem;
            margin-left: auto;
            margin-right: auto;
        }

        /* Stats Grid */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-top: 4rem;
            list-style: none;
        }

        .stat-card {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            border-radius: var(--border-radius-xl);
            padding: 2rem;
            text-align: center;
            border: 1px solid rgba(255,255,255,0.2);
            transition: var(--transition);
        }

        .stat-card:hover {
            transform: translateY(-5px);
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--accent-color);
            display: block;
            margin-bottom: 0.625rem;
        }

        .stat-label {
            font-size: 1rem;
            opacity: 0.9;
        }

        /* Content Sections */
        .content-section {
            padding: 5rem 0;
        }

        .content-section:nth-child(even) {
            background: var(--bg-secondary);
        }

        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-title {
            font-size: clamp(2rem, 4vw, 3rem);
            font-weight: 700;
            color: var(--text-primary);
            margin-bottom: 1rem;
        }

        .section-subtitle {
            font-size: 1.25rem;
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
        }

        /* How it Works Section */
        .steps-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .step-card {
            background: var(--bg-primary);
            border-radius: var(--border-radius-xl);
            padding: 2.5rem;
            text-align: center;
            box-shadow: var(--shadow-md);
            border: 1px solid var(--border-color);
            transition: var(--transition);
            position: relative;
        }

        .step-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-lg);
        }

        .step-number {
            position: absolute;
            top: -1.5rem;
            left: 50%;
            transform: translateX(-50%);
            background: linear-gradient(135deg, var(--brand-secondary) 0%, #dc2626 100%);
            color: var(--text-light);
            width: 3rem;
            height: 3rem;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 1.25rem;
        }

        .step-icon {
            font-size: 3rem;
            color: var(--brand-primary);
            margin-bottom: 1.5rem;
        }

        .step-title {
            font-size: 1.5rem;
            font-weight: 600;
            color: var(--text-primary);
            margin-bottom: 1rem;
        }

        .step-description {
            color: var(--text-secondary);
            line-height: 1.6;
        }

        /* About Project Section */
        .about-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 4rem;
            align-items: center;
        }

        .about-content h3 {
            font-size: 1.75rem;
            font-weight: 600;
            color: var(--text-primary);
            margin-bottom: 1.5rem;
        }

        .about-content p {
            color: var(--text-secondary);
            margin-bottom: 1.5rem;
            line-height: 1.7;
        }

        .features-list {
            list-style: none;
            margin-top: 2rem;
        }

        .features-list li {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
            color: var(--text-secondary);
        }

        .features-list .icon {
            color: var(--brand-secondary);
            font-size: 1.25rem;
            min-width: 1.5rem;
        }

        .about-visual {
            background: linear-gradient(135deg, var(--brand-primary) 0%, var(--brand-secondary) 100%);
            border-radius: var(--border-radius-xl);
            padding: 3rem;
            color: var(--text-light);
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .about-visual::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="25" cy="25" r="3" fill="rgba(255,255,255,0.1)"/><circle cx="75" cy="75" r="2" fill="rgba(255,255,255,0.1)"/><circle cx="50" cy="10" r="1" fill="rgba(255,255,255,0.1)"/></svg>');
            opacity: 0.3;
        }

        .visual-content {
            position: relative;
            z-index: 2;
        }

        .visual-icon {
            font-size: 4rem;
            margin-bottom: 1.5rem;
            opacity: 0.9;
        }

        .visual-title {
            font-size: 1.75rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .visual-stats {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .visual-stat {
            text-align: center;
        }

        .visual-stat-number {
            font-size: 2rem;
            font-weight: 700;
            display: block;
            margin-bottom: 0.5rem;
        }

        .visual-stat-label {
            font-size: 0.875rem;
            opacity: 0.8;
        }

        /* LGPD Cookie Banner */
        .cookie-banner {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: var(--bg-primary);
            border-top: 1px solid var(--border-color);
            padding: 1.5rem;
            box-shadow: var(--shadow-lg);
            z-index: 9999;
            transform: translateY(100%);
            transition: var(--transition);
        }

        .cookie-banner.show {
            transform: translateY(0);
        }

        .cookie-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .cookie-text {
            flex: 1;
            min-width: 300px;
        }

        .cookie-actions {
            display: flex;
            gap: 1rem;
            flex-wrap: wrap;
        }

        .btn-secondary {
            background: var(--bg-secondary);
            color: var(--text-primary);
            border: 1px solid var(--border-color);
            padding: 0.75rem 1.25rem;
            border-radius: var(--border-radius-lg);
            font-weight: 500;
            cursor: pointer;
            transition: var(--transition);
            text-decoration: none;
            display: inline-flex;
            align-items: center;
        }

        .btn-secondary:hover,
        .btn-secondary:focus-visible {
            background: var(--bg-tertiary);
            text-decoration: none;
            color: var(--text-primary);
        }

        /* Footer */
        .main-footer {
            background: var(--bg-secondary);
            padding: 2rem 0 1rem;
            border-top: 1px solid var(--border-color);
            margin-top: 4rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            font-size: 1.125rem;
            font-weight: 600;
            margin-bottom: 1rem;
            color: var(--text-primary);
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 0.5rem;
        }

        .footer-links a {
            color: var(--text-secondary);
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover,
        .footer-links a:focus-visible {
            color: var(--brand-primary);
            text-decoration: underline;
        }

        .footer-bottom {
            border-top: 1px solid var(--border-color);
            padding-top: 1rem;
            text-align: center;
            color: var(--text-secondary);
            font-size: 0.875rem;
        }

        /* Responsive Design */
        @media (max-width: 1024px) {
            .container {
                padding: 0 1.5rem;
            }
        }

        @media (max-width: 768px) {
            .top-bar .container {
                flex-direction: column;
                text-align: center;
            }

            .header-container {
                padding: 1rem;
                min-height: 80px;
                gap: 1rem;
            }

            .logo svg {
                width: 200px;
            }

            .main-nav {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                right: 0;
                background: var(--bg-primary);
                box-shadow: var(--shadow-lg);
                padding: 1.5rem;
                flex-direction: column;
                gap: 0;
                border-top: 1px solid var(--border-color);
                justify-content: flex-start;
            }

            .main-nav.show {
                display: flex;
            }

            .main-nav li {
                border-bottom: 1px solid var(--border-color);
            }

            .main-nav li:last-child {
                border-bottom: none;
            }

            .main-nav a {
                display: block;
                padding: 1rem 0;
                text-align: center;
            }

            .mobile-menu-btn {
                display: block;
            }

            .header-actions {
                gap: 0.5rem;
                flex-shrink: 0;
            }

            .search-form {
                flex-direction: column;
                border-radius: var(--border-radius-xl);
                padding: 1.5rem;
                gap: 1rem;
            }

            .search-input {
                text-align: center;
                padding: 0.75rem;
                border: 1px solid var(--border-color);
                border-radius: var(--border-radius-lg);
            }

            .search-submit {
                width: 100%;
                justify-content: center;
            }

            .cookie-content {
                flex-direction: column;
                text-align: center;
            }

            .cookie-actions {
                justify-content: center;
            }

            .steps-grid {
                grid-template-columns: 1fr;
            }

            .about-grid {
                grid-template-columns: 1fr;
                gap: 2rem;
            }

            .visual-stats {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 480px) {
            .header-container {
                padding: 0.75rem;
                min-height: 70px;
            }

            .logo svg {
                width: 160px;
            }

            .hero {
                padding: 3rem 0;
            }

            .stats-grid {
                grid-template-columns: 1fr;
                gap: 1rem;
            }

            .stat-card {
                padding: 1.5rem;
            }

            .stat-number {
                font-size: 2rem;
            }

            .top-links {
                flex-direction: column;
                gap: 0.5rem;
            }

            .top-buttons {
                flex-direction: column;
                gap: 0.5rem;
            }

            .content-section {
                padding: 3rem 0;
            }

            .step-card {
                padding: 2rem 1.5rem;
            }
        }

        /* Print styles */
        @media print {
            .top-bar,
            .search-section,
            .header-actions,
            .cookie-banner {
                display: none;
            }
            
            .hero {
                background: none;
                color: black;
            }
        }

        /* Reduced motion */
        @media (prefers-reduced-motion: reduce) {
            *,
            *::before,
            *::after {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
            }
        }
    </style>
</head>
<body>
    <!-- Skip Link -->
    <a href="#main-content" class="skip-link focus-visible">Pular para o conteúdo</a>

    <!-- Top Bar -->
    <div class="top-bar">
        <div class="container">
            <div class="top-links">
                <a href="tel:136" aria-label="Ligar para Central de Atendimento do SUS">
                    <i class="fas fa-phone-alt" aria-hidden="true"></i>
                    136 - Central de Atendimento
                </a>
                <a href="#" aria-label="Encontrar Unidade Básica de Saúde próxima">
                    <i class="fas fa-map-marker-alt" aria-hidden="true"></i>
                    Encontre uma UBS
                </a>
            </div>
            <div class="top-buttons">
                <a href="#" class="btn-text focus-visible">Área Médica</a>
                <a href="#" class="btn-outline-sm focus-visible">Acessar</a>
            </div>
        </div>
    </div>

    <!-- Main Header -->
    <header class="main-header">
        <div class="container">
            <div class="header-container">
                <a href="#hero" class="logo focus-visible" aria-label="MedSUS - Página inicial">
                    <svg width="280" height="140" viewBox="0 0 700 220" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="logo-title">
                        <title id="logo-title">Logotipo MedSUS</title>
                        <path d="M140 60 C 120 40, 80 40, 80 80 C 80 110, 140 150, 140 150 C 140 150, 200 110, 200 80 C 200 40, 160 40, 140 60 Z" fill="#E63946"/>
                        <rect x="135" y="85" width="10" height="30" fill="#FFFFFF"/>
                        <rect x="125" y="95" width="30" height="10" fill="#FFFFFF"/>
                        <path d="M60 105 L100 105 L110 85 L120 125 L130 105 L180 105" stroke="#FFFFFF" stroke-width="3" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
                        <text x="250" y="100" font-size="72" font-family="Arial, Helvetica, sans-serif" font-weight="700" fill="#222222">MED</text>
                        <text x="250" y="160" font-size="72" font-family="Arial, Helvetica, sans-serif" font-weight="700" fill="#222222">SUS</text>
                    </svg>
                </a>

                <nav aria-label="Navegação principal">
                    <ul class="main-nav" id="main-nav">
                        <li><a href="#hero" aria-current="page" class="focus-visible nav-link">Início</a></li>
                        <li><a href="#como-funciona" class="focus-visible nav-link">Como Funciona</a></li>
                        <li><a href="#" class="focus-visible">Para Unidades de Saúde</a></li>
                        <li><a href="#sobre-projeto" class="focus-visible nav-link">Sobre o Projeto</a></li>
                        <li><a href="#" class="focus-visible">Contato</a></li>
                    </ul>
                </nav>

                <div class="header-actions">
                    <button class="btn-icon search-btn focus-visible" 
                            aria-label="Expandir busca" 
                            aria-expanded="false" 
                            aria-controls="search-section">
                        <i class="fas fa-search" aria-hidden="true"></i>
                    </button>
                    <a href="#" class="btn-primary focus-visible" aria-label="Fazer login no sistema">
                        <i class="fas fa-user" aria-hidden="true"></i>
                        Entrar
                    </a>
                    <button class="mobile-menu-btn focus-visible" 
                            aria-label="Abrir menu de navegação" 
                            aria-expanded="false" 
                            aria-controls="main-nav">
                        <i class="fas fa-bars" aria-hidden="true"></i>
                    </button>
                </div>
            </div>
        </div>
    </header>

    <!-- Search Section -->
    <section class="search-section" id="search-section" aria-label="Busca de sintomas">
        <div class="container">
            <form class="search-form" role="search" aria-label="Analisar sintomas">
                <i class="fas fa-search search-icon" aria-hidden="true"></i>
                <label for="symptom-input" class="sr-only">Descreva seus sintomas</label>
                <input type="text" 
                       id="symptom-input" 
                       class="search-input focus-visible" 
                       placeholder="Descreva seus sintomas (ex.: dor de cabeça, febre, náuseas)"
                       aria-describedby="search-help">
                <button type="submit" class="btn-primary search-submit focus-visible">
                    <i class="fas fa-stethoscope" aria-hidden="true"></i>
                    Analisar
                </button>
            </form>
            <div id="search-help" class="sr-only">
                Digite seus sintomas para receber orientação médica preliminar
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <main id="main-content">
        <!-- Hero Section -->
        <section class="hero" id="hero" aria-labelledby="hero-title">
            <div class="container">
                <div class="hero-content">
                    <h1 id="hero-title">
                        Triagem médica <span class="highlight">inteligente</span> para o SUS
                    </h1>
                    <p class="hero-subtitle">
                        Tecnologia avançada para orientação médica preliminar e gestão eficiente de recursos do Sistema Único de Saúde
                    </p>

                    <ul class="stats-grid" aria-label="Estatísticas do sistema">
                        <li class="stat-card">
                            <span class="stat-number" aria-label="98 por cento">98%</span>
                            <span class="stat-label">Precisão na triagem</span>
                        </li>
                        <li class="stat-card">
                            <span class="stat-number" aria-label="45 minutos">45min</span>
                            <span class="stat-label">Redução no tempo de espera</span>
                        </li>
                        <li class="stat-card">
                            <span class="stat-number" aria-label="24 horas por dia, 7 dias por semana">24/7</span>
                            <span class="stat-label">Disponibilidade</span>
                        </li>
                        <li class="stat-card">
                            <span class="stat-number" aria-label="Mais de 500 mil">500k+</span>
                            <span class="stat-label">Pacientes atendidos</span>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Como Funciona Section -->
        <section class="content-section" id="como-funciona" aria-labelledby="como-funciona-title">
            <div class="container">
                <div class="section-header">
                    <h2 id="como-funciona-title" class="section-title">Como Funciona</h2>
                    <p class="section-subtitle">
                        Um processo simples e inteligente para conectar você ao cuidado médico adequado
                    </p>
                </div>

                <div class="steps-grid">
                    <div class="step-card">
                        <div class="step-number">1</div>
                        <div class="step-icon">
                            <i class="fas fa-edit" aria-hidden="true"></i>
                        </div>
                        <h3 class="step-title">Descreva seus Sintomas</h3>
                        <p class="step-description">
                            Digite de forma natural seus sintomas, como "dor de cabeça e febre". Nossa IA compreende linguagem cotidiana e identifica padrões médicos relevantes.
                        </p>
                    </div>

                    <div class="step-card">
                        <div class="step-number">2</div>
                        <div class="step-icon">
                            <i class="fas fa-brain" aria-hidden="true"></i>
                        </div>
                        <h3 class="step-title">Análise Inteligente</h3>
                        <p class="step-description">
                            Algoritmos avançados de IA médica analisam seus sintomas em segundos, comparando com milhares de casos e protocolos clínicos do SUS.
                        </p>
                    </div>

                    <div class="step-card">
                        <div class="step-number">3</div>
                        <div class="step-icon">
                            <i class="fas fa-clipboard-list" aria-hidden="true"></i>
                        </div>
                        <h3 class="step-title">Triagem Personalizada</h3>
                        <p class="step-description">
                            Receba uma avaliação de urgência, recomendações específicas e orientações sobre qual tipo de atendimento buscar no SUS.
                        </p>
                    </div>

                    <div class="step-card">
                        <div class="step-number">4</div>
                        <div class="step-icon">
                            <i class="fas fa-hospital" aria-hidden="true"></i>
                        </div>
                        <h3 class="step-title">Direcionamento Eficiente</h3>
                        <p class="step-description">
                            Seja direcionado para a unidade de saúde mais adequada: UBS para casos leves, UPA para urgências ou SAMU para emergências.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Sobre o Projeto Section -->
        <section class="content-section" id="sobre-projeto" aria-labelledby="sobre-projeto-title">
            <div class="container">
                <div class="section-header">
                    <h2 id="sobre-projeto-title" class="section-title">Sobre o Projeto</h2>
                    <p class="section-subtitle">
                        Inovação tecnológica a serviço da saúde pública brasileira
                    </p>
                </div>

                <div class="about-grid">
                    <div class="about-content">
                        <h3>Transformando o Atendimento no SUS</h3>
                        <p>
                            O MedSUS é uma iniciativa pioneira que combina inteligência artificial com os protocolos médicos do Sistema Único de Saúde para revolucionar a triagem médica no Brasil.
                        </p>
                        <p>
                            Desenvolvido em parceria com profissionais de saúde, gestores públicos e especialistas em tecnologia, nossa plataforma visa otimizar o fluxo de pacientes e melhorar a qualidade do atendimento em todo o país.
                        </p>

                        <ul class="features-list">
                            <li>
                                <i class="fas fa-check-circle icon" aria-hidden="true"></i>
                                <span>Baseado em protocolos oficiais do Ministério da Saúde</span>
                            </li>
                            <li>
                                <i class="fas fa-shield-alt icon" aria-hidden="true"></i>
                                <span>Dados protegidos conforme LGPD e normas de saúde</span>
                            </li>
                            <li>
                                <i class="fas fa-users icon" aria-hidden="true"></i>
                                <span>Desenvolvido com participação de médicos do SUS</span>
                            </li>
                            <li>
                                <i class="fas fa-mobile-alt icon" aria-hidden="true"></i>
                                <span>Acessível em qualquer dispositivo, 24 horas por dia</span>
                            </li>
                            <li>
                                <i class="fas fa-chart-line icon" aria-hidden="true"></i>
                                <span>Melhoria contínua baseada em dados reais</span>
                            </li>
                        </ul>
                    </div>

                    <div class="about-visual">
                        <div class="visual-content">
                            <div class="visual-icon">
                                <i class="fas fa-heartbeat" aria-hidden="true"></i>
                            </div>
                            <h3 class="visual-title">Impacto Real na Saúde Pública</h3>
                            <p>
                                Desde o lançamento, o MedSUS tem transformado a experiência de milhares de brasileiros no acesso aos serviços de saúde.
                            </p>
                            
                            <div class="visual-stats">
                                <div class="visual-stat">
                                    <span class="visual-stat-number">2.1M</span>
                                    <span class="visual-stat-label">Consultas realizadas</span>
                                </div>
                                <div class="visual-stat">
                                    <span class="visual-stat-number">1.2k</span>
                                    <span class="visual-stat-label">Unidades conectadas</span>
                                </div>
                                <div class="visual-stat">
                                    <span class="visual-stat-number">67%</span>
                                    <span class="visual-stat-label">Redução de filas</span>
                                </div>
                                <div class="visual-stat">
                                    <span class="visual-stat-number">4.8★</span>
                                    <span class="visual-stat-label">Avaliação dos usuários</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="main-footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>MedSUS</h3>
                    <p>Plataforma de triagem médica inteligente do Sistema Único de Saúde, desenvolvida para otimizar o atendimento e melhorar o acesso à saúde pública.</p>
                </div>
                <div class="footer-section">
                    <h3>Links Úteis</h3>
                    <ul class="footer-links">
                        <li><a href="#como-funciona" class="focus-visible">Como Funciona</a></li>
                        <li><a href="#" class="focus-visible">Para Profissionais</a></li>
                        <li><a href="#" class="focus-visible">Unidades de Saúde</a></li>
                        <li><a href="#" class="focus-visible">Suporte Técnico</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Informações Legais</h3>
                    <ul class="footer-links">
                        <li><a href="/privacy" class="focus-visible">Política de Privacidade</a></li>
                        <li><a href="/terms" class="focus-visible">Termos de Uso</a></li>
                        <li><a href="/cookies" class="focus-visible">Política de Cookies</a></li>
                        <li><a href="/accessibility" class="focus-visible">Acessibilidade</a></li>
                    </ul>
                </div>
                <div class="footer-section">
                    <h3>Contato</h3>
                    <ul class="footer-links">
                        <li><a href="tel:136" class="focus-visible">136 - Central SUS</a></li>
                        <li><a href="mailto:contato@medsus.gov.br" class="focus-visible">contato@medsus.gov.br</a></li>
                        <li><a href="#" class="focus-visible">Ouvidoria</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2024 MedSUS - Sistema Único de Saúde. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- LGPD Cookie Banner -->
    <div class="cookie-banner" id="cookie-banner" role="dialog" aria-labelledby="cookie-title" aria-describedby="cookie-description">
        <div class="container">
            <div class="cookie-content">
                <div class="cookie-text">
                    <h3 id="cookie-title">Uso de Cookies e Privacidade</h3>
                    <p id="cookie-description">
                        Utilizamos cookies essenciais para o funcionamento do site. Cookies analíticos são opcionais e nos ajudam a melhorar sua experiência.
                        <a href="/privacy" class="focus-visible">Saiba mais sobre nossa política de privacidade</a>.
                    </p>
                </div>
                <div class="cookie-actions">
                    <button class="btn-secondary focus-visible" onclick="acceptEssentialCookies()">
                        Apenas Essenciais
                    </button>
                    <button class="btn-primary focus-visible" onclick="acceptAllCookies()">
                        Aceitar Todos
                    </button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Navigation functionality
        const navLinks = document.querySelectorAll('.nav-link');
        
        if (navLinks.length > 0) {
            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    // Remove active state from all links
                    navLinks.forEach(l => l.removeAttribute('aria-current'));
                    
                    // Add active state to clicked link
                    this.setAttribute('aria-current', 'page');
                    
                    // Get target section
                    const targetId = this.getAttribute('href');
                    const targetSection = document.querySelector(targetId);
                    
                    if (targetSection) {
                        // Smooth scroll to section
                        targetSection.scrollIntoView({ 
                            behavior: 'smooth', 
                            block: 'start' 
                        });
                        
                        // Close mobile menu if open
                        const mainNav = document.querySelector('.main-nav');
                        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
                        if (mainNav && mainNav.classList.contains('show')) {
                            mainNav.classList.remove('show');
                            if (mobileMenuBtn) {
                                mobileMenuBtn.setAttribute('aria-expanded', 'false');
                                mobileMenuBtn.setAttribute('aria-label', 'Abrir menu de navegação');
                            }
                        }
                    }
                });
            });
        }

        // Mobile menu functionality
        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
        const mainNav = document.querySelector('.main-nav');
        
        if (mobileMenuBtn && mainNav) {
            mobileMenuBtn.addEventListener('click', function() {
                const isExpanded = this.getAttribute('aria-expanded') === 'true';
                this.setAttribute('aria-expanded', !isExpanded);
                mainNav.classList.toggle('show');
                
                // Update button text for screen readers
                this.setAttribute('aria-label', isExpanded ? 'Abrir menu de navegação' : 'Fechar menu de navegação');
            });
        }

        // Close mobile menu with Escape key
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape' && mainNav && mainNav.classList.contains('show')) {
                mainNav.classList.remove('show');
                if (mobileMenuBtn) {
                    mobileMenuBtn.setAttribute('aria-expanded', 'false');
                    mobileMenuBtn.setAttribute('aria-label', 'Abrir menu de navegação');
                    mobileMenuBtn.focus();
                }
            }
        });

        // Search functionality
        const searchBtn = document.querySelector('.search-btn');
        const searchSection = document.querySelector('.search-section');
        const searchInput = document.querySelector('#symptom-input');
        const searchForm = document.querySelector('.search-form');
        const analyzeBtn = document.querySelector('.search-submit');

        if (searchBtn && searchSection && searchInput) {
            searchBtn.addEventListener('click', function() {
                const isExpanded = this.getAttribute('aria-expanded') === 'true';
                this.setAttribute('aria-expanded', !isExpanded);
                
                if (!isExpanded) {
                    searchSection.hidden = false;
                    searchInput.focus();
                } else {
                    searchSection.hidden = true;
                }
            });
        }

        // Symptom analysis - Form submission
        if (searchForm) {
            searchForm.addEventListener('submit', function(e) {
                e.preventDefault();
                analyzeSymptoms();
            });
        }

        // Symptom analysis - Button click
        if (analyzeBtn) {
            analyzeBtn.addEventListener('click', function(e) {
                e.preventDefault();
                analyzeSymptoms();
            });
        }

        function analyzeSymptoms() {
            console.log('analyzeSymptoms called');
            
            if (!searchInput) {
                console.error('Search input not found');
                return;
            }
            
            const symptoms = searchInput.value.trim().toLowerCase();
            console.log('Symptoms input:', symptoms);
            
            if (!symptoms) {
                showError('Por favor, descreva seus sintomas para análise.');
                searchInput.focus();
                return;
            }
            
            // Show loading state
            let originalButtonContent = '';
            if (analyzeBtn) {
                originalButtonContent = analyzeBtn.innerHTML;
                analyzeBtn.innerHTML = '<i class="fas fa-spinner fa-spin" aria-hidden="true"></i> Analisando...';
                analyzeBtn.disabled = true;
            }
            
            // Hide any previous results
            hideResultPanel();
            
            // Simulate AI processing time
            setTimeout(() => {
                try {
                    console.log('Starting analysis...');
                    const analysis = performAIAnalysis(symptoms);
                    console.log('Analysis completed:', analysis);
                    showAnalysisResult(analysis);
                } catch (error) {
                    console.error('Error in analysis:', error);
                    showError('❌ Erro durante a análise: ' + error.message);
                } finally {
                    // Reset button in finally block to ensure it always happens
                    if (analyzeBtn) {
                        analyzeBtn.innerHTML = originalButtonContent || '<i class="fas fa-stethoscope" aria-hidden="true"></i> Analisar';
                        analyzeBtn.disabled = false;
                    }
                }
            }, 1500);
        }

        function performAIAnalysis(symptoms) {
            console.log('Analyzing symptoms:', symptoms); // Debug log
            
            // AI-powered symptom analysis based on keywords
            const symptomPatterns = {
                fever: ['febre', 'temperatura', 'calor', 'quente'],
                headache: ['dor de cabeça', 'cefaleia', 'enxaqueca', 'cabeça doendo'],
                cough: ['tosse', 'tossindo', 'pigarro'],
                nausea: ['náusea', 'enjoo', 'vômito', 'vomitando'],
                pain: ['dor', 'doendo', 'machucado', 'ferido'],
                breathing: ['falta de ar', 'respiração', 'ofegante', 'sufocando'],
                chest: ['peito', 'tórax', 'coração'],
                stomach: ['barriga', 'estômago', 'abdominal', 'intestino'],
                throat: ['garganta', 'engolir', 'rouquidão'],
                cold: ['resfriado', 'gripe', 'coriza', 'nariz entupido']
            };

            let detectedSymptoms = [];
            let urgencyLevel = 'baixa';
            let recommendations = [];
            let immediateActions = [];

            // Detect symptoms
            for (let [category, keywords] of Object.entries(symptomPatterns)) {
                if (keywords.some(keyword => symptoms.includes(keyword))) {
                    detectedSymptoms.push(category);
                }
            }

            // Determine urgency and recommendations based on detected symptoms
            if (detectedSymptoms.includes('breathing') || detectedSymptoms.includes('chest')) {
                urgencyLevel = 'alta';
                recommendations.push('Procure atendimento médico IMEDIATAMENTE');
                recommendations.push('Dirija-se ao pronto-socorro mais próximo');
                immediateActions.push('Mantenha-se calmo e respire devagar');
                immediateActions.push('Evite esforços físicos');
            } else if (detectedSymptoms.includes('fever') && detectedSymptoms.includes('cough')) {
                urgencyLevel = 'moderada';
                recommendations.push('Consulte um médico em até 24 horas');
                recommendations.push('Procure uma UBS ou clínica');
                immediateActions.push('Mantenha-se hidratado');
                immediateActions.push('Descanse e evite contato próximo com outras pessoas');
                immediateActions.push('Use máscara se precisar sair');
            } else if (detectedSymptoms.includes('headache') && detectedSymptoms.includes('fever')) {
                urgencyLevel = 'moderada';
                recommendations.push('Agende consulta médica em 1-2 dias');
                recommendations.push('Monitore a temperatura corporal');
                immediateActions.push('Tome bastante líquido');
                immediateActions.push('Descanse em ambiente fresco');
                immediateActions.push('Evite automedicação');
            } else if (detectedSymptoms.includes('nausea') || detectedSymptoms.includes('stomach')) {
                urgencyLevel = 'baixa';
                recommendations.push('Consulte um clínico geral nos próximos dias');
                recommendations.push('Observe a evolução dos sintomas');
                immediateActions.push('Mantenha dieta leve (chás, torradas)');
                immediateActions.push('Evite alimentos gordurosos');
                immediateActions.push('Hidrate-se aos poucos');
            } else if (detectedSymptoms.includes('cold') || detectedSymptoms.includes('throat')) {
                urgencyLevel = 'baixa';
                recommendations.push('Cuidados domiciliares podem ser suficientes');
                recommendations.push('Consulte médico se piorar em 3-5 dias');
                immediateActions.push('Faça gargarejos com água morna e sal');
                immediateActions.push('Beba líquidos quentes (chás, sopas)');
                immediateActions.push('Descanse adequadamente');
            } else {
                // Generic response for unrecognized symptoms
                urgencyLevel = 'moderada';
                recommendations.push('Consulte um profissional de saúde');
                recommendations.push('Descreva detalhadamente seus sintomas ao médico');
                immediateActions.push('Monitore a evolução dos sintomas');
                immediateActions.push('Mantenha-se hidratado');
            }

            const result = {
                symptoms: detectedSymptoms,
                urgency: urgencyLevel,
                recommendations: recommendations,
                immediateActions: immediateActions,
                originalText: symptoms
            };
            
            console.log('Analysis result:', result); // Debug log
            return result;
        }

        function showAnalysisResult(analysis) {
            console.log('Showing analysis result:', analysis);
            
            if (!analysis) {
                showError('❌ Erro na análise. Tente novamente.');
                return;
            }
            
            const urgencyColors = {
                'baixa': { emoji: '🟢', color: '#22c55e', bg: '#dcfce7' },
                'moderada': { emoji: '🟡', color: '#f59e0b', bg: '#fef3c7' },
                'alta': { emoji: '🔴', color: '#ef4444', bg: '#fee2e2' }
            };

            const urgencyInfo = urgencyColors[analysis.urgency] || urgencyColors['moderada'];
            
            // Create result panel
            const resultPanel = createResultPanel();
            
            let resultHTML = `
                <div class="analysis-header" style="background: ${urgencyInfo.bg}; color: ${urgencyInfo.color}; padding: 1.5rem; border-radius: 0.75rem; margin-bottom: 1.5rem; border: 2px solid ${urgencyInfo.color};">
                    <h3 style="margin: 0; font-size: 1.5rem; display: flex; align-items: center; gap: 0.75rem;">
                        ${urgencyInfo.emoji} ANÁLISE INTELIGENTE MedSUS
                    </h3>
                    <p style="margin: 0.5rem 0 0 0; font-size: 1.125rem; font-weight: 600;">
                        Nível de Urgência: ${(analysis.urgency || 'moderada').toUpperCase()}
                    </p>
                </div>
                
                <div class="analysis-content" style="display: grid; gap: 1.5rem;">
            `;
            
            // Symptoms section
            resultHTML += `
                <div class="analysis-section">
                    <h4 style="color: #374151; margin: 0 0 0.75rem 0; font-size: 1.125rem; display: flex; align-items: center; gap: 0.5rem;">
                        📋 Sintomas Identificados
                    </h4>
                    <ul style="margin: 0; padding-left: 1.25rem; color: #6b7280;">
            `;
            
            if (analysis.symptoms && analysis.symptoms.length > 0) {
                const symptomNames = {
                    fever: 'Febre',
                    headache: 'Dor de cabeça',
                    cough: 'Tosse',
                    nausea: 'Náusea/Enjoo',
                    pain: 'Dor',
                    breathing: 'Dificuldade respiratória',
                    chest: 'Dor no peito',
                    stomach: 'Problemas estomacais',
                    throat: 'Dor de garganta',
                    cold: 'Sintomas de resfriado'
                };
                analysis.symptoms.forEach(symptom => {
                    resultHTML += `<li style="margin-bottom: 0.25rem;">${symptomNames[symptom] || symptom}</li>`;
                });
            } else {
                resultHTML += `<li>Sintomas gerais detectados</li>`;
            }
            
            resultHTML += `</ul></div>`;
            
            // Recommendations section
            resultHTML += `
                <div class="analysis-section">
                    <h4 style="color: #374151; margin: 0 0 0.75rem 0; font-size: 1.125rem; display: flex; align-items: center; gap: 0.5rem;">
                        💡 Recomendações Médicas
                    </h4>
                    <ul style="margin: 0; padding-left: 1.25rem; color: #6b7280;">
            `;
            
            if (analysis.recommendations && analysis.recommendations.length > 0) {
                analysis.recommendations.forEach(rec => {
                    resultHTML += `<li style="margin-bottom: 0.5rem; font-weight: 500;">${rec}</li>`;
                });
            } else {
                resultHTML += `<li>Consulte um profissional de saúde</li>`;
            }
            
            resultHTML += `</ul></div>`;
            
            // Immediate actions section
            resultHTML += `
                <div class="analysis-section">
                    <h4 style="color: #374151; margin: 0 0 0.75rem 0; font-size: 1.125rem; display: flex; align-items: center; gap: 0.5rem;">
                        🏠 Cuidados Imediatos
                    </h4>
                    <ul style="margin: 0; padding-left: 1.25rem; color: #6b7280;">
            `;
            
            if (analysis.immediateActions && analysis.immediateActions.length > 0) {
                analysis.immediateActions.forEach(action => {
                    resultHTML += `<li style="margin-bottom: 0.25rem;">${action}</li>`;
                });
            } else {
                resultHTML += `<li>Mantenha-se hidratado</li><li>Descanse adequadamente</li>`;
            }
            
            resultHTML += `</ul></div>`;
            
            // Emergency contacts
            resultHTML += `
                <div class="analysis-section" style="background: #f3f4f6; padding: 1rem; border-radius: 0.5rem;">
                    <h4 style="color: #374151; margin: 0 0 0.75rem 0; font-size: 1.125rem; display: flex; align-items: center; gap: 0.5rem;">
                        📞 Contatos de Emergência
                    </h4>
                    <div style="display: grid; gap: 0.5rem; color: #6b7280;">
                        <div><strong>SAMU:</strong> <a href="tel:192" style="color: #dc2626;">192</a> (emergências)</div>
                        <div><strong>Central SUS:</strong> <a href="tel:136" style="color: #0ea5e9;">136</a> (orientações)</div>
                        <div><strong>Bombeiros:</strong> <a href="tel:193" style="color: #dc2626;">193</a> (emergências graves)</div>
                    </div>
                </div>
            `;
            
            // Important disclaimer
            resultHTML += `
                <div class="analysis-section" style="background: #fef3c7; padding: 1rem; border-radius: 0.5rem; border-left: 4px solid #f59e0b;">
                    <h4 style="color: #92400e; margin: 0 0 0.5rem 0; font-size: 1rem; display: flex; align-items: center; gap: 0.5rem;">
                        ⚠️ Importante
                    </h4>
                    <p style="margin: 0; color: #92400e; font-size: 0.875rem; line-height: 1.5;">
                        Esta é uma análise preliminar baseada em IA. <strong>SEMPRE consulte um profissional de saúde</strong> para diagnóstico e tratamento adequados.
                    </p>
            `;
            
            if (analysis.urgency === 'alta') {
                resultHTML += `
                    <p style="margin: 0.75rem 0 0 0; color: #dc2626; font-weight: 600; font-size: 0.875rem;">
                        🚨 ATENÇÃO: Seus sintomas indicam necessidade de atendimento médico IMEDIATO!
                    </p>
                `;
            }
            
            resultHTML += `</div></div>`;
            
            resultPanel.innerHTML = resultHTML;
            
            // Show the panel
            resultPanel.hidden = false;
            resultPanel.scrollIntoView({ behavior: 'smooth', block: 'start' });
            
            // Clear the input after analysis
            if (searchInput) searchInput.value = '';
            
            // Announce result to screen readers
            announceToScreenReader(`Análise concluída. Nível de urgência: ${analysis.urgency || 'moderada'}. Verifique as recomendações.`);
        }

        function createResultPanel() {
            let resultPanel = document.getElementById('analysis-result-panel');
            
            if (!resultPanel) {
                resultPanel = document.createElement('div');
                resultPanel.id = 'analysis-result-panel';
                resultPanel.style.cssText = `
                    background: white;
                    border-radius: 1rem;
                    padding: 2rem;
                    margin: 2rem auto;
                    max-width: 50rem;
                    box-shadow: 0 1rem 3rem rgba(0, 0, 0, 0.175);
                    border: 1px solid #e5e7eb;
                    position: relative;
                `;
                resultPanel.hidden = true;
                
                // Add close button
                const closeBtn = document.createElement('button');
                closeBtn.innerHTML = '✕';
                closeBtn.style.cssText = `
                    position: absolute;
                    top: 1rem;
                    right: 1rem;
                    background: #f3f4f6;
                    border: none;
                    border-radius: 50%;
                    width: 2rem;
                    height: 2rem;
                    cursor: pointer;
                    font-size: 1rem;
                    color: #6b7280;
                    display: flex;
                    align-items: center;
                    justify-content: center;
                `;
                closeBtn.onclick = () => hideResultPanel();
                closeBtn.setAttribute('aria-label', 'Fechar resultado da análise');
                
                resultPanel.appendChild(closeBtn);
                
                // Insert after search section
                const searchSection = document.querySelector('.search-section');
                if (searchSection && searchSection.parentNode) {
                    searchSection.parentNode.insertBefore(resultPanel, searchSection.nextSibling);
                }
            }
            
            return resultPanel;
        }

        function hideResultPanel() {
            const resultPanel = document.getElementById('analysis-result-panel');
            if (resultPanel) {
                resultPanel.hidden = true;
            }
        }

        function showError(message) {
            const resultPanel = createResultPanel();
            resultPanel.innerHTML = `
                <div style="background: #fee2e2; color: #dc2626; padding: 1.5rem; border-radius: 0.75rem; text-align: center; border: 2px solid #dc2626;">
                    <h3 style="margin: 0 0 0.5rem 0; font-size: 1.25rem;">❌ Erro</h3>
                    <p style="margin: 0;">${message}</p>
                </div>
            `;
            resultPanel.hidden = false;
            resultPanel.scrollIntoView({ behavior: 'smooth', block: 'start' });
        }

        // LGPD Cookie Banner
        const cookieBanner = document.querySelector('#cookie-banner');
        
        // Show banner if no consent given
        if (!localStorage.getItem('cookieConsent')) {
            setTimeout(() => {
                cookieBanner.classList.add('show');
            }, 2000);
        }

        function acceptEssentialCookies() {
            localStorage.setItem('cookieConsent', 'essential');
            localStorage.setItem('analyticsConsent', 'false');
            cookieBanner.classList.remove('show');
            
            // Only load essential cookies
            console.log('Essential cookies accepted');
        }

        function acceptAllCookies() {
            localStorage.setItem('cookieConsent', 'all');
            localStorage.setItem('analyticsConsent', 'true');
            cookieBanner.classList.remove('show');
            
            // Load all cookies including analytics
            console.log('All cookies accepted');
            
            // Here you would initialize analytics services
            // Example: gtag('config', 'GA_MEASUREMENT_ID');
        }

        // Close mobile menu when clicking outside
        document.addEventListener('click', function(e) {
            if (mainNav && mobileMenuBtn && !mainNav.contains(e.target) && !mobileMenuBtn.contains(e.target)) {
                if (mainNav.classList.contains('show')) {
                    mainNav.classList.remove('show');
                    mobileMenuBtn.setAttribute('aria-expanded', 'false');
                    mobileMenuBtn.setAttribute('aria-label', 'Abrir menu de navegação');
                }
            }
        });

        // Handle responsive navigation on resize
        window.addEventListener('resize', function() {
            if (window.innerWidth > 768 && mainNav && mobileMenuBtn) {
                mainNav.classList.remove('show');
                mobileMenuBtn.setAttribute('aria-expanded', 'false');
                mobileMenuBtn.setAttribute('aria-label', 'Abrir menu de navegação');
            }
        });

        // Form validation
        function validateForm(form) {
            const inputs = form.querySelectorAll('input[required]');
            let isValid = true;
            
            inputs.forEach(input => {
                if (!input.value.trim()) {
                    input.setAttribute('aria-invalid', 'true');
                    isValid = false;
                } else {
                    input.setAttribute('aria-invalid', 'false');
                }
            });
            
            return isValid;
        }

        // Announce page changes for screen readers
        function announceToScreenReader(message) {
            const announcement = document.createElement('div');
            announcement.setAttribute('aria-live', 'polite');
            announcement.setAttribute('aria-atomic', 'true');
            announcement.className = 'sr-only';
            announcement.textContent = message;
            
            document.body.appendChild(announcement);
            
            setTimeout(() => {
                document.body.removeChild(announcement);
            }, 1000);
        }

        // Initialize page
        document.addEventListener('DOMContentLoaded', function() {
            // Set focus management
            const skipLink = document.querySelector('.skip-link');
            if (skipLink) {
                skipLink.addEventListener('click', function(e) {
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        target.focus();
                        target.scrollIntoView();
                    }
                });
            }
            
            // Announce page load for screen readers
            announceToScreenReader('Página MedSUS carregada. Use Tab para navegar pelos elementos.');
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'975d2a7136ba8cdf',t:'MTc1NjMxNDQ1Mi4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
