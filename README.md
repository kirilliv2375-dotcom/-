Модельная программа профильной смены Движения Первых 
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Смены Первых - Модельная программа профильной смены Движения Первых</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/docx/7.1.0/docx.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/FileSaver.js/2.0.5/FileSaver.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        /* Подключаем шрифты */
        @font-face {
            font-family: 'Pervye Extended Bold';
            src: url('https://db.onlinewebfonts.com/t/1e6b5f4b8a7e3f6a9c5d8e7f4b3a2c1d.woff2') format('woff2'),
                 url('https://db.onlinewebfonts.com/t/1e6b5f4b8a7e3f6a9c5d8e7f4b3a2c1d.woff') format('woff');
            font-weight: bold;
            font-style: normal;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Inter V', 'Inter', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f9e8e8 0%, #efe4e4 100%);
            color: #502c2c;
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1100px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.12);
            overflow: hidden;
            animation: fadeIn 0.8s ease;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        header {
            background: linear-gradient(90deg, rgb(216, 20, 25) 0%, rgb(255, 60, 25) 100%);
            color: white;
            padding: 35px 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            transform: rotate(30deg);
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 12px;
            position: relative;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
            font-family: 'Pervye Extended Bold', sans-serif;
        }
        
        .subtitle {
            font-size: 1.3rem;
            opacity: 0.92;
            max-width: 700px;
            margin: 0 auto;
            position: relative;
            font-family: 'Inter V', 'Inter', sans-serif;
        }
        
        .content {
            padding: 35px;
        }
        
        .intro {
            margin-bottom: 35px;
            text-align: center;
            font-size: 1.15rem;
            line-height: 1.7;
            background: linear-gradient(to right, #f9f8f8, #f8e9e9);
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            font-family: 'Inter V', 'Inter', sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 120px;
        }
        
        .filter-section {
            margin-bottom: 35px;
            padding: 25px;
            background: #f9f8f8;
            border-radius: 15px;
            border-left: 6px solid rgb(216, 20, 25);
            position: relative;
        }
        
        .filter-title {
            font-size: 1.6rem;
            margin-bottom: 25px;
            color: rgb(216, 20, 25);
            display: flex;
            align-items: center;
            padding-bottom: 15px;
            border-bottom: 2px dashed #e7cccc;
            font-family: 'Pervye Extended Bold', sans-serif;
            justify-content: center;
            text-align: center;
        }
        
        .options-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-bottom: 25px;
        }
        
        .option-group {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.06);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border-top: 4px solid rgb(216, 20, 25);
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            min-height: 320px;
        }
        
        .option-group:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
        }
        
        .option-group h3 {
            margin-bottom: 20px;
            color: rgb(216, 20, 25);
            font-size: 1.3rem;
            display: flex;
            align-items: center;
            font-family: 'Pervye Extended Bold', sans-serif;
            text-align: center;
            justify-content: center;
            flex-direction: column;
            flex-grow: 0;
            min-height: 80px;
        }
        
        .option-group h3 i {
            margin-right: 0;
            margin-bottom: 10px;
            font-size: 1.5em;
        }
        
        .options {
            display: flex;
            flex-direction: column;
            gap: 15px;
            flex-grow: 1;
            justify-content: center;
            align-items: stretch;
        }
        
        .option {
            display: flex;
            align-items: center;
            padding: 15px 18px;
            background: #f9f8f8;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            border: 2px solid #ece9e9;
            position: relative;
            overflow: hidden;
            font-family: 'Inter V', 'Inter', sans-serif;
            text-align: left;
            justify-content: flex-start;
            min-height: 60px;
            height: 100%;
        }
        
        .option span {
            flex: 1;
            text-align: center;
        }
        
        .option::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(216, 20, 25, 0.1), transparent);
            transition: left 0.7s ease;
        }
        
        .option:hover::before {
            left: 100%;
        }
        
        .option:hover {
            background: #ece9e9;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
        }
        
        .option.selected {
            background: #edd4d4;
            border-color: rgb(216, 20, 25);
            box-shadow: 0 7px 20px rgba(216, 20, 25, 0.25);
            transform: translateY(-2px);
        }
        
        .option input {
            margin-right: 12px;
            transform: scale(1.2);
            accent-color: rgb(216, 20, 25);
        }

        /* Стили для ползунков приложений */
        .app-slider-group {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.06);
            margin-bottom: 25px;
            border-top: 4px solid #3366cc;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .app-slider-group h3 {
            margin-bottom: 20px;
            color: #3366cc;
            font-size: 1.3rem;
            display: flex;
            align-items: center;
            font-family: 'Pervye Extended Bold', sans-serif;
            justify-content: center;
            text-align: center;
        }

        .app-slider-group h3 i {
            margin-right: 10px;
            font-size: 1.2em;
        }

        .slider-container {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 15px;
            padding: 15px;
            background: #f8f9ff;
            border-radius: 10px;
            border: 2px solid #e6e9ff;
            transition: all 0.3s ease;
            font-family: 'Inter V', 'Inter', sans-serif;
            justify-content: space-between;
        }

        .slider-container.active {
            background: #e6eeff;
            border-color: #3366cc;
            box-shadow: 0 5px 15px rgba(51, 102, 204, 0.2);
        }

        .slider-container:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .slider {
            position: relative;
            width: 60px;
            height: 30px;
        }

        .slider input {
            opacity: 0;
            width: 0;
            height: 0;
        }

        .slider-label {
            flex: 1;
            font-weight: 500;
            color: #333;
            text-align: left;
        }

        .slider-track {
            position: absolute;
            cursor: pointer;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: #ccc;
            transition: .4s;
            border-radius: 34px;
        }

        .slider-track:before {
            position: absolute;
            content: "";
            height: 22px;
            width: 22px;
            left: 4px;
            bottom: 4px;
            background-color: white;
            transition: .4s;
            border-radius: 50%;
        }

        input:checked + .slider-track {
            background-color: #3366cc;
        }

        input:checked + .slider-track:before {
            transform: translateX(30px);
        }
        
        .selection-preview {
            background: white;
            padding: 20px;
            border-radius: 12px;
            margin-top: 25px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.06);
            border: 1px dashed rgb(216, 20, 25);
            display: none;
            text-align: center;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .selection-preview h4 {
            color: rgb(216, 20, 25);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            font-family: 'Pervye Extended Bold', sans-serif;
            justify-content: center;
            text-align: center;
        }
        
        .selection-preview h4 i {
            margin-right: 10px;
        }
        
        .preview-items {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            justify-content: center;
        }
        
        .preview-item {
            background: #f5e9e9;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.95rem;
            display: flex;
            align-items: center;
            animation: fadeIn 0.5s ease;
            font-family: 'Inter V', 'Inter', sans-serif;
            text-align: center;
            justify-content: center;
        }

        .preview-item.app {
            background: #e6eeff;
            color: #3366cc;
        }
        
        .preview-item i {
            margin-right: 8px;
            color: rgb(216, 20, 25);
        }

        .preview-item.app i {
            color: #3366cc;
        }
        
        .generate-btn {
            display: block;
            width: 100%;
            padding: 20px;
            background: linear-gradient(90deg, rgb(216, 20, 25) 0%, rgb(255, 60, 25) 100%);
            color: white;
            border: none;
            border-radius: 12px;
            font-size: 1.3rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 25px;
            box-shadow: 0 7px 20px rgba(216, 20, 25, 0.35);
            position: relative;
            overflow: hidden;
            font-family: 'Pervye Extended Bold', sans-serif;
            text-align: center;
        }
        
        .generate-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transform: translateX(-100%);
        }
        
        .generate-btn:hover::before {
            animation: shine 1.5s infinite;
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        .generate-btn:hover {
            transform: translateY(-4px);
            box-shadow: 0 10px 25px rgba(216, 20, 25, 0.45);
        }
        
        .generate-btn:active {
            transform: translateY(-1px);
        }
        
        .result-container {
            display: none;
            margin-top: 35px;
            padding: 25px;
            background: linear-gradient(to right, #f9f8f8, #f8e9e9);
            border-radius: 12px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            animation: fadeIn 0.8s ease;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border-left: 6px solid rgb(216, 20, 25);
        }
        
        .result-container h3 {
            margin-bottom: 18px;
            color: rgb(216, 20, 25);
            font-size: 1.5rem;
            font-family: 'Inter V', 'Inter', sans-serif;
            text-align: center;
        }
        
        .result-container p {
            font-size: 1.15rem;
            line-height: 1.7;
            font-family: 'Inter V', 'Inter', sans-serif;
        }
        
        .download-links {
            margin-top: 20px;
            display: flex;
            flex-direction: column;
            gap: 15px;
            width: 100%;
        }
        
        .download-link {
            display: flex;
            align-items: center;
            padding: 15px;
            background: linear-gradient(90deg, #3366cc 0%, #5599ff 100%);
            color: white;
            border-radius: 10px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(51, 102, 204, 0.3);
            font-size: 0.9rem;
            white-space: normal;
            text-align: left;
            line-height: 1.4;
            word-break: break-word;
        }
        
        .download-link:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(51, 102, 204, 0.4);
        }
        
        .download-link i {
            margin-right: 12px;
            flex-shrink: 0;
            font-size: 1.1rem;
            min-width: 24px;
        }
        
        .download-link.app-link {
            flex-direction: row;
            align-items: flex-start;
            padding: 12px 15px;
        }
        
        .app-link-content {
            display: flex;
            flex-direction: column;
            flex: 1;
        }
        
        .app-link-title {
            font-weight: 600;
            font-size: 0.9rem;
            margin-bottom: 4px;
            line-height: 1.3;
        }
        
        .app-link-subtitle {
            font-weight: 500;
            font-size: 0.8rem;
            opacity: 0.95;
            line-height: 1.2;
        }
        
        .wishes {
            margin-top: 35px;
            padding: 25px;
            background: #f9f8f8;
            border-radius: 15px;
            border-left: 6px solid rgb(216, 20, 25);
            position: relative;
        }
        
        .wishes-title {
            font-size: 1.6rem;
            margin-bottom: 25px;
            color: rgb(216, 20, 25);
            display: flex;
            align-items: center;
            padding-bottom: 15px;
            border-bottom: 2px dashed #e7cccc;
            font-family: 'Pervye Extended Bold', sans-serif;
            justify-content: center;
            text-align: center;
        }
        
        .signature {
            margin-top: 35px;
            background: linear-gradient(90deg, rgb(216, 20, 25) 0%, rgb(255, 60, 25) 100%);
            color: white;
            padding: 35px 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
            border-radius: 15px;
        }
        
        .signature::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            transform: rotate(30deg);
        }
        
        .signature p {
            font-size: 1.5rem;
            position: relative;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
            font-family: 'Pervye Extended Bold', sans-serif;
            z-index: 1;
        }
        
        @media (max-width: 768px) {
            .options-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .content {
                padding: 25px;
            }
            
            .filter-title {
                font-size: 1.4rem;
            }
            
            .wishes-title {
                font-size: 1.4rem;
            }
            
            .signature p {
                font-size: 1.3rem;
            }

            .slider-container {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }

            .slider {
                align-self: flex-end;
            }
            
            .option-group {
                min-height: 300px;
            }
            
            .option-group h3 {
                min-height: 70px;
            }
            
            .download-link {
                font-size: 0.85rem;
                padding: 12px;
            }
            
            .download-link.app-link {
                padding: 10px 12px;
            }
            
            .app-link-title {
                font-size: 0.85rem;
            }
            
            .app-link-subtitle {
                font-size: 0.75rem;
            }
            
            .download-link i {
                margin-right: 10px;
                font-size: 1rem;
            }
        }
        
        @media (max-width: 480px) {
            .download-link {
                font-size: 0.8rem;
                padding: 10px;
            }
            
            .app-link-title {
                font-size: 0.8rem;
            }
            
            .app-link-subtitle {
                font-size: 0.7rem;
            }
            
            .download-link i {
                margin-right: 8px;
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>СМЕНЫ ПЕРВЫХ</h1>
            <p class="subtitle">Модельная программа профильной смены Движения Первых</p>
        </header>
        
        <div class="content">
            <div class="intro">
                <p>Для составления программы воспользуйтесь фильтром, предложенным на данной странице.</p>
                <p>В результате вы получите документ, в котором выдержана логика проведения Смен Первых.</p>
                <p>Вам останется заполнить вариативный модуль программы</p>
                <p>в соответствии с предложенными в документе формами.</p>
            </div>
            
            <h2 class="filter-title">
                Давайте приступим!
            </h2>
            
            <div class="filter-section">
                <div class="options-grid">
                    <div class="option-group">
                        <h3><i class="fas fa-users"></i> Выберите возраст участников смены</h3>
                        <div class="options">
                            <label class="option">
                                <input type="radio" name="age" value="7-10">
                                <span>7 - 10 лет</span>
                            </label>
                            <label class="option">
                                <input type="radio" name="age" value="11-14">
                                <span>11 - 14 лет</span>
                            </label>
                            <label class="option">
                                <input type="radio" name="age" value="15-17">
                                <span>15 - 17 лет</span>
                            </label>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <h3><i class="fas fa-campground"></i> Выберите тип организации отдыха детей и их оздоровления</h3>
                        <div class="options">
                            <label class="option">
                                <input type="radio" name="type" value="country">
                                <span>Загородный лагерь</span>
                            </label>
                            <label class="option">
                                <input type="radio" name="type" value="school">
                                <span>Пришкольный лагерь</span>
                            </label>
                        </div>
                    </div>
                    
                    <div class="option-group">
                        <h3><i class="fas fa-calendar-alt"></i> Выберите продолжительность Смены Первых</h3>
                        <div class="options">
                            <label class="option">
                                <input type="radio" name="duration" value="14">
                                <span>14 дней</span>
                            </label>
                            <label class="option">
                                <input type="radio" name="duration" value="18">
                                <span>18 дней</span>
                            </label>
                            <label class="option">
                                <input type="radio" name="duration" value="21">
                                <span>21 день</span>
                            </label>
                        </div>
                    </div>
                </div>

                <!-- Блок выбора приложений -->
                <div class="app-slider-group">
                    <h3><i class="fas fa-paperclip"></i> Выберите дополнительные приложения</h3>
                    <div class="slider-container" id="app1Container">
                        <label class="slider">
                            <input type="checkbox" id="app1Toggle">
                            <span class="slider-track"></span>
                        </label>
                        <span class="slider-label">Приложение 1: Модель организации самоуправления на профильной смене Движения Первых</span>
                    </div>
                    <div class="slider-container" id="app2Container">
                        <label class="slider">
                            <input type="checkbox" id="app2Toggle">
                            <span class="slider-track"></span>
                        </label>
                        <span class="slider-label">Приложение 2: Общие рекомендации по разработке игровой модели профильных смен Движения первых</span>
                    </div>
                </div>
                
                <div id="selectionPreview" class="selection-preview">
                    <h4><i class="fas fa-check-circle"></i> Ваш выбор:</h4>
                    <div class="preview-items">
                        <div id="agePreview" class="preview-item" style="display: none;">
                            <i class="fas fa-user-friends"></i> Возраст: <span></span>
                        </div>
                        <div id="durationPreview" class="preview-item" style="display: none;">
                            <i class="fas fa-calendar-check"></i> Длительность: <span></span>
                        </div>
                        <div id="typePreview" class="preview-item" style="display: none;">
                            <i class="fas fa-map-marker-alt"></i> Тип: <span></span>
                        </div>
                        <div id="app1Preview" class="preview-item app" style="display: none;">
                            <i class="fas fa-paperclip"></i> Приложение 1
                        </div>
                        <div id="app2Preview" class="preview-item app" style="display: none;">
                            <i class="fas fa-paperclip"></i> Приложение 2
                        </div>
                    </div>
                </div>
                
                <button id="generateBtn" class="generate-btn">
                    <i class="fas fa-file-word"></i> Сформировать программу профильной смены Движения Первых
                </button>
                
                <div id="resultContainer" class="result-container">
                    <h3>Ваша программа успешно сформирована!</h3>
                    <p>Теперь вы можете скачать выбранные документы:</p>
                    <div class="download-links" id="downloadLinks">
                        <!-- Ссылки для скачивания будут добавлены здесь -->
                    </div>
                </div>
            </div>
            
            <div class="wishes">
                <h2 class="wishes-title">
                    Желаем успехов в реализации Смены Первых!
                </h2>
            </div>

            <div class="signature">
                <p>С уважением, команда Движения Первых</p>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const options = document.querySelectorAll('.option');
            const generateBtn = document.getElementById('generateBtn');
            const resultContainer = document.getElementById('resultContainer');
            const selectionPreview = document.getElementById('selectionPreview');
            const agePreview = document.getElementById('agePreview');
            const durationPreview = document.getElementById('durationPreview');
            const typePreview = document.getElementById('typePreview');
            const app1Preview = document.getElementById('app1Preview');
            const app2Preview = document.getElementById('app2Preview');
            const app1Toggle = document.getElementById('app1Toggle');
            const app2Toggle = document.getElementById('app2Toggle');
            const app1Container = document.getElementById('app1Container');
            const app2Container = document.getElementById('app2Container');
            const downloadLinks = document.getElementById('downloadLinks');
            
            // Сопоставление выбора пользователя с ссылками на облако Mail.ru
            const documentMapping = {
                // 7-10 лет
                '7-10': {
                    'country': {
                        '14': 'https://cloud.mail.ru/public/CBhJ/DBuV3yZDb',
                        '18': 'https://cloud.mail.ru/public/EPCw/ciJRjWmFZ',
                        '21': 'https://cloud.mail.ru/public/PS9C/kpMi9bEXF'
                    },
                    'school': {
                        '14': 'https://cloud.mail.ru/public/gCCW/jACVNJwjX',
                        '18': 'https://cloud.mail.ru/public/JBBw/8AKs3k8uU',
                        '21': 'https://cloud.mail.ru/public/Tt1C/TwhKDzETN'
                    }
                },
                // 11-14 лет
                '11-14': {
                    'country': {
                        '14': 'https://cloud.mail.ru/public/oVtF/BLAxs6Dag',
                        '18': 'https://cloud.mail.ru/public/m9t8/Gwi5p4XtJ',
                        '21': 'https://cloud.mail.ru/public/f6PN/rCpmouyHr'
                    },
                    'school': {
                        '14': 'https://cloud.mail.ru/public/cWE4/kkVCsedFh',
                        '18': 'https://cloud.mail.ru/public/w64P/6xPGdDxY2',
                        '21': 'https://cloud.mail.ru/public/LaCY/zWMiYzp9w'
                    }
                },
                // 15-17 лет
                '15-17': {
                    'country': {
                        '14': 'https://cloud.mail.ru/public/6v4j/3yYrxdnge',
                        '18': 'https://cloud.mail.ru/public/v3qA/hHcUWstF2',
                        '21': 'https://cloud.mail.ru/public/JXcf/eVMntfqFb'
                    },
                    'school': {
                        '14': 'https://cloud.mail.ru/public/xRRW/s9WKC4H8v',
                        '18': 'https://cloud.mail.ru/public/qmGu/tPRTto4yn',
                        '21': 'https://cloud.mail.ru/public/KxSb/WPiY9YkNk'
                    }
                },
                // Приложения
                'app1': 'https://cloud.mail.ru/public/HtyV/yRM67E3MP',
                'app2': 'https://cloud.mail.ru/public/4RDd/vbdjc8bbB'
            };
            
            // Добавляем обработчики для стилизации выбранных опций
            options.forEach(option => {
                const radio = option.querySelector('input[type="radio"]');
                
                radio.addEventListener('change', function() {
                    // Убираем класс selected у всех опций в той же группе
                    const groupOptions = option.closest('.options').querySelectorAll('.option');
                    groupOptions.forEach(opt => opt.classList.remove('selected'));
                    
                    // Добавляем класс selected к выбранной опции
                    if (this.checked) {
                        option.classList.add('selected');
                    }
                    
                    // Обновляем предпросмотр выбора
                    updateSelectionPreview();
                });
            });

            // Обработчики для ползунков приложений
            app1Toggle.addEventListener('change', function() {
                app1Container.classList.toggle('active', this.checked);
                updateSelectionPreview();
            });

            app2Toggle.addEventListener('change', function() {
                app2Container.classList.toggle('active', this.checked);
                updateSelectionPreview();
            });
            
            // Функция обновления предпросмотра выбора
            function updateSelectionPreview() {
                const ageSelected = document.querySelector('input[name="age"]:checked');
                const durationSelected = document.querySelector('input[name="duration"]:checked');
                const typeSelected = document.querySelector('input[name="type"]:checked');
                const app1Selected = app1Toggle.checked;
                const app2Selected = app2Toggle.checked;
                
                // Показываем/скрываем предпросмотр в зависимости от выбора
                if (ageSelected || durationSelected || typeSelected || app1Selected || app2Selected) {
                    selectionPreview.style.display = 'flex';
                } else {
                    selectionPreview.style.display = 'none';
                }
                
                // Обновляем текст предпросмотра
                if (ageSelected) {
                    agePreview.style.display = 'flex';
                    agePreview.querySelector('span').textContent = getAgeText(ageSelected.value);
                } else {
                    agePreview.style.display = 'none';
                }
                
                if (durationSelected) {
                    durationPreview.style.display = 'flex';
                    durationPreview.querySelector('span').textContent = getDurationText(durationSelected.value);
                } else {
                    durationPreview.style.display = 'none';
                }
                
                if (typeSelected) {
                    typePreview.style.display = 'flex';
                    typePreview.querySelector('span').textContent = getTypeText(typeSelected.value);
                } else {
                    typePreview.style.display = 'none';
                }

                if (app1Selected) {
                    app1Preview.style.display = 'flex';
                } else {
                    app1Preview.style.display = 'none';
                }

                if (app2Selected) {
                    app2Preview.style.display = 'flex';
                } else {
                    app2Preview.style.display = 'none';
                }
            }
            
            // Обработчик для кнопки генерации
            generateBtn.addEventListener('click', function() {
                // Проверяем, все ли обязательные поля заполнены
                const ageSelected = document.querySelector('input[name="age"]:checked');
                const durationSelected = document.querySelector('input[name="duration"]:checked');
                const typeSelected = document.querySelector('input[name="type"]:checked');
                
                if (!ageSelected || !durationSelected || !typeSelected) {
                    alert('Пожалуйста, заполните все обязательные поля: возраст, продолжительность и тип лагеря.');
                    return;
                }
                
                // Определяем, какие документы выбрать на основе выбора пользователя
                const selectedDocuments = determineDocuments(
                    ageSelected.value,
                    durationSelected.value,
                    typeSelected.value,
                    app1Toggle.checked,
                    app2Toggle.checked
                );
                
                // Показываем ссылки для скачивания
                showDownloadLinks(selectedDocuments);
            });
            
            // Функция для определения документов на основе выбора пользователя
            function determineDocuments(age, duration, type, app1, app2) {
                const documents = [];
                
                // Основной документ
                if (documentMapping[age] && documentMapping[age][type] && documentMapping[age][type][duration]) {
                    documents.push({
                        name: getDocumentName(age, duration, type),
                        url: documentMapping[age][type][duration]
                    });
                }
                
                // Приложения
                if (app1 && documentMapping['app1']) {
                    documents.push({
                        name: 'Приложение 1: Модель организации самоуправления на профильной смене Движения Первых',
                        url: documentMapping['app1']
                    });
                }
                
                if (app2 && documentMapping['app2']) {
                    documents.push({
                        name: 'Приложение 2: Общие рекомендации по разработке игровой модели профильных смен Движения первых',
                        url: documentMapping['app2']
                    });
                }
                
                return documents;
            }
            
            // Функция для отображения ссылок для скачивания
            function showDownloadLinks(documents) {
                // Показываем сообщение о генерации
                generateBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Формируем документ...';
                generateBtn.disabled = true;
                
                // Очищаем контейнер с ссылками
                downloadLinks.innerHTML = '';
                
                // Добавляем ссылки для скачивания
                documents.forEach(doc => {
                    const link = document.createElement('a');
                    link.href = doc.url;
                    link.target = '_blank';
                    link.className = 'download-link';
                    
                    // Для приложений используем двухстрочный текст с полными названиями
                    if (doc.name.includes('Приложение 1')) {
                        link.classList.add('app-link');
                        link.innerHTML = `
                            <i class="fas fa-download"></i>
                            <div class="app-link-content">
                                <div class="app-link-title">Скачать Приложение 1:</div>
                                <div class="app-link-subtitle">Модель организации самоуправления на профильной смене Движения Первых</div>
                            </div>
                        `;
                    } else if (doc.name.includes('Приложение 2')) {
                        link.classList.add('app-link');
                        link.innerHTML = `
                            <i class="fas fa-download"></i>
                            <div class="app-link-content">
                                <div class="app-link-title">Скачать Приложение 2:</div>
                                <div class="app-link-subtitle">Общие рекомендации по разработке игровой модели профильных смен Движения первых</div>
                            </div>
                        `;
                    } else {
                        // Для обычных документов оставляем как было
                        link.innerHTML = `<i class="fas fa-download"></i> Скачать ${doc.name}`;
                    }
                    
                    downloadLinks.appendChild(link);
                });
                
                // Восстанавливаем кнопку
                setTimeout(function() {
                    generateBtn.innerHTML = '<i class="fas fa-file-word"></i> Сформировать программу профильной смены Движения Первых';
                    generateBtn.disabled = false;
                    
                    // Показываем результат
                    resultContainer.style.display = 'flex';
                    
                    // Прокручиваем к результату
                    resultContainer.scrollIntoView({ behavior: 'smooth' });
                }, 1000);
            }
            
            // Функция для получения имени документа
            function getDocumentName(age, duration, type) {
                const ageText = getAgeText(age);
                const durationText = getDurationText(duration);
                const typeText = getTypeText(type);
                
                return `Программа (${ageText}, ${typeText}, ${durationText})`;
            }
            
            // Вспомогательные функции для получения текстовых представлений
            function getAgeText(age) {
                switch(age) {
                    case '7-10': return '7-10 лет';
                    case '11-14': return '11-14 лет';
                    case '15-17': return '15-17 лет';
                    default: return '';
                }
            }
            
            function getDurationText(duration) {
                return `${duration} дней`;
            }
            
            function getTypeText(type) {
                switch(type) {
                    case 'school': return 'Пришкольный лагерь';
                    case 'country': return 'Загородный лагерь';
                    default: return '';
                }
            }
        });
    </script>
</body>
</html>
