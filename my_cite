<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мурр ✦ Блог любителей кошек</title>
    <!-- Font Awesome для иконок (социальные сети, контакты) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* ---------- ГЛОБАЛЬНЫЙ СБРОС И ПЕРЕМЕННЫЕ ---------- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, system-ui, -apple-system, sans-serif;
        }

        :root {
            --bg-body: #fcf7f2;
            --bg-card: #ffffff;
            --primary: #d48c7c;
            --primary-dark: #b46a5a;
            --secondary: #f0e3d9;
            --text-main: #3e2e2a;
            --text-light: #7a625a;
            --border-soft: #eddcd2;
            --shadow: 0 8px 24px rgba(90, 60, 50, 0.08);
            --radius: 28px;
            --transition: 0.25s ease;
        }

        body {
            background-color: var(--bg-body);
            color: var(--text-main);
            line-height: 1.6;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        .container {
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 30px;
            width: 100%;
        }

        /* ---------- ШАПКА (ХЕДЕР) ---------- */
        .header {
            background: var(--bg-card);
            border-bottom: 2px solid var(--border-soft);
            padding: 18px 0;
            box-shadow: 0 4px 12px rgba(0,0,0,0.02);
            position: sticky;
            top: 0;
            z-index: 50;
        }

        .header .container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
        }

        .logo a {
            font-size: 2rem;
            font-weight: 700;
            letter-spacing: -0.5px;
            color: var(--primary-dark);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .logo i {
            font-size: 2rem;
            color: var(--primary);
        }

        .nav-menu {
            display: flex;
            gap: 24px;
            flex-wrap: wrap;
        }

        .nav-menu a {
            text-decoration: none;
            color: var(--text-main);
            font-weight: 500;
            font-size: 1.05rem;
            padding: 6px 0;
            border-bottom: 3px solid transparent;
            transition: var(--transition);
        }

        .nav-menu a:hover,
        .nav-menu a.active {
            border-bottom-color: var(--primary);
            color: var(--primary-dark);
        }

        /* ---------- ХЛЕБНЫЕ КРОШКИ ---------- */
        .breadcrumb {
            padding: 20px 0 8px 0;
            font-size: 0.9rem;
            color: var(--text-light);
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 6px;
        }

        .breadcrumb a {
            color: var(--primary-dark);
            text-decoration: none;
            transition: var(--transition);
        }

        .breadcrumb a:hover {
            text-decoration: underline;
        }

        .breadcrumb i {
            font-size: 0.7rem;
            margin: 0 4px;
            color: var(--text-light);
        }

        .breadcrumb .current {
            font-weight: 500;
            color: var(--text-main);
        }

        /* ---------- ОСНОВНОЙ КОНТЕНТ ---------- */
        .main-content {
            flex: 1;
            padding: 20px 0 40px;
        }

        /* заголовки страниц */
        .page-title {
            font-size: 2.4rem;
            font-weight: 700;
            color: var(--text-main);
            margin-bottom: 20px;
            letter-spacing: -0.02em;
            border-left: 8px solid var(--primary);
            padding-left: 20px;
        }

        .page-subtitle {
            font-size: 1.2rem;
            color: var(--text-light);
            margin-top: -8px;
            margin-bottom: 32px;
        }

        /* карточки для постов / контента */
        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            margin: 30px 0;
        }

        .card {
            background: var(--bg-card);
            border-radius: var(--radius);
            padding: 24px 22px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border: 1px solid var(--border-soft);
        }

        .card:hover {
            transform: translateY(-6px);
            box-shadow: 0 16px 36px rgba(90, 60, 50, 0.12);
        }

        .card h3 {
            font-size: 1.5rem;
            margin-bottom: 6px;
            color: var(--primary-dark);
        }

        .card .meta {
            font-size: 0.85rem;
            color: var(--text-light);
            margin-bottom: 12px;
            display: flex;
            gap: 12px;
        }

        .card p {
            color: var(--text-main);
            margin-bottom: 12px;
        }

        .card .tag {
            display: inline-block;
            background: var(--secondary);
            color: var(--text-main);
            padding: 4px 14px;
            border-radius: 40px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        /* ---------- ФОРМА ОБРАТНОЙ СВЯЗИ ---------- */
        .contact-form {
            background: var(--bg-card);
            padding: 36px 40px;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            border: 1px solid var(--border-soft);
            max-width: 680px;
            margin: 30px 0;
        }

        .contact-form label {
            font-weight: 600;
            display: block;
            margin: 16px 0 4px 0;
        }

        .contact-form input,
        .contact-form textarea,
        .contact-form select {
            width: 100%;
            padding: 14px 18px;
            border: 2px solid var(--border-soft);
            border-radius: 40px;
            font-size: 1rem;
            background: var(--bg-body);
            transition: var(--transition);
            outline: none;
        }

        .contact-form input:focus,
        .contact-form textarea:focus {
            border-color: var(--primary);
            background: white;
        }

        .contact-form textarea {
            min-height: 130px;
            border-radius: 28px;
            resize: vertical;
        }

        .btn {
            background: var(--primary);
            border: none;
            color: white;
            padding: 14px 38px;
            border-radius: 60px;
            font-weight: 600;
            font-size: 1.1rem;
            cursor: pointer;
            transition: var(--transition);
            margin-top: 18px;
            display: inline-block;
            border: 2px solid transparent;
        }

        .btn:hover {
            background: var(--primary-dark);
            transform: scale(0.97);
            box-shadow: 0 8px 18px rgba(180, 90, 70, 0.25);
        }

        /* ---------- ПОДВАЛ (ФУТЕР) ---------- */
        .footer {
            background: #2f2420;
            color: #f0e3d9;
            padding: 40px 0 28px;
            margin-top: 30px;
            border-top: 6px solid var(--primary);
        }

        .footer .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }

        .footer-col h4 {
            font-size: 1.2rem;
            margin-bottom: 12px;
            color: #f7e8df;
            letter-spacing: 0.3px;
        }

        .footer-col p,
        .footer-col a {
            color: #d6c4bb;
            text-decoration: none;
            display: block;
            margin: 4px 0;
            transition: var(--transition);
        }

        .footer-col a:hover {
            color: white;
            padding-left: 4px;
        }

        .footer-social a {
            display: inline-block;
            margin-right: 18px;
            font-size: 1.8rem;
            color: #d6c4bb;
            transition: var(--transition);
        }

        .footer-social a:hover {
            color: white;
            transform: scale(1.1);
        }

        .footer-bottom {
            border-top: 1px solid #4d3832;
            margin-top: 28px;
            padding-top: 20px;
            text-align: center;
            font-size: 0.9rem;
            color: #b9a69b;
            width: 100%;
        }

        /* ---------- АДАПТИВНОСТЬ ---------- */
        @media (max-width: 768px) {
            .header .container {
                flex-direction: column;
                gap: 12px;
            }
            .nav-menu {
                justify-content: center;
                gap: 14px;
            }
            .page-title {
                font-size: 2rem;
            }
            .contact-form {
                padding: 24px;
            }
            .footer .container {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }
            .footer-social a {
                margin: 0 10px;
            }
        }

        /* ---------- СТИЛИ ДЛЯ ОТДЕЛЬНЫХ СТРАНИЦ (примеры) ---------- */
        .about-text {
            background: var(--bg-card);
            padding: 30px 36px;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            border: 1px solid var(--border-soft);
            font-size: 1.1rem;
            line-height: 1.8;
        }

        .team-list {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }

        .team-item {
            background: var(--bg-card);
            padding: 14px 28px;
            border-radius: 80px;
            border: 1px solid var(--border-soft);
            box-shadow: var(--shadow);
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .team-item i {
            font-size: 1.8rem;
            color: var(--primary);
        }

        /* галерея (для страницы "Галерея") */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 24px;
            margin: 28px 0;
        }

        .gallery-grid .card {
            padding: 12px;
            text-align: center;
            background: var(--bg-card);
            border-radius: 32px;
        }

        .gallery-grid .card i {
            font-size: 4.4rem;
            color: var(--primary);
            margin: 16px 0 6px;
        }
    </style>
