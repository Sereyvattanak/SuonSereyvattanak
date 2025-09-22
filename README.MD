<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Academic CV</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7f9;
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }
        
        .cv-container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #2c3e50, #1a2530);
            color: white;
            padding: 30px;
            text-align: center;
        }
        
        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            padding: 30px;
        }
        
        .main-content {
            grid-column: 1 / -1;
        }
        
        .section {
            margin-bottom: 30px;
        }
        
        .section-title {
            color: #2c3e50;
            border-bottom: 2px solid #3498db;
            padding-bottom: 10px;
            margin-bottom: 15px;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
        }
        
        .section-title i {
            margin-right: 10px;
            color: #3498db;
        }
        
        .timeline-item {
            margin-bottom: 20px;
            position: relative;
            padding-left: 30px;
        }
        
        .timeline-item:before {
            content: '';
            position: absolute;
            left: 0;
            top: 8px;
            width: 12px;
            height: 12px;
            border: 2px solid #3498db;
            border-radius: 50%;
            background: white;
        }
        
        .timeline-item:after {
            content: '';
            position: absolute;
            left: 5px;
            top: 22px;
            width: 2px;
            height: calc(100% + 10px);
            background: #3498db;
        }
        
        .timeline-item:last-child:after {
            display: none;
        }
        
        .item-title {
            font-weight: 600;
            color: #2c3e50;
            margin-bottom: 5px;
        }
        
        .item-date {
            color: #7f8c8d;
            font-style: italic;
            margin-bottom: 8px;
            display: block;
        }
        
        .item-details {
            color: #555;
            margin-top: 5px;
            font-size: 0.95rem;
        }
        
        .two-column {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }
        
        .tag {
            display: inline-block;
            background: #e8f4fc;
            color: #3498db;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 0.85rem;
            margin: 3px 5px 3px 0;
        }
        
        .hobbies-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 15px;
        }
        
        .hobby-item {
            flex: 1;
            min-width: 200px;
            background: #f8f9fa;
            border-radius: 8px;
            padding: 15px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s;
        }
        
        .hobby-item:hover {
            transform: translateY(-5px);
        }
        
        .hobby-icon {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: #3498db;
        }
        
        .hobby-name {
            font-weight: 600;
            color: #2c3e50;
            margin-bottom: 5px;
        }
        
        .hobby-desc {
            color: #7f8c8d;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .content {
                grid-template-columns: 1fr;
            }
            
            .two-column {
                grid-template-columns: 1fr;
            }
            
            .hobby-item {
                min-width: 100%;
            }
        }
        
        .print-btn {
            display: block;
            margin: 20px auto;
            padding: 12px 25px;
            background: #3498db;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1rem;
            transition: background 0.3s;
        }
        
        .print-btn:hover {
            background: #2980b9;
        }
    </style>
</head>
<body>
    <div class="cv-container">
        <div class="header">
            <h1>Academic Curriculum Vitae</h1>
            <p>Master's Candidate in Applied Mathematics</p>
        </div>
        
        <div class="content">
            <div class="main-content">
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
                        <span class="item-title">Entered the Royal University of Phnom Penh</span>
                        <span class="item-date">2020</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Entrance Exam by the Mathematical Association of Cambodia</span>
                        <span class="item-date">2023</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Awarded ICCR Master's Program full scholarship to study in India</span>
                        <span class="item-date">2024</span>
                    </div>
                    
                    <div class="timeline-item">
                        <span class="item-title">Gave a public talk on Operators on Inner Product Spaces in MAC</span>
                        <span class="item-date">August 2024</span>
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
                    
                    <div class="timeline-item">
                        <span class="item-title">Webinar on Möbius Function by Prof. Krishnaswami Alladi</span>
                        <span class="item-date">August 15, 2024</span>
                        <div class="item-details">
                            University of Florida
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
                            <div class="hobby-desc">Enjoy playing as a midfielder, team sports enthusiast</div>
                        </div>
                        
                        <div class="hobby-item">
                            <div class="hobby-icon">
                                <i class="fas fa-guitar"></i>
                            </div>
                            <div class="hobby-name">Guitar</div>
                            <div class="hobby-desc">Playing acoustic and electric guitar, enjoy classic rock</div>
                        </div>
                        
                        <div class="hobby-item">
                            <div class="hobby-icon">
                                <i class="fas fa-fist-raised"></i>
                            </div>
                            <div class="hobby-name">Boxing</div>
                            <div class="hobby-desc">Training for fitness and discipline, amateur level</div>
                        </div>
                    </div>
                </div>
            </div>
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
