<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta
        name="description"
        content="Muhammad Fathi Duraini — International Relations academic portfolio covering research, human rights, international law, policy analysis and humanitarian affairs."
    >

    <meta name="author" content="Muhammad Fathi Duraini">

    <title>Muhammad Fathi Duraini | Academic Portfolio</title>

    <style>

        :root {
            --navy: #0c1524;
            --navy-2: #121f33;
            --gold: #b99a5b;
            --cream: #f5f2ea;
            --paper: #fffdf8;
            --white: #ffffff;
            --text: #172131;
            --muted: #697386;
            --line: #ddd9cf;
            --soft: #ece9e1;
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
            font-family: Arial, Helvetica, sans-serif;
            background: var(--cream);
            color: var(--text);
            line-height: 1.6;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        .container {
            width: min(1180px, 90%);
            margin: auto;
        }


        /* =========================
           NAVIGATION
        ========================= */

        nav {
            position: sticky;
            top: 0;
            z-index: 999;

            background: rgba(245,242,234,.94);
            backdrop-filter: blur(14px);

            border-bottom: 1px solid var(--line);
        }

        .nav-inner {
            min-height: 72px;

            display: flex;
            align-items: center;
            justify-content: space-between;

            gap: 30px;
        }

        .brand {
            font-family: Georgia, "Times New Roman", serif;
            font-size: 19px;
        }

        .nav-links {
            display: flex;
            gap: 25px;

            font-size: 10px;
            text-transform: uppercase;
            letter-spacing: .13em;

            color: var(--muted);
        }

        .nav-links a:hover {
            color: var(--text);
        }


        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 88vh;

            display: grid;
            grid-template-columns: 1.15fr .85fr;

            align-items: center;

            gap: 80px;

            padding: 90px 0;
        }

        .eyebrow {
            margin-bottom: 25px;

            font-size: 10px;
            font-weight: bold;

            text-transform: uppercase;
            letter-spacing: .2em;

            color: var(--gold);
        }

        .hero h1 {
            font-family: Georgia, "Times New Roman", serif;

            font-size: clamp(60px, 8vw, 105px);

            font-weight: 400;

            line-height: .88;

            letter-spacing: -.055em;

            margin-bottom: 35px;
        }

        .hero-description {
            max-width: 650px;

            font-size: 18px;

            color: var(--muted);

            margin-bottom: 35px;
        }

        .hero-actions {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .button {
            display: inline-block;

            padding: 13px 19px;

            border: 1px solid var(--text);

            font-size: 10px;

            text-transform: uppercase;
            letter-spacing: .12em;

            transition: .25s ease;
        }

        .button:hover {
            background: var(--navy);
            color: white;
        }

        .button.secondary {
            border-color: var(--line);
            color: var(--muted);
        }


        /* =========================
           HERO VISUAL
        ========================= */

        .hero-visual {
            position: relative;

            height: 470px;

            border: 1px solid var(--line);

            background:
                linear-gradient(var(--line) 1px, transparent 1px),
                linear-gradient(90deg, var(--line) 1px, transparent 1px);

            background-size: 55px 55px;

            overflow: hidden;
        }

        .orbit {
            position: absolute;

            width: 310px;
            height: 310px;

            border: 1px solid var(--gold);

            border-radius: 50%;

            top: 50%;
            left: 50%;

            transform: translate(-50%, -50%);
        }

        .orbit::before {
            content: "";

            position: absolute;

            width: 210px;
            height: 210px;

            border: 1px solid rgba(185,154,91,.55);

            border-radius: 50%;

            top: 49px;
            left: 49px;
        }

        .orbit::after {
            content: "";

            position: absolute;

            width: 95px;
            height: 95px;

            background: var(--navy);

            border-radius: 50%;

            top: 106px;
            left: 106px;
        }

        .visual-label {
            position: absolute;

            font-size: 9px;

            text-transform: uppercase;
            letter-spacing: .16em;

            color: var(--muted);
        }

        .visual-top {
            top: 22px;
            left: 22px;
        }

        .visual-bottom {
            bottom: 22px;
            right: 22px;
        }


        /* =========================
           GENERAL SECTIONS
        ========================= */

        section {
            padding: 110px 0;
        }

        .section-label {
            margin-bottom: 15px;

            font-size: 10px;
            font-weight: bold;

            text-transform: uppercase;
            letter-spacing: .2em;

            color: var(--gold);
        }

        .section-title {
            font-family: Georgia, "Times New Roman", serif;

            font-size: clamp(40px, 5vw, 65px);

            font-weight: 400;

            line-height: 1;

            margin-bottom: 45px;
        }


        /* =========================
           INTELLECTUAL FOCUS
        ========================= */

        .focus {
            background: var(--navy);
            color: white;
        }

        .focus-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);

            border-top: 1px solid rgba(255,255,255,.2);
        }

        .focus-card {
            padding: 35px 25px 35px 0;

            border-right: 1px solid rgba(255,255,255,.2);
        }

        .focus-card:not(:first-child) {
            padding-left: 25px;
        }

        .focus-card:last-child {
            border-right: none;
        }

        .focus-number {
            font-family: Georgia, serif;

            font-size: 40px;

            color: var(--gold);

            margin-bottom: 12px;
        }

        .focus-card h3 {
            font-family: Georgia, serif;

            font-size: 25px;

            font-weight: 400;

            margin-bottom: 10px;
        }

        .focus-card p {
            font-size: 13px;

            color: #bbc2cc;
        }


        /* =========================
           PORTFOLIO DIRECTORY
        ========================= */

        .directory-header {
            display: flex;
            justify-content: space-between;
            align-items: end;

            gap: 40px;

            margin-bottom: 45px;
        }

        .directory-header p {
            max-width: 450px;

            color: var(--muted);

            font-size: 13px;
        }

        .directory {
            border-top: 1px solid var(--line);
        }

        .directory-item {
            display: grid;

            grid-template-columns: 100px 1fr 170px;

            gap: 30px;

            align-items: center;

            padding: 30px 0;

            border-bottom: 1px solid var(--line);

            transition: .25s ease;
        }

        .directory-item:hover {
            padding-left: 12px;

            background: rgba(255,255,255,.25);
        }

        .directory-code {
            font-family: Georgia, serif;

            font-size: 22px;

            color: var(--gold);
        }

        .directory-item h3 {
            font-family: Georgia, serif;

            font-size: 27px;

            font-weight: 400;

            margin-bottom: 5px;
        }

        .directory-item p {
            font-size: 13px;

            color: var(--muted);
        }

        .directory-status {
            text-align: right;

            font-size: 9px;

            text-transform: uppercase;

            letter-spacing: .12em;

            color: var(--muted);
        }


        /* =========================
           FEATURED RESEARCH
        ========================= */

        .featured {
            background: var(--paper);
        }

        .featured-box {
            display: grid;

            grid-template-columns: .7fr 1.3fr;

            min-height: 430px;
        }

        .featured-number {
            background: var(--navy);

            color: white;

            padding: 45px;

            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .featured-number span {
            font-size: 9px;

            text-transform: uppercase;

            letter-spacing: .15em;

            color: var(--gold);
        }

        .featured-number strong {
            font-family: Georgia, serif;

            font-size: 105px;

            font-weight: 400;
        }

        .featured-content {
            background: white;

            padding: 55px;
        }

        .featured-content h2 {
            font-family: Georgia, serif;

            font-size: 45px;

            font-weight: 400;

            line-height: 1.05;

            margin-bottom: 22px;
        }

        .featured-content p {
            max-width: 650px;

            color: var(--muted);

            font-size: 14px;

            margin-bottom: 30px;
        }

        .tags {
            display: flex;
            flex-wrap: wrap;

            gap: 8px;

            margin-bottom: 30px;
        }

        .tag {
            padding: 7px 10px;

            border: 1px solid var(--line);

            font-size: 9px;

            text-transform: uppercase;

            letter-spacing: .08em;
        }


        /* =========================
           RESEARCH METHOD
        ========================= */

        .method-grid {
            display: grid;

            grid-template-columns: repeat(4, 1fr);

            gap: 25px;
        }

        .method {
            border-top: 2px solid var(--text);

            padding-top: 20px;
        }

        .method-number {
            font-family: Georgia, serif;

            font-size: 28px;

            color: var(--gold);
        }

        .method h3 {
            font-family: Georgia, serif;

            font-size: 23px;

            font-weight: 400;

            margin: 10px 0;
        }

        .method p {
            font-size: 13px;

            color: var(--muted);
        }


        /* =========================
           INTELLECTUAL MAP
        ========================= */

        .map-section {
            background: var(--navy-2);

            color: white;
        }

        .map {
            position: relative;

            height: 470px;

            border: 1px solid rgba(255,255,255,.13);

            background:
                linear-gradient(rgba(255,255,255,.05) 1px, transparent 1px),
                linear-gradient(90deg, rgba(255,255,255,.05) 1px, transparent 1px);

            background-size: 60px 60px;
        }

        .map-center {
            position: absolute;

            width: 150px;
            height: 150px;

            top: 50%;
            left: 50%;

            transform: translate(-50%, -50%);

            border: 1px solid var(--gold);

            border-radius: 50%;

            display: flex;
            align-items: center;
            justify-content: center;

            text-align: center;

            font-family: Georgia, serif;

            font-size: 19px;
        }

        .map-node {
            position: absolute;

            padding: 12px 16px;

            border: 1px solid rgba(255,255,255,.2);

            font-size: 9px;

            text-transform: uppercase;

            letter-spacing: .1em;
        }

        .node-1 {
            top: 15%;
            left: 13%;
        }

        .node-2 {
            top: 17%;
            right: 12%;
        }

        .node-3 {
            bottom: 17%;
            left: 10%;
        }

        .node-4 {
            bottom: 14%;
            right: 13%;
        }


        /* =========================
           PROFILE
        ========================= */

        .profile-grid {
            display: grid;

            grid-template-columns: .8fr 1.2fr;

            gap: 80px;
        }

        .profile-name {
            font-family: Georgia, serif;

            font-size: 48px;

            line-height: 1;
        }

        .profile-content p {
            color: var(--muted);

            font-size: 14px;

            margin-bottom: 22px;
        }

        .profile-details {
            display: grid;

            grid-template-columns: 1fr 1fr;

            border-top: 1px solid var(--line);

            margin-top: 35px;
        }

        .detail {
            padding: 18px 0;

            border-bottom: 1px solid var(--line);
        }

        .detail:nth-child(odd) {
            margin-right: 25px;
        }

        .detail-label {
            display: block;

            margin-bottom: 5px;

            font-size: 9px;

            text-transform: uppercase;

            letter-spacing: .13em;

            color: var(--gold);
        }

        .detail-value {
            font-size: 12px;
        }


        /* =========================
           FOOTER
        ========================= */

        footer {
            background: #080e17;

            color: white;

            padding: 65px 0;
        }

        .footer-inner {
            display: flex;

            justify-content: space-between;

            align-items: end;

            gap: 30px;
        }

        .footer-name {
            font-family: Georgia, serif;

            font-size: 30px;

            margin-bottom: 7px;
        }

        .footer-note {
            color: #929aa8;

            font-size: 11px;
        }

        .footer-links {
            display: flex;

            gap: 20px;

            font-size: 9px;

            text-transform: uppercase;

            letter-spacing: .1em;
        }

        .footer-links a:hover {
            color: var(--gold);
        }


        /* =========================
           MOBILE
        ========================= */

        @media (max-width: 850px) {

            .nav-inner {
                flex-direction: column;

                align-items: flex-start;

                padding: 18px 0;

                gap: 15px;
            }

            .nav-links {
                flex-wrap: wrap;

                gap: 15px;
            }

            .hero {
                grid-template-columns: 1fr;

                gap: 50px;

                padding: 70px 0;
            }

            .hero-visual {
                height: 350px;
            }

            .focus-grid {
                grid-template-columns: 1fr;
            }

            .focus-card,
            .focus-card:not(:first-child) {
                padding: 30px 0;

                border-right: none;

                border-bottom: 1px solid rgba(255,255,255,.2);
            }

            .directory-item {
                grid-template-columns: 60px 1fr;
            }

            .directory-status {
                display: none;
            }

            .featured-box {
                grid-template-columns: 1fr;
            }

            .method-grid {
                grid-template-columns: 1fr 1fr;
            }

            .profile-grid {
                grid-template-columns: 1fr;

                gap: 40px;
            }

            .footer-inner {
                flex-direction: column;

                align-items: flex-start;
            }
        }

        @media (max-width: 550px) {

            .hero h1 {
                font-size: 55px;
            }

            .method-grid {
                grid-template-columns: 1fr;
            }

            .featured-content {
                padding: 35px;
            }

            .featured-content h2 {
                font-size: 35px;
            }

            .profile-details {
                grid-template-columns: 1fr;
            }

            .detail:nth-child(odd) {
                margin-right: 0;
            }

            .map {
                height: 390px;
            }

            .map-center {
                width: 115px;
                height: 115px;

                font-size: 16px;
            }
        }

    </style>
</head>


<body>


<!-- =====================================
     NAVIGATION
===================================== -->

<nav>

    <div class="container nav-inner">

        <a href="#" class="brand">
            Muhammad Fathi Duraini
        </a>

        <div class="nav-links">

            <a href="#portfolio">
                Portfolio
            </a>

            <a href="#research">
                Research
            </a>

            <a href="#method">
                Method
            </a>

            <a href="#profile">
                Profile
            </a>

        </div>

    </div>

</nav>


<!-- =====================================
     HERO
===================================== -->

<section class="container hero">

    <div>

        <div class="eyebrow">
            International Relations · Academic Research
        </div>

        <h1>
            Ideas<br>
            into<br>
            research.
        </h1>

        <p class="hero-description">
            An academic portfolio and knowledge environment
            focused on international relations, international law,
            human rights, humanitarian affairs, policy and global security.
        </p>

        <div class="hero-actions">

            <a href="#portfolio" class="button">
                Explore Portfolio
            </a>

            <a href="#research" class="button secondary">
                Research Archive
            </a>

        </div>

    </div>


    <div class="hero-visual">

        <div class="visual-label visual-top">
            Academic Knowledge Archive
        </div>

        <div class="orbit"></div>

        <div class="visual-label visual-bottom">
            IR · LAW · RIGHTS · POLICY
        </div>

    </div>

</section>


<!-- =====================================
     INTELLECTUAL FOCUS
===================================== -->

<section class="focus">

    <div class="container">

        <div class="section-label">
            Intellectual Focus
        </div>

        <div class="section-title">
            Areas of inquiry
        </div>


        <div class="focus-grid">


            <div class="focus-card">

                <div class="focus-number">
                    01
                </div>

                <h3>
                    International Law
                </h3>

                <p>
                    International legal principles, treaties,
                    state responsibility and the relationship
                    between international and domestic law.
                </p>

            </div>


            <div class="focus-card">

                <div class="focus-number">
                    02
                </div>

                <h3>
                    Human Rights
                </h3>

                <p>
                    Human rights standards, constitutional
                    protections, institutional mechanisms
                    and rights-based approaches.
                </p>

            </div>


            <div class="focus-card">

                <div class="focus-number">
                    03
                </div>

                <h3>
                    Global Affairs
                </h3>

                <p>
                    International security, humanitarian affairs,
                    development, policy and the institutions
                    shaping global order.
                </p>

            </div>


        </div>

    </div>

</section>


<!-- =====================================
     PORTFOLIO DIRECTORY
===================================== -->

<section id="portfolio">

    <div class="container">


        <div class="directory-header">

            <div>

                <div class="section-label">
                    Portfolio Directory
                </div>

                <div class="section-title">
                    Explore the work.
                </div>

            </div>

            <p>
                A structured academic portfolio connecting
                research projects, policy work, human rights
                analysis and practical experiences.
            </p>

        </div>


        <div class="directory">


            <!-- RESEARCH -->

            <a
                href="research/"
                class="directory-item"
            >

                <div class="directory-code">
                    01
                </div>

                <div>

                    <h3>
                        Research
                    </h3>

                    <p>
                        Academic research, legal materials,
                        case law, international instruments,
                        literature and analytical findings.
                    </p>

                </div>

                <div class="directory-status">
                    Research Archive
                </div>

            </a>


            <!-- HUMAN RIGHTS -->

            <a
                href="human-rights-development/"
                class="directory-item"
            >

                <div class="directory-code">
                    02
                </div>

                <div>

                    <h3>
                        Human Rights & Development
                    </h3>

                    <p>
                        Malaysia-focused work examining human rights,
                        development, institutions, policy,
                        vulnerable communities and accountability.
                    </p>

                </div>

                <div class="directory-status">
                    Developing
                </div>

            </a>


            <!-- POLICY -->

            <a
                href="policy-briefs/"
                class="directory-item"
            >

                <div class="directory-code">
                    03
                </div>

                <div>

                    <h3>
                        Policy Briefs
                    </h3>

                    <p>
                        Concise policy analysis connecting
                        research evidence with contemporary
                        public-policy questions.
                    </p>

                </div>

                <div class="directory-status">
                    Policy Work
                </div>

            </a>


            <!-- GROUNDWORK -->

            <a
                href="groundwork-volunteering/"
                class="directory-item"
            >

                <div class="directory-code">
                    04
                </div>

                <div>

                    <h3>
                        Groundwork & Volunteering
                    </h3>

                    <p>
                        Practical experiences, humanitarian
                        engagement, volunteering and activities
                        supporting the development of field awareness.
                    </p>

                </div>

                <div class="directory-status">
                    Experience
                </div>

            </a>


        </div>

    </div>

</section>


<!-- =====================================
     FEATURED RESEARCH
===================================== -->

<section class="featured" id="research">

    <div class="container">

        <div class="section-label">
            Featured Research
        </div>


        <div class="featured-box">


            <div class="featured-number">

                <span>
                    Research Project 01
                </span>

                <strong>
                    R01
                </strong>

                <span>
                    Malaysia · Human Rights · International Law
                </span>

            </div>


            <div class="featured-content">

                <h2>
                    Malaysia & International Human Rights Law
                </h2>

                <p>
                    A structured legal research project examining
                    Malaysia's domestic human rights framework,
                    international human rights instruments,
                    constitutional jurisprudence, treaty implementation,
                    Malaysian case law and the role of SUHAKAM.
                </p>


                <div class="tags">

                    <span class="tag">
                        Constitutional Law
                    </span>

                    <span class="tag">
                        Human Rights
                    </span>

                    <span class="tag">
                        International Law
                    </span>

                    <span class="tag">
                        Treaty Law
                    </span>

                    <span class="tag">
                        Malaysia
                    </span>

                </div>


                <a
                    href="research/r01/"
                    class="button"
                >
                    Open R01 Dossier
                </a>

            </div>

        </div>

    </div>

</section>


<!-- =====================================
     RESEARCH METHOD
===================================== -->

<section id="method">

    <div class="container">


        <div class="section-label">
            Research Method
        </div>

        <div class="section-title">
            From source<br>
            to analysis.
        </div>


        <div class="method-grid">


            <div class="method">

                <div class="method-number">
                    01
                </div>

                <h3>
                    Source
                </h3>

                <p>
                    Primary legal sources, official institutional
                    documents, judicial decisions and academic
                    scholarship.
                </p>

            </div>


            <div class="method">

                <div class="method-number">
                    02
                </div>

                <h3>
                    Context
                </h3>

                <p>
                    Establishing the legal, political and
                    institutional context surrounding an issue.
                </p>

            </div>


            <div class="method">

                <div class="method-number">
                    03
                </div>

                <h3>
                    Analysis
                </h3>

                <p>
                    Distinguishing legal rules, institutional
                    positions, academic interpretations and
                    independent analysis.
                </p>

            </div>


            <div class="method">

                <div class="method-number">
                    04
                </div>

                <h3>
                    Questions
                </h3>

                <p>
                    Identifying unresolved issues and directions
                    for further research rather than forcing
                    predetermined conclusions.
                </p>

            </div>


        </div>

    </div>

</section>


<!-- =====================================
     INTELLECTUAL MAP
===================================== -->

<section class="map-section">

    <div class="container">

        <div class="section-label">
            Intellectual Map
        </div>

        <div class="section-title">
            A connected field<br>
            of inquiry
        </div>


        <div class="map">


            <div class="map-center">
                GLOBAL<br>
                AFFAIRS
            </div>


            <div class="map-node node-1">
                International Law
            </div>


            <div class="map-node node-2">
                Human Rights
            </div>


            <div class="map-node node-3">
                Humanitarian Affairs
            </div>


            <div class="map-node node-4">
                International Security
            </div>


        </div>

    </div>

</section>


<!-- =====================================
     PROFILE
===================================== -->

<section id="profile">

    <div class="container">


        <div class="profile-grid">


            <div>

                <div class="section-label">
                    Academic Profile
                </div>

                <div class="profile-name">
                    Muhammad<br>
                    Fathi Duraini
                </div>

            </div>


            <div class="profile-content">

                <p>
                    I am a Bachelor of International Relations
                    (Hons.) student at Universiti Sultan Zainal
                    Abidin (UniSZA), currently developing an academic
                    foundation in international relations,
                    international law and human rights.
                </p>


                <p>
                    This website serves as a personal academic
                    knowledge archive where research, legal materials,
                    policy work and practical experiences are organised
                    into a continuously developing portfolio.
                </p>


                <div class="profile-details">


                    <div class="detail">

                        <span class="detail-label">
                            Programme
                        </span>

                        <span class="detail-value">
                            Bachelor of International Relations (Hons.)
                        </span>

                    </div>


                    <div class="detail">

                        <span class="detail-label">
                            Institution
                        </span>

                        <span class="detail-value">
                            Universiti Sultan Zainal Abidin
                        </span>

                    </div>


                    <div class="detail">

                        <span class="detail-label">
                            Current Stage
                        </span>

                        <span class="detail-value">
                            Year 2 · Semester 3
                        </span>

                    </div>


                    <div class="detail">

                        <span class="detail-label">
                            Research Interests
                        </span>

                        <span class="detail-value">
                            International Law · Human Rights ·
                            Humanitarian Affairs · Global Security
                        </span>

                    </div>


                </div>

            </div>

        </div>

    </div>

</section>


<!-- =====================================
     FOOTER
===================================== -->

<footer>

    <div class="container footer-inner">


        <div>

            <div class="footer-name">
                Muhammad Fathi Duraini
            </div>

            <div class="footer-note">
                International Relations · Academic Research · Human Rights
            </div>

        </div>


        <div class="footer-links">

            <a href="#portfolio">
                Portfolio
            </a>

            <a href="#research">
                Research
            </a>

            <a href="#method">
                Method
            </a>

            <a href="#profile">
                Profile
            </a>

        </div>


    </div>

</footer>


</body>
</html>
