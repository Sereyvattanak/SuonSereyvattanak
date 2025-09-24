
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sereyvattanak Suon | Academic CV</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2c3e50;
            --primary-light: #34495e;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --text: #333;
            --text-light: #7f8c8d;
            --border-radius: 10px;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: var(--text);
            line-height: 1.6;
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1000px;
            margin: 0 auto;
        }

        /* Header Styles with Photo */
        header {
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 40px;
            text-align: center;
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
        }

        .profile-header {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .profile-img-container {
            flex-shrink: 0;
            width: 200px;
            height: 250px;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
            border: 4px solid white;
        }

        .profile-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }

        .profile-text {
            text-align: left;
            max-width: 500px;
        }

        .name {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 10px;
            color: var(--primary);
            line-height: 1.2;
        }

        .title {
            font-size: 1.3rem;
            color: var(--secondary);
            margin-bottom: 20px;
            font-weight: 500;
        }

        .contact-info {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 15px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.95rem;
        }

        .contact-item i {
            color: var(--secondary);
            width: 20px;
        }

        /* Navigation */
        nav {
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            margin-bottom: 30px;
        }

        .nav-links {
            display: flex;
            list-style: none;
            justify-content: center;
            flex-wrap: wrap;
            padding: 15px;
        }

        .nav-links li {
            margin: 0 15px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: var(--transition);
            padding: 8px 15px;
            border-radius: 5px;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--secondary);
            background: var(--light);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            width: 0;
            height: 2px;
            background: var(--secondary);
            transition: var(--transition);
            transform: translateX(-50%);
        }

        .nav-links a:hover::after {
            width: 80%;
        }

        /* Main Content Styles */
        .main-content {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }

        .section {
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            padding: 35px;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: var(--secondary);
        }

        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.12);
        }

        .section-title {
            font-size: 1.6rem;
            margin-bottom: 25px;
            color: var(--primary);
            position: relative;
            padding-bottom: 12px;
            display: flex;
            align-items: center;
        }

        .section-title i {
            margin-right: 12px;
            color: var(--secondary);
            background: var(--light);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 60px;
            height: 3px;
            background: var(--secondary);
        }

        .about-text {
            font-size: 1.08rem;
            line-height: 1.8;
            margin-bottom: 20px;
        }

        .motto {
            background: #e3f2fd;
            padding: 20px;
            border-radius: var(--border-radius);
            font-style: italic;
            margin: 25px 0;
            border-left: 4px solid var(--secondary);
            font-size: 1.15rem;
            position: relative;
        }

        .motto::before {
            content: '"';
            font-size: 4rem;
            position: absolute;
            top: -10px;
            left: 10px;
            color: var(--secondary);
            opacity: 0.2;
            font-family: serif;
        }

        /* Timeline */
        .timeline {
            position: relative;
            padding-left: 30px;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            bottom: 0;
            width: 2px;
            background: var(--secondary);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 30px;
            padding-left: 30px;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -36px;
            top: 5px;
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background: var(--secondary);
            border: 3px solid white;
            box-shadow: 0 0 0 3px var(--secondary);
            z-index: 1;
        }

        .item-title {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 5px;
            color: var(--primary);
        }

        .item-date {
            display: inline-block;
            background: var(--light);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            margin-bottom: 12px;
            color: var(--text-light);
            font-weight: 500;
        }

        .item-details {
            color: var(--text-light);
            line-height: 1.7;
        }

        /* Hobbies */
        .hobbies-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 25px;
            margin-top: 20px;
        }

        .hobby-item {
            background: #f8f9fa;
            border-radius: var(--border-radius);
            padding: 25px;
            text-align: center;
            transition: var(--transition);
            border-top: 4px solid var(--secondary);
            position: relative;
            overflow: hidden;
        }

        .hobby-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, var(--secondary) 0%, transparent 100%);
            opacity: 0;
            transition: var(--transition);
        }

        .hobby-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .hobby-item:hover::before {
            opacity: 0.05;
        }

        .hobby-icon {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 15px;
            position: relative;
            z-index: 1;
        }

        .hobby-name {
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 10px;
            position: relative;
            z-index: 1;
        }

        /* Download Button */
        .download-section {
            text-align: center;
            padding: 40px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            border-radius: var(--border-radius);
            margin: 40px 0 30px;
            position: relative;
            overflow: hidden;
        }

        .download-section::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            transform: rotate(30deg);
        }

        .download-btn {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: white;
            color: var(--primary);
            padding: 14px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            margin-top: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            position: relative;
            z-index: 1;
        }

        .download-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
        }

        /* Footer */
        footer {
            background: var(--primary);
            color: white;
            padding: 40px;
            border-radius: var(--border-radius);
            text-align: center;
            margin-top: 30px;
            position: relative;
            overflow: hidden;
        }

        footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 5px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 25px 0;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            transition: var(--transition);
            font-size: 1.2rem;
        }

        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-3px) scale(1.1);
        }

        .copyright {
            margin-top: 25px;
            opacity: 0.7;
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .profile-header {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-text {
                text-align: center;
            }
            
            .profile-img-container {
                width: 180px;
                height: 220px;
            }
            
            .name {
                font-size: 2rem;
            }
            
            .contact-info {
                justify-content: center;
            }
            
            .nav-links {
                flex-direction: column;
                align-items: center;
                gap: 10px;
            }
            
            .section {
                padding: 25px;
            }
            
            .hobbies-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header with Photo -->
        <header>
            <div class="profile-header">
                <div class="profile-img-container">
                    <img src="https://uploads.onecompiler.io/435eqnbkv/43xpqtzzh/My%20Picture%20in%20HTML.jpg" alt="Sereyvattanak Suon" class="profile-img">
                </div>
                <div class="profile-text">
                    <h1 class="name">Sereyvattanak Suon</h1>
                    <p class="title">Master's Candidate in Applied Mathematics</p>
                    <div class="contact-info">
                        <div class="contact-item">
                            <i class="fas fa-envelope"></i>
                            <span>vattanakvn1@gmail.com</span>
                        </div>
                        <div class="contact-item">
                            <i class="fas fa-phone"></i>
                            <span>+91 8987584023 </span>
                        </div>
                        <div class="contact-item">
                            <i class="fas fa-map-marker-alt"></i>
                            <span>Country: Phnom Penh, Cambodia</span>
                            <i class="fas fa-map-marker-alt"></i>
                            <span>Currently : Dhanbad , India</span>
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <!-- Navigation -->
        <nav>
            <ul class="nav-links">
                <li><a href="#about">About Me</a></li>
                <li><a href="#education">Education</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#hobbies">Interests</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>

        <!-- Main Content -->
        <main class="main-content">
            <!-- About Section -->
            <section id="about" class="section">
                <h2 class="section-title"><i class="fas fa-user"></i> About Me</h2>
                <p class="about-text">
                    I am a passionate learner from Cambodia with a relentless drive to study hard, explore the unknown, and push boundaries. My strong interest lies in Deep Learning and Natural Language Processing 
                </p>
                
                <div class="motto">
                    Never give up, keep moving forward, and stay strong. Life is about embracing hard work, overcoming obstacles, and never surrendering to difficulties.
                </div>
                
                <p class="about-text">
                    I am eager to contribute to cutting-edge research and develop solutions that can solve real-world problems. I thrive on curiosity, creativity, and the pursuit of knowledge that transforms ideas into reality.
                </p>
                
                <div class="motto">
                    Cristiano Ronaldo - My Inspiration: I admire him not only for his incredible talent but also for his consistency, discipline, and dedication. I apply these qualities to my studies and personal development.
                </div>
            </section>
            
            <!-- Education Section -->
            <section id="education" class="section">
                <h2 class="section-title"><i class="fas fa-graduation-cap"></i> Education</h2>
                <div class="timeline">
                    <div class="timeline-item">
                        <div class="item-title">Indian Institute of Technology (ISM) Dhanbad</div>
                        <span class="item-date">2024 - Present</span>
                        <div class="item-details">
                            Master's degree in Applied Mathematics<br>
                            Thesis: Deep Learning (ongoing)
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-title">Royal University of Phnom Penh</div>
                        <span class="item-date">2020 - 2024</span>
                        <div class="item-details">
                            Bachelor's degree in Pure Mathematics<br>
                            Project: <i>Matrix Exponentials and System of Differential Equations</i>
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-title">Mathematical Association of Cambodia</div>
                        <span class="item-date">2023 - Present</span>
                        <div class="item-details">
                            Advanced courses: Introduction to Statistical Learning, Machine Learning
                        </div>
                    </div>
                </div>
            </section>
            
            <!-- Experience Section -->
            <section id="experience" class="section">
                <h2 class="section-title"><i class="fas fa-briefcase"></i> Experience & Achievements</h2>
                <div class="timeline">
                    <div class="timeline-item">
                        <div class="item-title">Master's Candidate in Mathematics and Computing </div>
                        <span class="item-date">2024-Present</span>
                        <div class="item-details">
                            Focus on mathematics and Computer science
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-title">Awarded ICCR Master's Program Scholarship</div>
                        <span class="item-date">2024</span>
                        <div class="item-details">
                            Full scholarship to study in India
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-title">Public speaking at Mathematical Association of Cambodia </div>
                        <span class="item-date">August 2024</span>
                        <div class="item-details">
                            Gave a talk on Operators on Inner Product Spaces
                        </div>
                    </div>
                    <div class="timeline-item">
                        <div class="item-title"> Seminar Presenting on Inverse Problems </div>
                        <span class="item-date">July 2025</span>
                        <div class="item-details">
                            Given at Los Baños, Philippines
                        </div>
                    </div>
              
                <div class="timeline-item">
                        <div class="item-title">Public speaking at Mathematical Association of Cambodia </div>
                        <span class="item-date">(Upcoming) October 2025 </span>
                        <div class="item-details">
                            Introduction to Natural Language Processing
                        </div>
                    </div>
                </div>
            </section>
            
            <!-- Projects Section -->
            <section id="projects" class="section">
                <h2 class="section-title"><i class="fas fa-project-diagram"></i> Projects & Research</h2>
                <div class="timeline">
                    <div class="timeline-item">
                        <div class="item-title">Machine Learning Studies</div>
                        <span class="item-date">2023</span>
                        <div class="item-details">
                            Studied under Dr. Vanny Khon and Dr. Has Sothea in the Forum Pushing the Boundary
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <div class="item-title">Academic Project</div>
                        <span class="item-date">2023</span>
                        <div class="item-details">
                            Worked on a project under Assoc. Prof. Dr. Meas Len
                        </div>
                    </div>    
                    <div class="timeline-item">
                        <div class="item-title">Lightweight Text-Based Emotion Recognition
 Using Transformer Embeddings</div>
                        <span class="item-date">2025</span>
                        <div class="item-details">
                            Review by Dr. Vanny Khon
                        </div>
                        </div>
                        
        
            
            <!-- Hobbies Section -->
            <section id="hobbies" class="section">
                <h2 class="section-title"><i class="fas fa-heart"></i> Interests</h2>
                <div class="hobbies-container">
                    <div class="hobby-item">
                        <div class="hobby-icon">
                            <i class="fas fa-futbol"></i>
                        </div>
                        <div class="hobby-name">Football</div>
                        <div class="item-details"> Winger inspired by Cristiano Ronaldo's work ethic</div>
                    </div>
                    
                    <div class="hobby-item">
                        <div class="hobby-icon">
                            <i class="fas fa-guitar"></i>
                        </div>
                        <div class="hobby-name">Guitar</div>
                        <div class="item-details">Acoustic and electric </div>
                    </div>
                    
                    <div class="hobby-item">
                        <div class="hobby-icon">
                            <i class="fas fa-fist-raised"></i>
                        </div>
                        <div class="hobby-name">Boxing</div>
                        <div class="item-details">Training for fitness and mental discipline inspired by Bruce Lee </div>
                    </div>
                </div>
            </section>

            
        
        <!-- Footer -->
        <footer id="contact">
            <h2>Let's Connect</h2>
            <p> "Never stop learning, because life never stops teaching </p>
            
            <div class="social-links">
                <a href="#"><i class="fab fa-linkedin-in"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fas fa-envelope"></i></a>
            </div>
            
            <div class="copyright">
                &copy; 2025 Sereyvattanak Suon. All Rights Reserved.
            </div>
        </footer>
    </div>

    <script>
        // Simple animation on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const sections = document.querySelectorAll('.section');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            sections.forEach(section => {
                section.style.opacity = 0;
                section.style.transform = 'translateY(20px)';
                section.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(section);
            });
            
            // Smooth scrolling for navigation links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    if(targetId === '#') return;
                    
                    const targetElement = document.querySelector(targetId);
                    if(targetElement) {
                        window.scrollTo({
                            top: targetElement.offsetTop - 100,
                            behavior: 'smooth'
                        });
                    }
                });
            });
        });
    </script>
