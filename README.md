<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Novel Website</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" integrity="sha512-Fo3rlrZj/kMVq7Kkrm8t4Ov2UGjAbcD0uGi3VoWIxdz4dyVu7C2RzVyVSk8zj6OmGm0DJD27HXJpB09GPAJDoQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Roboto', sans-serif;
        }
        body {
            background: linear-gradient(135deg, #aeceff 0%, #aeceff 100%);
            color: #333;
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* Navbar Styling */
        .navbar {
            background-color: #2c3e50;
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            backdrop-filter: blur(10px);
        }

        .navbar .logo a {
            color: #2980b9;
            font-size: 1.5rem;
            text-decoration: none;
            font-family: 'Pacifico', cursive;
        }

        .navbar .nav-links a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            transition: color 0.3s ease;
        }

        .navbar .nav-links a:hover {
            color: #2980b9;
        }

        /* Hero Section Styling */
        .hero {
            background: url('https://i.pinimg.com/enabled_hi/236x/2d/83/37/2d83374e945c711357e9ac13082a9ad1.jpg') no-repeat center center/cover;
            color: white;
            text-align: center;
            padding: 120px 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            height: 80vh;
            position: relative;
            overflow: hidden;
        }
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            z-index: 2;
            text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.8);
            animation: slideIn 1.5s ease-out;
        }

        .hero p {
            font-size: 1.5rem;
            max-width: 800px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
            z-index: 2;
        }

        .hero .cta-button {
            margin-top: 20px;
            padding: 12px 30px;
            background: #2980b9;
            color: white;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            transition: background 0.3s ease;
            z-index: 2;
        }

        .hero .cta-button:hover {
            background: #2980b9;
        }
        @keyframes slideIn {
            0% { transform: translateY(-50px); opacity: 0; }
            100% { transform: translateY(0); opacity: 1; }
        }

        /* Content Layout */
        .container {
            padding: 40px 20px;
            max-width: 1200px;
            margin: auto;
        }

        /* Chapter List Styling */
        .chapter-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .chapter-list li {
            background-color: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s, background-color 0.3s;
            cursor: pointer;
        }

        .chapter-list li:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            background-color: #2980b9;
            color: white;
        }

        .chapter-list a {
            text-decoration: none;
            color: #333;
            font-weight: bold;
            display: block;
            margin-bottom: 10px;
            font-size: 1.2rem;
        }

        .chapter-list a:hover {
            color: #2980b9;
        }

        /* Footer styling */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
            font-size: 0.9rem;
        }
        footer p {
            margin: 5px 0;
        }
        
    </style>
</head>
<body>
    
    <!-- Navbar -->
    <div class="navbar">
        <div class="logo">
            <a href="home.html"><i class="fas fa-book-open"></i> My Novel</a>
        </div>
        <div class="nav-links">
            <a href="home.html">HOME</a>
            <a href="about.html">ABOUT</a>
        </div>
    </div>

    <!-- Hero Section -->
    <div class="hero">
        <h1>SELAMAT DATANG</h1>
        <p>DISINI ANDA DAPAT MELIHAT BEBERAPA CERPEN DAN NOVEL SAYA</p>
    </div>

    <!-- Main Content Section -->
    <div class="container" id="cerita">
        <h2>cerita</h2>
        <ul class="chapter-list">
            <li>
                <a href="cerita-pertama.html">Story 1:</a>
                <span>...</span>
            </li>
            <li>
                <a href="cerita-kedua.html">Story 2:</a>
                <span>...</span>
            </li>
        </ul>
    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 My Novel. All rights reserved.</p>
    </footer>

</body>
</html>
