
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Devi Sri Arjun Health Tips</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Global Styles */
        :root {
            --primary: #ff6b6b;
            --secondary: #4ecdc4;
            --dark: #292f36;
            --light: #f7fff7;
            --accent: #ff9f1c;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f5f5f5;
            color: var(--dark);
            line-height: 1.6;
        }

        /* Header Styles */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo-container h1 {
            color: var(--primary);
            font-size: 1.8rem;
            margin-bottom: 0.2rem;
        }

        .logo-container p {
            color: var(--dark);
            font-size: 0.9rem;
            opacity: 0.8;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--primary);
        }

        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            height: 80vh;
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), 
                        url('https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            padding: 0 5rem;
            margin-top: 70px;
        }

        .hero-content {
            max-width: 600px;
            color: white;
        }

        .hero-content h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }

        .cta-button {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 0.8rem 2rem;
            font-size: 1rem;
            font-weight: bold;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s;
        }

        .cta-button:hover {
            background-color: #ff5252;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        /* Daily Tip Section */
        .daily-tip {
            padding: 4rem 2rem;
            text-align: center;
            background-color: var(--secondary);
            color: white;
        }

        .daily-tip h2 {
            margin-bottom: 2rem;
            font-size: 2rem;
        }

        .tip-container {
            max-width: 800px;
            margin: 0 auto;
        }

        .tip-text {
            font-size: 1.5rem;
            font-style: italic;
            margin-bottom: 2rem;
        }

        #new-tip-btn {
            background-color: white;
            color: var(--secondary);
            border: none;
            padding: 0.8rem 1.5rem;
            font-size: 1rem;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s;
        }

        #new-tip-btn:hover {
            background-color: var(--dark);
            color: white;
        }

        /* Workouts Section */
        .workouts {
            padding: 4rem 2rem;
            background-color: white;
        }

        .workouts h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
            color: var(--dark);
        }

        .workout-tabs {
            display: flex;
            justify-content: center;
            margin-bottom: 2rem;
            gap: 1rem;
        }

        .tab-btn {
            padding: 0.8rem 1.5rem;
            background-color: #eee;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            font-weight: bold;
            transition: all 0.3s;
        }

        .tab-btn.active {
            background-color: var(--primary);
            color: white;
        }

        .tab-btn:hover:not(.active) {
            background-color: #ddd;
        }

        .workout-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .workout-plan {
            display: none;
            background-color: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .workout-plan.active {
            display: block;
            animation: fadeIn 0.5s;
        }

        .workout-plan h3 {
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .workout-plan ul {
            list-style-position: inside;
        }

        .workout-plan ul li {
            margin-bottom: 0.5rem;
            padding-left: 1rem;
        }

        /* Exercise Demo Section */
        .exercise-demo {
            padding: 4rem 2rem;
            background-color: #f5f5f5;
        }

        .exercise-demo h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
            color: var(--dark);
        }

        .exercise-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .exercise-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }

        .exercise-card:hover {
            transform: translateY(-10px);
        }

        .exercise-img {
            height: 200px;
            background-size: cover;
            background-position: center;
        }

        .exercise-card h3 {
            padding: 1rem;
            color: var(--dark);
        }

        .view-demo {
            display: block;
            width: 100%;
            padding: 0.8rem;
            background-color: var(--primary);
            color: white;
            border: none;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
        }

        .view-demo:hover {
            background-color: #ff5252;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 2000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            overflow: auto;
        }

        .modal-content {
            background-color: white;
            margin: 5% auto;
            padding: 2rem;
            border-radius: 10px;
            max-width: 800px;
            width: 90%;
            position: relative;
        }

        .close-modal {
            position: absolute;
            right: 1rem;
            top: 1rem;
            font-size: 1.5rem;
            cursor: pointer;
            color: #aaa;
        }

        .close-modal:hover {
            color: var(--dark);
        }

        #modal-title {
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .video-placeholder {
            background-color: #eee;
            height: 400px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 1rem;
            border-radius: 5px;
        }

        /* Nutrition Section */
        .nutrition {
            padding: 4rem 2rem;
            background-color: white;
        }

        .nutrition h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
            color: var(--dark);
        }

        .nutrition-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .nutrition-card {
            background-color: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }

        .nutrition-card:hover {
            transform: translateY(-10px);
        }

        .nutrition-card i {
            font-size: 3rem;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .nutrition-card h3 {
            margin-bottom: 1rem;
            color: var(--dark);
        }

        /* Health Tips Section */
        .health-tips {
            padding: 4rem 2rem;
            background-color: #f5f5f5;
        }

        .health-tips h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
            color: var(--dark);
        }

        .tips-accordion {
            max-width: 800px;
            margin: 0 auto;
        }

        .accordion-item {
            margin-bottom: 1rem;
            border-radius: 5px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .accordion-btn {
            width: 100%;
            padding: 1rem 1.5rem;
            background-color: var(--primary);
            color: white;
            border: none;
            text-align: left;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .accordion-btn i {
            transition: transform 0.3s;
        }

        .accordion-btn.active i {
            transform: rotate(180deg);
        }

        .accordion-content {
            background-color: white;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
        }

        .accordion-content p {
            padding: 1.5rem;
        }

        /* Footer Styles */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 3rem 2rem 0;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-section h3 {
            color: var(--primary);
            margin-bottom: 1.5rem;
            font-size: 1.3rem;
        }

        .footer-section p {
            margin-bottom: 0.8rem;
            opacity: 0.8;
        }

        .footer-section i {
            margin-right: 0.5rem;
            color: var(--primary);
        }

        .social-icons {
            display: flex;
            gap: 1rem;
        }

        .social-icons a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s;
        }

        .social-icons a:hover {
            color: var(--primary);
        }

        .footer-bottom {
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.8;
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            nav ul {
                display: none;
            }
            
            .mobile-menu {
                display: block;
            }
            
            .hero {
                padding: 0 2rem;
                height: 70vh;
            }
            
            .hero-content h2 {
                font-size: 2.2rem;
            }
            
            .workout-tabs {
                flex-direction: column;
                align-items: center;
            }
        }

        @media (max-width: 480px) {
            header {
                padding: 1rem;
            }
            
            .hero {
                padding: 0 1rem;
                height: 60vh;
            }
            
            .hero-content h2 {
                font-size: 1.8rem;
            }
            
            .hero-content p {
                font-size: 1rem;
            }
            
            .cta-button {
                padding: 0.6rem 1.5rem;
            }
            
            .tip-text {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo-container">
            <h1>Devi Sri Arjun</h1>
            <p>Health & Fitness Coach</p>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#workouts">Workouts</a></li>
                <li><a href="#nutrition">Nutrition</a></li>
                <li><a href="#tips">Health Tips</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <div class="mobile-menu">
            <i class="fas fa-bars"></i>
        </div>
    </header>

    <main>
        <section id="home" class="hero">
            <div class="hero-content">
                <h2>Transform Your Life</h2>
                <p>Get fit, stay healthy, and feel amazing with personalized fitness guidance</p>
                <button class="cta-button">Start Your Journey</button>
            </div>
        </section>

        <section id="daily-tip" class="daily-tip">
            <h2>Today's Health Tip</h2>
            <div class="tip-container">
                <p class="tip-text">"Stay hydrated throughout the day. Drink at least 8 glasses of water to maintain optimal body function and energy levels."</p>
                <button id="new-tip-btn">Get Another Tip</button>
            </div>
        </section>

        <section id="workouts" class="workouts">
            <h2>Daily Workout Plans</h2>
            <div class="workout-tabs">
                <button class="tab-btn active" data-target="beginner">Beginner</button>
                <button class="tab-btn" data-target="intermediate">Intermediate</button>
                <button class="tab-btn" data-target="advanced">Advanced</button>
            </div>
            
            <div class="workout-content">
                <div id="beginner" class="workout-plan active">
                    <h3>Beginner Full Body Workout</h3>
                    <ul>
                        <li>Bodyweight Squats - 3 sets of 10 reps</li>
                        <li>Push-ups (knees or wall) - 3 sets of 8 reps</li>
                        <li>Plank - 3 sets of 20 seconds</li>
                        <li>Walking Lunges - 2 sets of 8 reps per leg</li>
                        <li>Superman - 2 sets of 10 reps</li>
                    </ul>
                </div>
                
                <div id="intermediate" class="workout-plan">
                    <h3>Intermediate Strength Training</h3>
                    <ul>
                        <li>Goblet Squats - 4 sets of 12 reps</li>
                        <li>Dumbbell Bench Press - 4 sets of 10 reps</li>
                        <li>Bent-over Rows - 3 sets of 12 reps</li>
                        <li>Romanian Deadlifts - 3 sets of 10 reps</li>
                        <li>Side Plank - 3 sets of 30 seconds per side</li>
                    </ul>
                </div>
                
                <div id="advanced" class="workout-plan">
                    <h3>Advanced HIIT Routine</h3>
                    <ul>
                        <li>Burpees - 45 seconds, 15 seconds rest</li>
                        <li>Jump Squats - 45 seconds, 15 seconds rest</li>
                        <li>Mountain Climbers - 45 seconds, 15 seconds rest</li>
                        <li>Box Jumps - 45 seconds, 15 seconds rest</li>
                        <li>Plank to Push-up - 45 seconds, 15 seconds rest</li>
                        <li>Repeat circuit 3-4 times</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="exercises" class="exercise-demo">
            <h2>Exercise Demonstrations</h2>
            <div class="exercise-gallery">
                <div class="exercise-card">
                    <div class="exercise-img" style="background-image: url('https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                    <h3>Perfect Push-up</h3>
                    <button class="view-demo" data-exercise="pushup">View Demo</button>
                </div>
                <div class="exercise-card">
                    <div class="exercise-img" style="background-image: url('https://images.unsplash.com/photo-1534258936925-c58bed479fcb?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                    <h3>Proper Squat Form</h3>
                    <button class="view-demo" data-exercise="squat">View Demo</button>
                </div>
                <div class="exercise-card">
                    <div class="exercise-img" style="background-image: url('https://images.unsplash.com/photo-1571019614243-c778b68a4ba0?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60');"></div>
                    <h3>Plank Variations</h3>
                    <button class="view-demo" data-exercise="plank">View Demo</button>
                </div>
            </div>
            
            <div id="demo-modal" class="modal">
                <div class="modal-content">
                    <span class="close-modal">&times;</span>
                    <h3 id="modal-title">Exercise Demo</h3>
                    <div id="modal-video" class="video-placeholder"></div>
                    <p id="modal-description"></p>
                </div>
            </div>
        </section>

        <section id="nutrition" class="nutrition">
            <h2>Nutrition Tips</h2>
            <div class="nutrition-cards">
                <div class="nutrition-card">
                    <i class="fas fa-apple-alt"></i>
                    <h3>Balanced Diet</h3>
                    <p>Include proteins, carbs, and healthy fats in every meal for sustained energy.</p>
                </div>
                <div class="nutrition-card">
                    <i class="fas fa-glass-whiskey"></i>
                    <h3>Hydration</h3>
                    <p>Drink at least 2-3 liters of water daily. More if you're active.</p>
                </div>
                <div class="nutrition-card">
                    <i class="fas fa-utensils"></i>
                    <h3>Meal Timing</h3>
                    <p>Eat every 3-4 hours to maintain metabolism and energy levels.</p>
                </div>
            </div>
        </se