</head>
<body>

<!-- ========== ШАПКА (ХЕДЕР) ========== -->
<header class="header">
    <div class="container">
        <div class="logo">
            <a href="#"><i class="fas fa-paw"></i> Мурр<span style="color:var(--primary);">блог</span></a>
        </div>
        <nav class="nav-menu">
            <a href="#" class="active" id="nav-home">Главная</a>
            <a href="#" id="nav-about">О нас</a>
            <a href="#" id="nav-gallery">Галерея</a>
            <a href="#" id="nav-contacts">Контакты</a>
            <a href="#" id="nav-feedback">Обратная связь</a>
        </nav>
    </div>
</header>

<!-- ========== ОСНОВНАЯ ЧАСТЬ ========== -->
<main class="main-content">
    <div class="container">

        <!-- ХЛЕБНЫЕ КРОШКИ (динамические через JS) -->
        <div class="breadcrumb" id="breadcrumb">
            <a href="#">Главная</a>
            <i class="fas fa-chevron-right"></i>
            <span class="current" id="breadcrumb-current">Блог</span>
        </div>

        <!-- КОНТЕЙНЕР ДЛЯ ДИНАМИЧЕСКОГО КОНТЕНТА СТРАНИЦ -->
        <div id="page-content">
            <!-- начальное содержимое — Главная -->
            <h1 class="page-title">🐾 Мурр-посты</h1>
            <p class="page-subtitle">Свежие истории от любителей кошек</p>
            <div class="card-grid" id="home-grid">
                <div class="card"><h3>Соня-лежебока</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 12.06.2026</span><span><i class="far fa-comment"></i> 14</span></div><p>Рыжая Соня обожает спать на солнце. За день она меняет 5 мест, но всегда находит самый тёплый уголок ☀️</p><span class="tag">#лежебока</span></div>
                <div class="card"><h3>Мурзик-исследователь</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 10.06.2026</span><span><i class="far fa-comment"></i> 8</span></div><p>Мурзик открыл новую коробку из-под чайника. Теперь это его личная крепость, вход строго по паролю.</p><span class="tag">#исследователь</span></div>
                <div class="card"><h3>Королева Багира</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 08.06.2026</span><span><i class="far fa-comment"></i> 21</span></div><p>Чёрная красавица Багира требует почесать ей живот. Но только когда она сама этого захочет. График — по настроению.</p><span class="tag">#королева</span></div>
                <div class="card"><h3>Котята-карапузы</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 05.06.2026</span><span><i class="far fa-comment"></i> 32</span></div><p>Трое малышей устроили гонки по коридору. Победила дружба и разбитая ваза (но мы не будем о грустном).</p><span class="tag">#карапузы</span></div>
            </div>
        </div>
    </div>
