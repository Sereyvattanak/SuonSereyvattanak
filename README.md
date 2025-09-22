<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sereyvattanak Suon - Academic CV</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #e0f7fa 0%, #bbdefb 100%);
            color: #333;
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }
        
        .cv-container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
            border-radius: 12px;
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #1a237e 0%, #283593 50%, #3949ab 100%);
            color: white;
            padding: 40px 30px;
            text-align: center;
            position: relative;
        }
        
        .header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #ff5252, #ff4081, #e040fb);
        }
        
        .header h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
            font-weight: 700;
        }
        
        .header p {
            font-size: 1.3rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
            padding: 35px;
        }
        
        .main-content {
            grid-column: 1 / -1;
        }
        
        .profile-section {
            background: #f8f9fa;
            border-radius: 10px;
            padding: 25px;
            margin-bottom: 30px;
            border-left: 5px solid #3949ab;
        }
        
        .profile-text {
            font-size: 1.05rem;
            line-height: 1.8;
            color: #444;
            margin-bottom: 15px;
        }
        
        .motto {
            background: #e3f2fd;
            padding: 15px;
            border-radius: 8px;
            font-style: italic;
            text-align: center;
            margin: 20px 0;
            border-left: 4px solid #2196f3;
        }
        
        .section {
            margin-bottom: 35px;
        }
        
        .section-title {
            color: #1a237e;
            border-bottom: 2px solid #3949ab;
            padding-bottom: 12px;
            margin-bottom: 20px;
            font-size: 1.6rem;
            display: flex;
            align-items: center;
        }
        
        .section-title i {
            margin-right: 12px;
            color: #3949ab;
            background: #e8eaf6;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .timeline-item {
            margin-bottom: 22px;
            position: relative;
            padding-left: 35px;
        }
        
        .timeline-item:before {
            content: '';
            position: absolute;
            left: 0;
            top: 8px;
            width: 14px;
            height: 14px;
            border: 3px solid #3949ab;
            border-radius: 50%;
            background: white;
            z-index: 2;
        }
        
        .timeline-item:after {
            content: '';
            position: absolute;
            left: 6px;
            top: 24px;
            width: 2px;
            height: calc(100% + 14px);
            background: #3949ab;
        }
        
        .timeline-item:last-child:after {
            display: none;
        }
        
        .item-title {
            font-weight: 700;
            color: #1a237e;
            margin-bottom: 6px;
            font-size: 1.1rem;
        }
        
        .item-date {
            color: #666;
            font-style: italic;
            margin-bottom: 10px;
            display: block;
            background: #f5f5f5;
            padding: 3px 10px;
            border-radius: 12px;
            display: inline-block;
        }
        
        .item-details {
            color: #555;
            margin-top: 8px;
            font-size: 0.98rem;
        }
        
        .two-column {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
        }
        
        .tag {
            display: inline-block;
            background: #e8eaf6;
            color: #3949ab;
            padding: 4px 12px;
            border-radius: 15px;
            font-size: 0.9rem;
            margin: 4px 6px 4px 0;
            font-weight: 500;
        }
        
        .hobbies-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .hobby-item {
            flex: 1;
            min-width: 200px;
            background: #f8f9fa;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s, box-shadow 0.3s;
            border-top: 4px solid #3949ab;
        }
        
        .hobby-item:hover {
            transform: translateY(-7px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.12);
        }
        
        .hobby-icon {
            font-size: 2.8rem;
            margin-bottom: 15px;
            color: #3949ab;
        }
        
        .hobby-name {
            font-weight: 700;
            color: #1a237e;
            margin-bottom: 8px;
            font-size: 1.2rem;
        }
        
        .hobby-desc {
            color: #666;
            font-size: 0.95rem;
            line-height: 1.5;
        }
        
        .idol-section {
            background: linear-gradient(135deg, #f5f5f5 0%, #e0e0e0 100%);
            border-radius: 10px;
            padding: 20px;
            margin: 25px 0;
            display: flex;
            align-items: center;
            gap: 20px;
            border-left: 5px solid #ff5252;
        }
        
        .idol-image {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            background: #3949ab;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2rem;
            flex-shrink: 0;
        }
        
        .idol-text {
            flex: 1;
        }
        
        .idol-name {
            font-weight: 700;
            color: #d32f2f;
            margin-bottom: 8px;
        }
        
        @media (max-width: 768px) {
            .content {
                grid-template-columns: 1fr;
                padding: 20px;
            }
            
            .two-column {
                grid-template-columns: 1fr;
            }
            
            .hobby-item {
                min-width: 100%;
            }
            
            .idol-section {
                flex-direction: column;
                text-align: center;
            }
            
            .header h1 {
                font-size: 2.2rem;
            }
        }
        
        .print-btn {
            display: block;
            margin: 25px auto;
            padding: 14px 30px;
            background: #3949ab;
            color: white;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            font-size: 1.1rem;
            transition: background 0.3s, transform 0.3s;
            box-shadow: 0 4px 8px rgba(57, 73, 171, 0.3);
        }
        
        .print-btn:hover {
            background: #283593;
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(57, 73, 171, 0.4);
        }
        
        .signature {
            text-align: right;
            margin-top: 30px;
            font-style: italic;
            color: #666;
            padding: 10px;
            border-top: 1px dashed #ccc;
        }
        
        .footer {
            text-align: center;
            padding: 20px;
            background: #1a237e;
            color: white;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>
    <div class="cv-container">
        <div class="header">
            <h1>Sereyvattanak Suon</h1>
            <p>Master's Candidate in Applied Mathematics </p>
        </div>
        
        <div class="content">
            <div class="main-content">
                <div class="profile-section">
                    <h2 class="section-title"><i class="fas fa-user"></i> Personal Profile</h2>
                    <p class="profile-text">
                        I am a young dreamer from Cambodia with a relentless drive to study hard, explore the impossible, and push boundaries. 
                        I am passionate about learning, innovating, and tackling challenges that others may consider too difficult.
                    </p>
                    
                    <div class="motto">
                        "Never give up, keep moving forward, and stay strong. Life is about embracing hard work, overcoming obstacles, and never surrendering to difficulties."
                    </div>
                    
                    <p class="profile-text">
                        My primary field of interest lies in Machine Learning and Deep Learning, where I am eager to contribute to cutting-edge research 
                        and develop solutions that can make a meaningful impact. I thrive on curiosity, creativity, and the pursuit of knowledge that transforms ideas into reality.
                    </p>
                    
                    <div class="idol-section">
                        <div class="idol-image">
                            <i class="fas fa-futbol"></i>
                        </div>
                        <div class="idol-text">
                            <div class="idol-name">Cristiano Ronaldo - My Inspiration</div>
                            <p>I admire him not only for his incredible talent on the field but also for his consistency, discipline, and dedication. 
                            I try to emulate these qualities in my own life—applying the same focus, hard work, and perseverance to my studies and research.</p>
                        </div>
                    </div>
                </div>
                
                <div class="section">
                    <h2 class="section-title"><i class="fas fa-graduation-cap"></i> Education</h2>
                    
                    <div class="timeline-item">
                        <span class="item-title">Indian Institute of Technology (ISM) Dhanbad</span>
                        <span class="item-date">2024 - Present</span>
                        <div class="item-details">
                            Master's degree in Applied Mathematics<br>
                            Thesis: Deep Learning (ongoing)
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Royal University of Phnom Penh</span>
                        <span class="item-date">2020 - 2024</span>
                        <div class="item-details">
                            Bachelor's degree in Pure Mathematics<br>
                            Project: <i>Matrix Exponentials and System of Differential Equations</i>
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Mathematical Association of Cambodia</span>
                        <span class="item-date">2023 - Present</span>
                        <div class="item-details">
                            Basic: Linear Algebra, Abstract Algebra, Real Analysis<br>
                            Advanced: Introduction to Statistical Learning, Machine Learning
                        </div>
                    </div>
                </div>
                
                <div class="section">
                    <h2 class="section-title"><i class="fas fa-briefcase"></i> Activities & Achievements</h2>
                    
                    <div class="timeline-item">
                        <span class="item-title">Master's degree Candidate in Applied Mathematics</span>
                        <span class="item-date">2024-Present</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Entrance the Examination at IIT(ISM) Dhanbad</span>
                        <span class="item-date">2024</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Awarded ICCR Master's Program full scholarship to study in India</span>
                        <span class="item-date">2024</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Gave a public talk on Operators on Inner Product Spaces in MAC</span>
                        <span class="item-date">August 2024</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Entrance Exam by the Mathematical Association of Cambodia</span>
                        <span class="item-date">2023</span>
                    </div>
                </div>
                
                <div class="section">
                    <h2 class="section-title"><i class="fas fa-chalkboard-teacher"></i> Conferences & Workshops</h2>
                    
                    <div class="timeline-item">
                        <span class="item-title">SEAMS School 2025</span>
                        <span class="item-date">July 14-22, 2025</span>
                        <div class="item-details">
                            School on Theoretical and Computational Tools for the Data-Enabled Sciences<br>
                            University of the Philippines Los Baños, Laguna, Philippines
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Workshop in Artificial Intelligence with Machine Learning</span>
                        <span class="item-date">March 2025</span>
                        <div class="item-details">
                            IIT Patna
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Seminar on Quantum Boltzmann Machines by Prof. Mark M. Wilde</span>
                        <span class="item-date">January 10, 2025</span>
                        <div class="item-details">
                            Cornell University, IIT(ISM) Dhanbad
                        </div>
                    </div>
                </div>
                
                <div class="section">
                    <h2 class="section-title"><i class="fas fa-project-diagram"></i> Projects & Research</h2>
                    
                    <div class="timeline-item">
                        <span class="item-title">Studied Machine Learning and Statistical learning</span>
                        <span class="item-date">2023</span>
                        <div class="item-details">
                            Under Dr. Vanny Khon and Dr. Has Sothea in the Forum Pushing the Boundary
                        </div>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Worked on a project under Assoc. Prof. Dr. Meas Len</span>
                        <span class="item-date">2023</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Given a Seminar talk on Inverse Problems</span>
                        <span class="item-date">July 22, 2025</span>
                        <div class="item-details">
                            Los Baños, Philippines
                        </div>
                    </div>
                </div>
                
                <div class="section">
                    <h2 class="section-title"><i class="fas fa-heart"></i> Hobbies & Interests</h2>
                    
                    <div class="hobbies-container">
                        <div class="hobby-item">
                            <div class="hobby-icon">
                                <i class="fas fa-futbol"></i>
                            </div>
                            <div class="hobby-name">Football</div>
                            <div class="hobby-desc">Enjoy playing as a midfielder, team sports enthusiast. Inspired by Cristiano Ronaldo's work ethic and dedication.</div>
                        </div>
                        
                        <div class="hobby-item">
                            <div class="hobby-icon">
                                <i class="fas fa-guitar"></i>
                            </div>
                            <div class="hobby-name">Guitar</div>
                            <div class="hobby-desc">Playing acoustic and electric guitar, enjoy classic rock and traditional Cambodian music.</div>
                        </div>
                        
                        <div class="hobby-item">
                            <div class="hobby-icon">
                                <i class="fas fa-fist-raised"></i>
                            </div>
                            <div class="hobby-name">Boxing</div>
                            <div class="hobby-desc">Training for fitness, discipline, and mental toughness. Amateur level with focus on technique.</div>
                        </div>
                    </div>
                </div>
                
                <div class="signature">
                    Sereyvattanak Suon<br>
                    <span style="font-size: 0.9em;">"Never stop learning, because life never stops teaching"</span>
                </div>
            </div>
        </div>
        
        <div class="footer">
            &copy; 2025 Sereyvattanak Suon | Email: vattanakvn1@gmail.com 
        </div>
    </div>
    
    <button class="print-btn" onclick="window.print()">
        <i class="fas fa-print"></i> Print CV
    </button>

    <script>
        // Add current year to future events if needed
        document.addEventListener('DOMContentLoaded', function() {
            const currentYear = new Date().getFullYear();
            document.querySelectorAll('.item-date').forEach(el => {
                if (el.textContent.includes('2025') && currentYear < 2025) {
                    el.innerHTML = el.innerHTML.replace('2025', '2025 (Upcoming)');
                }
            });
        });
    </script>
</body>
</html>
