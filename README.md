# naman-sharma62
this is my 19th repository
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon Prime Video Style UI</title>
    <style>
        :root {
            --prime-blue: #00A8E1;
            --prime-bg: #0F171E;
            --prime-nav: #1A242F;
            --text-main: #FFFFFF;
            --text-muted: #8197A4;
        }

        body {
            font-family: "Amazon Ember", Arial, sans-serif;
            background-color: var(--prime-bg);
            color: var(--text-main);
            margin: 0;
            display: flex;
        }

        /* Sidebar Navigation */
        .sidebar {
            width: 80px;
            height: 100vh;
            background-color: var(--prime-nav);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 20px;
            position: fixed;
            z-index: 10;
        }

        .nav-item {
            margin-bottom: 30px;
            cursor: pointer;
            font-size: 24px;
            color: var(--text-muted);
        }

        .nav-item:hover, .nav-item.active {
            color: var(--prime-blue);
        }

        /* Main Content */
        .main-container {
            margin-left: 80px;
            width: calc(100% - 80px);
        }

        /* Hero Banner */
        .hero-banner {
            position: relative;
            height: 60vh;
            width: 100%;
            overflow: hidden;
        }

        .hero-banner iframe {
            width: 100%;
            height: 100%;
            border: none;
            filter: brightness(0.6);
        }

        .hero-info {
            position: absolute;
            bottom: 10%;
            left: 50px;
            max-width: 500px;
        }

        .prime-tag {
            background-color: var(--prime-blue);
            padding: 2px 8px;
            font-size: 12px;
            font-weight: bold;
            border-radius: 4px;
            margin-bottom: 10px;
            display: inline-block;
        }

        h1 { font-size: 42px; margin: 0 0 10px 0; }
        
        .hero-actions { display: flex; gap: 15px; margin-top: 20px; }
        .btn-play {
            background-color: var(--prime-blue);
            color: white;
            padding: 12px 30px;
            border-radius: 4px;
            border: none;
            font-weight: bold;
            cursor: pointer;
        }

        /* Content Rows */
        .content-row {
            padding: 20px 0 20px 50px;
        }

        .row-title {
            font-size: 20px;
            font-weight: bold;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .row-title span { color: var(--prime-blue); font-size: 14px; }

        .carousel {
            display: flex;
            gap: 15px;
            overflow-x: auto;
            padding-bottom: 20px;
        }

        .carousel::-webkit-scrollbar { display: none; }

        .movie-card {
            min-width: 280px;
            height: 160px;
            background: #1A242F;
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s;
            cursor: pointer;
            border: 2px solid transparent;
        }

        .movie-card:hover {
            transform: scale(1.05);
            border-color: #fff;
        }

        .movie-card iframe { width: 100%; height: 100%; border: none; }

    </style>
</head>
<body>

    <div class="sidebar">
        <div class="nav-item">🔍</div>
        <div class="nav-item active">🏠</div>
        <div class="nav-item">🎬</div>
        <div class="nav-item">📺</div>
        <div class="nav-item">⭐</div>
    </div>

    <div class="main-container">
        <div class="hero-banner">
            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?autoplay=1&mute=1&controls=0&loop=1&playlist=dQw4w9WgXcQ" allow="autoplay"></iframe>
            <div class="hero-info">
                <div class="prime-tag">✓ Included with Prime</div>
                <h1>The 555 Chronicles</h1>
                <p>An aspiring engineer from **ABES** uncovers the mysteries of monostable circuits. A race against time before the **SSB Bangalore** interview.</p>
                <div class="hero-actions">
                    <button class="btn-play">▶ Play S1 E1</button>
                    <button style="background: rgba(255,255,255,0.2); border: none; color: white; padding: 12px; border-radius: 4px;">+</button>
                </div>
            </div>
        </div>

        <div class="content-row">
            <div class="row-title">Amazon Originals <span>See more ></span></div>
            <div class="carousel">
                <div class="movie-card"><iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0"></iframe></div>
                <div class="movie-card"><iframe src="https://www.youtube.com/embed/377pxMNUTwo?controls=0"></iframe></div>
                <div class="movie-card"><iframe src="https://www.youtube.com/embed/5PXg2mqo4f0?controls=0"></iframe></div>
                <div class="movie-card"><iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ?controls=0"></iframe></div>
            </div>
        </div>
    </div>

</body>
</html>