</main>

<!-- ========== ПОДВАЛ (ФУТЕР) ========== -->
<footer class="footer">
    <div class="container">
        <div class="footer-col">
            <h4><i class="fas fa-paw"></i> Муррблог</h4>
            <p>Блог для тех, кто обожает кошек. Делимся историями, советами и любовью 🐈</p>
        </div>
        <div class="footer-col">
            <h4>Навигация</h4>
            <a href="#" id="footer-home">Главная</a>
            <a href="#" id="footer-about">О нас</a>
            <a href="#" id="footer-gallery">Галерея</a>
            <a href="#" id="footer-contacts">Контакты</a>
            <a href="#" id="footer-feedback">Обратная связь</a>
        </div>
        <div class="footer-col footer-social">
            <h4>Мы в соцсетях</h4>
            <a href="#"><i class="fab fa-telegram"></i></a>
            <a href="#"><i class="fab fa-vk"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
        </div>
        <div class="footer-bottom">
            <span>© 2026 Муррблог · Сделано с ❤️ и мурчанием</span>
        </div>
    </div>
</footer>


<!-- ========== JavaScript (роутинг 5 страниц, хлебные крошки) ========== -->
<script>
    (function() {
        // ----- ДАННЫЕ СТРАНИЦ -----
        const pages = {
            home: {
                title: 'Главная',
                breadcrumb: 'Блог',
                render: () => `
                    <h1 class="page-title">🐾 Мурр-посты</h1>
                    <p class="page-subtitle">Свежие истории от любителей кошек</p>
                    <div class="card-grid">
                        <div class="card"><h3>Соня-лежебока</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 12.06.2026</span><span><i class="far fa-comment"></i> 14</span></div><p>Рыжая Соня обожает спать на солнце. За день она меняет 5 мест, но всегда находит самый тёплый уголок ☀️</p><span class="tag">#лежебока</span></div>
                        <div class="card"><h3>Мурзик-исследователь</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 10.06.2026</span><span><i class="far fa-comment"></i> 8</span></div><p>Мурзик открыл новую коробку из-под чайника. Теперь это его личная крепость, вход строго по паролю.</p><span class="tag">#исследователь</span></div>
                        <div class="card"><h3>Королева Багира</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 08.06.2026</span><span><i class="far fa-comment"></i> 21</span></div><p>Чёрная красавица Багира требует почесать ей живот. Но только когда она сама этого захочет. График — по настроению.</p><span class="tag">#королева</span></div>
                        <div class="card"><h3>Котята-карапузы</h3><div class="meta"><span><i class="far fa-calendar-alt"></i> 05.06.2026</span><span><i class="far fa-comment"></i> 32</span></div><p>Трое малышей устроили гонки по коридору. Победила дружба и разбитая ваза (но мы не будем о грустном).</p><span class="tag">#карапузы</span></div>
                    </div>
                `
            },
            about: {
                title: 'О нас',
                breadcrumb: 'О нас',
                render: () => `
                    <h1 class="page-title">😺 О нашем блоге</h1>
                    <p class="page-subtitle">Мы — команда кошатников, которые любят пушистых</p>
                    <div class="about-text">
                        <p><i class="fas fa-cat" style="color:var(--primary);font-size:2rem;margin-right:12px;"></i> Муррблог создан в 2020 году. Мы пишем о кошках, их повадках, забавных случаях, а также делимся лайфхаками по уходу. В нашей команде — ветеринары, фелинологи и просто обожатели мурлыканья.</p>
                        <p>Наша цель — создать уютное сообщество, где каждый найдет историю о своём любимце.</p>
                        <div class="team-list">
                            <div class="team-item"><i class="fas fa-user-circle"></i> Алина — редактор</div>
                            <div class="team-item"><i class="fas fa-user-circle"></i> Сергей — фотограф</div>
                            <div class="team-item"><i class="fas fa-user-circle"></i> Маша — волонтёр</div>
                            <div class="team-item"><i class="fas fa-user-circle"></i> Барсик — главный кот</div>
                        </div>
                    </div>
                `
            },
            gallery: {
                title: 'Галерея',
                breadcrumb: 'Галерея',
                render: () => `
                    <h1 class="page-title">📸 Кошачья галерея</h1>
                    <p class="page-subtitle">Лучшие моменты наших пушистых друзей</p>
                    <div class="gallery-grid">
                        <div class="card"><i class="fas fa-cat"></i><p>Рыжик</p></div>
                        <div class="card"><i class="fas fa-cat"></i><p>Снежок</p></div>
                        <div class="card"><i class="fas fa-cat"></i><p>Персик</p></div>
                        <div class="card"><i class="fas fa-cat"></i><p>Барсик</p></div>
                        <div class="card"><i class="fas fa-cat"></i><p>Мурка</p></div>
                        <div class="card"><i class="fas fa-cat"></i><p>Тигря</p></div>
                    </div>
                `
            },
            contacts: {
                title: 'Контакты',
                breadcrumb: 'Контакты',
                render: () => `
                    <h1 class="page-title">📬 Наши контакты</h1>
                    <p class="page-subtitle">Всегда рады новым друзьям и читателям</p>
                    <div style="background:var(--bg-card);padding:30px 36px;border-radius:var(--radius);border:1px solid var(--border-soft);">
                        <p><i class="fas fa-envelope" style="color:var(--primary);width:28px;"></i> <strong>Email:</strong> hello@murrblog.ru</p>
                        <p><i class="fas fa-phone" style="color:var(--primary);width:28px;"></i> <strong>Телефон:</strong> +7 (999) 123-45-67</p>
                        <p><i class="fas fa-map-pin" style="color:var(--primary);width:28px;"></i> <strong>Адрес:</strong> г. Мурманск, ул. Кошачья, 9</p>
                        <p><i class="fas fa-clock" style="color:var(--primary);width:28px;"></i> <strong>Режим работы:</strong> онлайн 24/7, офис — с 10 до 19</p>
                    </div>
                `
            },
            feedback: {
                title: 'Обратная связь',
                breadcrumb: 'Обратная связь',
                render: () => `
                    <h1 class="page-title">✉️ Напишите нам</h1>
                    <p class="page-subtitle">Ваши пожелания, вопросы или просто мурчание — мы всё прочитаем!</p>
                    <div class="contact-form">
                        <form id="feedbackForm">
                            <label for="name">Ваше имя <span style="color:var(--primary);">*</span></label>
                            <input type="text" id="name" placeholder="Например: Екатерина" required>

                            <label for="email">Email <span style="color:var(--primary);">*</span></label>
                            <input type="email" id="email" placeholder="kot@example.com" required>

                            <label for="subject">Тема</label>
                            <input type="text" id="subject" placeholder="Почему кошки мурчат?">

                            <label for="message">Сообщение <span style="color:var(--primary);">*</span></label>
                            <textarea id="message" placeholder="Расскажите о вашем коте..." required></textarea>

                            <button type="submit" class="btn"><i class="fas fa-paper-plane"></i>  Отправить</button>
                            <p style="margin-top:14px;font-size:0.9rem;color:var(--text-light);"><i class="fas fa-info-circle"></i> Мы ответим в течение 24 часов</p>
                        </form>
                    </div>
                `
            }
        };

        // ----- ЭЛЕМЕНТЫ -----
        const content = document.getElementById('page-content');
        const breadcrumbCurrent = document.getElementById('breadcrumb-current');
        const navLinks = document.querySelectorAll('.nav-menu a');
        const footerLinks = document.querySelectorAll('.footer-col a'); // все ссылки в футере, но нужны только навигационные

        // ----- ФУНКЦИЯ ПЕРЕХОДА -----
        function navigateTo(pageId) {
            const page = pages[pageId];
            if (!page) return;

            // обновить содержимое
            content.innerHTML = page.render();

            // обновить хлебные крошки
            breadcrumbCurrent.textContent = page.breadcrumb;

            // обновить активный класс в навигации (шапка)
            navLinks.forEach(link => link.classList.remove('active'));
            const activeNav = document.getElementById(`nav-${pageId}`);
            if (activeNav) activeNav.classList.add('active');

            // если страница "feedback" — вешаем обработчик на форму (после рендера)
            if (pageId === 'feedback') {
                const form = document.getElementById('feedbackForm');
                if (form) {
                    form.addEventListener('submit', function(e) {
                        e.preventDefault();
                        alert('🐱 Спасибо! Ваше сообщение отправлено (в демо-режиме). Мы мурчим от радости!');
                        form.reset();
                    });
                }
            }

            // прокрутка наверх
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // ----- ОБРАБОТЧИКИ НАВИГАЦИИ (шапка) -----
        navLinks.forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const id = this.id.replace('nav-', '');
                if (pages[id]) navigateTo(id);
            });
        });

        // ----- ОБРАБОТЧИКИ ФУТЕРА (только навигационные ссылки) -----
        document.querySelectorAll('.footer-col a').forEach(link => {
            link.addEventListener('click', function(e) {
                // если ссылка содержит # или пустой href, перехватываем
                const href = this.getAttribute('href');
                if (href && href.startsWith('#')) {
                    e.preventDefault();
                    // определяем id страницы по id ссылки (footer-home и т.д.)
                    const id = this.id.replace('footer-', '');
                    if (pages[id]) navigateTo(id);
                }
            });
        });

        // ----- СТАРТ: ГЛАВНАЯ -----
        navigateTo('home');

        // также чтобы ссылки в логотипе вели на главную
        document.querySelector('.logo a')?.addEventListener('click', function(e) {
            e.preventDefault();
            navigateTo('home');
        });

        // обработка для "хлебных крошек" - клик по "Главная" ведёт на home
        document.querySelector('.breadcrumb a')?.addEventListener('click', function(e) {
            e.preventDefault();
            navigateTo('home');
        });

    })();
</script>
</body>
</html>
