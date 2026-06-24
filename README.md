# sobirjonerkabaev.github.io
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Sobirjon Erkabaev - Shaxsiy sahifa">
    <title>Sobirjon Erkabaev</title>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
            transition: all 0.4s ease;
        }
        .container {
            max-width: 1000px;
            margin: 40px auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.25);
            overflow: hidden;
        }
        .header {
            background: linear-gradient(135deg, #0077cc, #00aaff);
            color: white;
            padding: 90px 40px 70px;
            text-align: center;
            position: relative;
        }
        .header h1 {
            margin: 0;
            font-size: 3.4rem;
            text-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }
        .header p {
            margin: 15px 0 0;
            font-size: 1.45rem;
            opacity: 0.95;
        }
        .lang-switch {
            position: absolute;
            top: 25px;
            right: 30px;
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            justify-content: flex-end;
            max-width: 280px;
        }
        .lang-btn {
            padding: 8px 16px;
            font-size: 0.95rem;
            border: none;
            background: rgba(255,255,255,0.25);
            color: white;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }
        .lang-btn:hover, .lang-btn.active {
            background: white;
            color: #0077cc;
            transform: translateY(-2px);
        }
        .content {
            padding: 60px 50px;
        }
        .card {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 18px;
            margin: 25px 0;
            box-shadow: 0 8px 20px rgba(0,0,0,0.08);
            transition: transform 0.3s ease;
        }
        .card:hover {
            transform: translateY(-8px);
        }
        h2 {
            color: #0077cc;
            margin-top: 0;
        }
        .contact a {
            color: #0077cc;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        .contact a:hover {
            color: #0055aa;
            text-decoration: underline;
        }
        footer {
            text-align: center;
            padding: 25px;
            background: #f8f9fa;
            color: #666;
            font-size: 0.95rem;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="lang-switch">
                <button class="lang-btn active" onclick="setLang('uz')">UZ</button>
                <button class="lang-btn" onclick="setLang('en')">EN</button>
                <button class="lang-btn" onclick="setLang('ru')">RU</button>
                <button class="lang-btn" onclick="setLang('de')">DE</button>
                <button class="lang-btn" onclick="setLang('fr')">FR</button>
                <button class="lang-btn" onclick="setLang('es')">ES</button>
                <button class="lang-btn" onclick="setLang('tr')">TR</button>
                <button class="lang-btn" onclick="setLang('ar')">AR</button>
            </div>
            <h1 id="name">Sobirjon Erkabaev</h1>
            <p id="birth">08.07.2008</p>
        </div>
        
        <div class="content">
            <div class="card">
                <h2 id="about-title">Haqimda</h2>
                <p id="about-text">Salom! Men Sobirjon Erkabaevman.</p>
            </div>

            <div class="card">
                <h2 id="edu-title">Ta'lim</h2>
                <p id="edu-text">2024–2026 yillar oralig‘ida Aluwedni bitirdim.</p>
            </div>

            <div class="card contact">
                <h2 id="contact-title">Aloqa</h2>
                <p>
                    <strong>Email:</strong> <a href="mailto:sobirjon08072008@icloud.com">sobirjon08072008@icloud.com</a><br><br>
                    <strong>Instagram:</strong> <a href="https://www.instagram.com/sobirjon_erkabaev" target="_blank" rel="noopener noreferrer">@sobirjon_erkabaev</a>
                </p>
            </div>
        </div>
        
        <footer>
            © Sobirjon Erkabaev
        </footer>
    </div>

    <script>
        const translations = {
            uz: { name: "Sobirjon Erkabaev", birth: "08.07.2008", aboutTitle: "Haqimda", aboutText: "Salom! Men Sobirjon Erkabaevman.", eduTitle: "Ta'lim", eduText: "2024–2026 yillar oralig‘ida Aluwedni bitirdim.", contactTitle: "Aloqa" },
            en: { name: "Sobirjon Erkabaev", birth: "08.07.2008", aboutTitle: "About Me", aboutText: "Hello! I am Sobirjon Erkabaev.", eduTitle: "Education", eduText: "Graduated from Aluwed in 2024–2026.", contactTitle: "Contact" },
            ru: { name: "Собиржон Эркабаев", birth: "08.07.2008", aboutTitle: "Обо мне", aboutText: "Здравствуйте! Я Собиржон Эркабаев.", eduTitle: "Образование", eduText: "Окончил Aluwed в 2024–2026 годах.", contactTitle: "Контакты" },
            de: { name: "Sobirjon Erkabaev", birth: "08.07.2008", aboutTitle: "Über mich", aboutText: "Hallo! Ich bin Sobirjon Erkabaev.", eduTitle: "Bildung", eduText: "Ich habe 2024–2026 Aluwed abgeschlossen.", contactTitle: "Kontakt" },
            fr: { name: "Sobirjon Erkabaev", birth: "08.07.2008", aboutTitle: "À propos de moi", aboutText: "Bonjour! Je suis Sobirjon Erkabaev.", eduTitle: "Éducation", eduText: "J'ai obtenu mon diplôme d'Aluwed en 2024–2026.", contactTitle: "Contact" },
            es: { name: "Sobirjon Erkabaev", birth: "08.07.2008", aboutTitle: "Sobre mí", aboutText: "¡Hola! Soy Sobirjon Erkabaev.", eduTitle: "Educación", eduText: "Me gradué de Aluwed en 2024–2026.", contactTitle: "Contacto" },
            tr: { name: "Sobirjon Erkabaev", birth: "08.07.2008", aboutTitle: "Hakkımda", aboutText: "Merhaba! Ben Sobirjon Erkabaev.", eduTitle: "Eğitim", eduText: "2024–2026 yıllarında Aluwed'i bitirdim.", contactTitle: "İletişim" },
            ar: { name: "سوبيرجون إركاباييف", birth: "08.07.2008", aboutTitle: "عني", aboutText: "مرحبا! أنا سوبيرجون إركاباييف.", eduTitle: "التعليم", eduText: "تخرجت من ألويد في 2024-2026.", contactTitle: "اتصل" }
        };

        function setLang(lang) {
            document.getElementById('name').textContent = translations[lang].name;
            document.getElementById('birth').textContent = translations[lang].birth;
            document.getElementById('about-title').textContent = translations[lang].aboutTitle;
            document.getElementById('about-text').textContent = translations[lang].aboutText;
            document.getElementById('edu-title').textContent = translations[lang].eduTitle;
            document.getElementById('edu-text').textContent = translations[lang].eduText;
            document.getElementById('contact-title').textContent = translations[lang].contactTitle;

            document.querySelectorAll('.lang-btn').forEach(btn => {
                btn.classList.toggle('active', btn.textContent.toLowerCase() === lang);
            });
        }
    </script>
</body>
</html>
