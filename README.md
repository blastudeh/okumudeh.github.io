<!DOCTYPE html> 
<html lang="en"> 
<head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Okum Udeh | System Administrator & Cybersecurity Specialist</title> 
    <link rel="stylesheet" 
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"> 
    <style> 
        /* Base Styles */ 
        * { 
            margin: 0; 
            padding: 0; 
            box-sizing: border-box; 
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
        } 
 
        :root { 
            --primary: #2c3e50; 
            --secondary: #3498db; 
            --accent: #e74c3c; 
            --light: #ecf0f1; 
            --dark: #2c3e50; 
            --gray: #7f8c8d; 
        } 
 
        body { 
            line-height: 1.6; 
            color: #333; 
            background-color: #f9f9f9; 
        } 
 
        .container { 
            width: 90%; 
            max-width: 1200px; 
            margin: 0 auto; 
            padding: 0 20px; 
        } 
 
        section { 
            padding: 80px 0; 
        } 
 
        h1, h2, h3, h4 { 
            margin-bottom: 20px; 
            color: var(--dark); 
        } 
 
        h1 { 
            font-size: 2.8rem; 
            line-height: 1.2; 
        } 
 
        h2 { 
            font-size: 2.2rem; 
            text-align: center; 
            margin-bottom: 50px; 
            position: relative; 
        } 
 
        h2:after { 
            content: ''; 
            position: absolute; 
            width: 80px; 
            height: 4px; 
            background: var(--secondary); 
            bottom: -15px; 
            left: 50%; 
            transform: translateX(-50%); 
        } 
 
        h3 { 
            font-size: 1.5rem; 
            color: var(--primary); 
        } 
 
        p { 
            margin-bottom: 15px; 
            font-size: 1.1rem; 
        } 
 
        a { 
            text-decoration: none; 
            color: var(--secondary); 
            transition: color 0.3s; 
        } 
 
        a:hover { 
            color: var(--accent); 
        } 
 
        .btn { 
            display: inline-block; 
            padding: 12px 30px; 
            background: var(--secondary); 
            color: white; 
            border-radius: 5px; 
            font-weight: 600; 
            border: none; 
            cursor: pointer; 
            transition: all 0.3s; 
            text-transform: uppercase; 
            letter-spacing: 1px; 
            font-size: 0.9rem; 
        } 
 
        .btn:hover { 
            background: var(--primary); 
            transform: translateY(-3px); 
            box-shadow: 0 5px 15px rgba(0,0,0,0.1); 
        } 
 
        .btn-secondary { 
            background: transparent; 
            border: 2px solid var(--secondary); 
            color: var(--secondary); 
        } 
 
        .btn-secondary:hover { 
            background: var(--secondary); 
            color: white; 
        } 
 
        /* Header & Navigation */ 
        header { 
            background: white; 
            box-shadow: 0 2px 10px rgba(0,0,0,0.1); 
            position: fixed; 
            width: 100%; 
            top: 0; 
            z-index: 1000; 
        } 
 
        .header-container { 
            display: flex; 
            justify-content: space-between; 
            align-items: center; 
            padding: 20px 0; 
        } 
 
        .logo { 
            font-size: 1.8rem; 
            font-weight: 700; 
            color: var(--primary); 
        } 
 
        .logo span { 
            color: var(--secondary); 
        } 
 
        nav ul { 
            display: flex; 
            list-style: none; 
        } 
 
        nav ul li { 
            margin-left: 30px; 
        } 
 
        nav ul li a { 
            color: var(--dark); 
            font-weight: 600; 
            font-size: 1rem; 
        } 
 
        nav ul li a:hover { 
            color: var(--secondary); 
        } 
 
        .menu-toggle { 
            display: none; 
            font-size: 1.5rem; 
            cursor: pointer; 
        } 
 
        /* Hero Section */ 
        .hero { 
            background: linear-gradient(135deg, var(--primary) 0%, #1a2530 100%); 
            color: white; 
            padding: 180px 0 100px; 
            text-align: center; 
        } 
 
        .hero h1 { 
            color: white; 
            margin-bottom: 20px; 
        } 
 
        .hero p { 
            font-size: 1.3rem; 
            max-width: 700px; 
            margin: 0 auto 40px; 
            color: var(--light); 
        } 
 
        .hero-btns { 
            margin-top: 30px; 
        } 
 
        .hero-btns .btn { 
            margin: 0 10px; 
        } 
 
        .hero-btns .btn-secondary { 
            color: white; 
            border-color: white; 
        } 
 
        /* About Section */ 
        .about-content { 
            display: flex; 
            align-items: center; 
            gap: 50px; 
        } 
 
        .about-img { 
            flex: 1; 
            text-align: center; 
        } 
 
        .profile-img { 
            width: 300px; 
            height: 300px; 
            border-radius: 50%; 
            object-fit: cover; 
            border: 5px solid var(--light); 
            box-shadow: 0 10px 30px rgba(0,0,0,0.1); 
        } 
 
        .about-text { 
            flex: 2; 
        } 
 
        .about-details { 
            display: flex; 
            margin-top: 30px; 
            flex-wrap: wrap; 
        } 
 
        .detail-item { 
            flex: 1; 
            min-width: 200px; 
            margin-bottom: 20px; 
        } 
 
        .detail-item i { 
            color: var(--secondary); 
            margin-right: 10px; 
        } 
 
        /* Portfolio Section */ 
        .portfolio-items { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr)); 
            gap: 30px; 
        } 
 
        .portfolio-item { 
            background: white; 
            border-radius: 10px; 
            overflow: hidden; 
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); 
            transition: transform 0.3s; 
        } 
 
        .portfolio-item:hover { 
            transform: translateY(-10px); 
        } 
 
        .portfolio-img { 
            height: 200px; 
            background: var(--light); 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            color: var(--secondary); 
            font-size: 3rem; 
        } 
 
        .portfolio-content { 
            padding: 25px; 
        } 
 
        .portfolio-content h3 { 
            margin-bottom: 10px; 
        } 
 
        .portfolio-tags { 
            display: flex; 
            flex-wrap: wrap; 
            margin: 15px 0; 
        } 
 
        .tag { 
            background: var(--light); 
            padding: 5px 10px; 
            border-radius: 20px; 
            font-size: 0.8rem; 
            margin-right: 8px; 
            margin-bottom: 8px; 
        } 
 
        /* Skills Section */ 
        .skills-container { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); 
            gap: 30px; 
        } 
 
        .skill-category { 
            background: white; 
            padding: 30px; 
            border-radius: 10px; 
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); 
        } 
 
        .skill-list { 
            margin-top: 20px; 
        } 
 
        .skill-item { 
            margin-bottom: 15px; 
        } 
 
        .skill-name { 
            display: flex; 
            justify-content: space-between; 
            margin-bottom: 5px; 
        } 
 
        .skill-bar { 
            height: 8px; 
            background: var(--light); 
            border-radius: 4px; 
            overflow: hidden; 
        } 
 
        .skill-level { 
            height: 100%; 
            background: var(--secondary); 
        } 
 
        /* Blog Section */ 
        .blog-posts { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr)); 
            gap: 30px; 
        } 
 
        .blog-post { 
            background: white; 
            border-radius: 10px; 
            overflow: hidden; 
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); 
        } 
 
        .blog-img { 
            height: 200px; 
            background: linear-gradient(135deg, #2c3e50 0%, #3498db 100%); 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            color: white; 
            font-size: 3rem; 
        } 
 
        .blog-content { 
            padding: 25px; 
        } 
 
        .blog-meta { 
            display: flex; 
            justify-content: space-between; 
            color: #7f8c8d; 
            font-size: 0.9rem; 
            margin-bottom: 15px; 
        } 
 
        .blog-tags { 
            display: flex; 
            flex-wrap: wrap; 
            margin: 15px 0; 
        } 
 
        /* Certifications Section */ 
        .cert-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
            gap: 30px; 
            margin-top: 40px; 
        } 
 
        .cert-card { 
            background: white; 
            padding: 30px; 
            border-radius: 10px; 
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); 
        } 
 
        /* Services Section */ 
        .services-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); 
            gap: 30px; 
            margin-top: 40px; 
        } 
 
        .service-card { 
            background: white; 
            padding: 30px; 
            border-radius: 10px; 
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); 
            text-align: center; 
            transition: transform 0.3s; 
        } 
 
        .service-card:hover { 
            transform: translateY(-10px); 
        } 
 
        .service-icon { 
            width: 70px; 
            height: 70px; 
            background: var(--secondary); 
            color: white; 
            border-radius: 50%; 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            margin: 0 auto 20px; 
            font-size: 1.8rem; 
        } 
 
        /* Contact Section */ 
        .contact-container { 
            display: flex; 
            gap: 50px; 
        } 
 
        .contact-info { 
            flex: 1; 
        } 
 
        .contact-item { 
            display: flex; 
            align-items: center; 
            margin-bottom: 25px; 
        } 
 
        .contact-icon { 
            width: 50px; 
            height: 50px; 
            background: var(--secondary); 
            color: white; 
            border-radius: 50%; 
            display: flex; 
            align-items: center; 
            justify-content: center; 
            margin-right: 15px; 
            font-size: 1.2rem; 
        } 
 
        .contact-form { 
            flex: 2; 
            background: white; 
            padding: 30px; 
            border-radius: 10px; 
            box-shadow: 0 5px 15px rgba(0,0,0,0.05); 
        } 
 
        .form-group { 
            margin-bottom: 20px; 
        } 
 
        .form-group label { 
            display: block; 
            margin-bottom: 8px; 
            font-weight: 600; 
        } 
 
        .form-group input, 
        .form-group textarea { 
            width: 100%; 
            padding: 12px; 
            border: 1px solid #ddd; 
            border-radius: 5px; 
            font-size: 1rem; 
        } 
 
        .form-group textarea { 
            height: 150px; 
            resize: vertical; 
        } 
 
        /* Footer */ 
        footer { 
            background: var(--dark); 
            color: white; 
            padding: 50px 0 20px; 
        } 
 
        .footer-content { 
            display: flex; 
            justify-content: space-between; 
            align-items: center; 
            margin-bottom: 30px; 
        } 
 
        .social-links { 
            display: flex; 
            gap: 20px; 
        } 
 
        .social-links a { 
            color: white; 
            font-size: 1.2rem; 
            transition: color 0.3s; 
        } 
 
        .social-links a:hover { 
            color: var(--secondary); 
        } 
 
        .copyright { 
            text-align: center; 
            padding-top: 20px; 
            border-top: 1px solid rgba(255,255,255,0.1); 
            font-size: 0.9rem; 
            color: rgba(255,255,255,0.7); 
        } 
 
        /* Responsive Design */ 
        @media (max-width: 992px) { 
            .about-content { 
                flex-direction: column; 
            } 
             
            .contact-container { 
                flex-direction: column; 
            } 
        } 
 
        @media (max-width: 768px) { 
            .menu-toggle { 
                display: block; 
            } 
             
            nav ul { 
                position: fixed; 
                top: 80px; 
                left: -100%; 
                width: 100%; 
                flex-direction: column; 
                background: white; 
                text-align: center; 
                transition: 0.3s; 
                box-shadow: 0 10px 15px rgba(0,0,0,0.1); 
            } 
             
            nav ul.active { 
                left: 0; 
            } 
             
            nav ul li { 
                margin: 0; 
                padding: 15px 0; 
                border-bottom: 1px solid #eee; 
            } 
             
            h1 { 
                font-size: 2.2rem; 
            } 
             
            h2 { 
                font-size: 1.8rem; 
            } 
        } 
    </style> 
</head> 
<body> 
    <!-- Header & Navigation --> 
    <header> 
        <div class="container header-container"> 
            <div class="logo">Okum <span>Udeh</span></div> 
            <div class="menu-toggle" id="menuToggle"> 
                <i class="fas fa-bars"></i> 
            </div> 
            <nav> 
                <ul id="navMenu"> 
                    <li><a href="#home">Home</a></li> 
                    <li><a href="#about">About</a></li> 
                    <li><a href="#portfolio">Portfolio</a></li> 
                    <li><a href="#skills">Skills</a></li> 
                    <li><a href="#blog">Blog</a></li> 
                    <li><a href="#certifications">Certifications</a></li> 
                    <li><a href="#services">Services</a></li> 
                    <li><a href="#contact">Contact</a></li> 
                </ul> 
            </nav> 
        </div> 
    </header> 
 
    <!-- Hero Section --> 
    <section class="hero" id="home"> 
        <div class="container"> 
            <h1>System Administrator & Cybersecurity Specialist</h1> 
            <p>Bridging practical IT infrastructure experience with proven cybersecurity skills. I 
specialize in system administration, vulnerability assessment, and creating secure, efficient 
technology solutions.</p> 
            <div class="hero-btns"> 
                <a href="#portfolio" class="btn">View My Work</a> 
                <a href="#contact" class="btn btn-secondary">Contact Me</a> 
            </div> 
        </div> 
    </section> 
 
    <!-- About Section --> 
    <section id="about"> 
        <div class="container"> 
            <h2>About Me</h2> 
            <div class="about-content"> 
                <div class="about-img"> 
                    <!-- Replace with your actual photo --> 
                    <div class="profile-img" style="background: #3498db; color: white; display: flex; 
align-items: center; justify-content: center; font-size: 4rem;"> 
                        OU 
                    </div> 
                </div> 
                <div class="about-text"> 
                    <h3>Hello! I'm Okum Udeh</h3> 
                    <p>I'm a dedicated System Administrator with specialized training in 
cybersecurity. With experience spanning e-commerce logistics optimization at Mytheresa 
and Amazon to remote system administration for B2B platforms, I bring a unique perspective 
to IT infrastructure management.</p> 
                    <p>My recent focus has been on developing cybersecurity skills through 
hands-on vulnerability assessments and penetration testing, complementing my practical 
system administration background. I'm passionate about creating secure, efficient systems 
that support business objectives.</p> 
                     
                    <div class="about-details"> 
                        <div class="detail-item"> 
                            <p><i class="fas fa-map-marker-alt"></i> <strong>Location:</strong> 
Germany</p> 
                        </div> 
                        <div class="detail-item"> 
                            <p><i class="fas fa-language"></i> <strong>Languages:</strong> English, 
German (B1)</p> 
                        </div> 
                        <div class="detail-item"> 
                            <p><i class="fas fa-briefcase"></i> <strong>Status:</strong> Open to 
Opportunities</p> 
                        </div> 
                        <div class="detail-item"> 
                            <p><i class="fas fa-graduation-cap"></i> <strong>Education:</strong> 
B.Sc. Computer Science</p> 
                        </div> 
                    </div> 
                     
                    <a href="B2B cv.pdf" class="btn" download style="margin-top: 20px;"> 
                        <i class="fas fa-download"></i> Download CV 
                    </a> 
                </div> 
            </div> 
        </div> 
    </section> 
 
    <!-- Portfolio Section --> 
    <section id="portfolio"> 
        <div class="container"> 
            <h2>My Portfolio</h2> 
            <div class="portfolio-items"> 
                <!-- Project 1 --> 
                <div class="portfolio-item"> 
                    <div class="portfolio-img" style="background: #2c3e50;"> 
                        <i class="fas fa-shield-alt"></i> 
                    </div> 
                    <div class="portfolio-content"> 
                        <h3>Comprehensive Vulnerability Assessment</h3> 
                        <p>Full security assessment of Metasploitable 2 environment using Nmap 
and Metasploit Framework. Identified 28+ vulnerabilities across 20+ services with detailed 
remediation recommendations.</p> 
                        <div class="portfolio-tags"> 
                            <span class="tag">Cybersecurity</span> 
                            <span class="tag">Nmap</span> 
                            <span class="tag">Metasploit</span> 
                            <span class="tag">Penetration Testing</span> 
                        </div> 
                        <a href="metasploitable-case-study.html" class="btn">View Case Study</a> 
                    </div> 
                </div> 
                 
                <!-- Project 2 --> 
                <div class="portfolio-item"> 
                    <div class="portfolio-img" style="background: #3498db;"> 
                        <i class="fas fa-server"></i> 
                    </div> 
                    <div class="portfolio-content"> 
                        <h3>B2B E-commerce System Integration</h3> 
                        <p>ERP system integration for Tech Lab Marketers, improving product 
tracking, invoicing, and order management for B2B clients. Configured and maintained 
servers, networks, and helpdesk support systems.</p> 
                        <div class="portfolio-tags"> 
                            <span class="tag">System Administration</span> 
                            <span class="tag">ERP</span> 
                            <span class="tag">B2B</span> 
                            <span class="tag">Remote Support</span> 
                        </div> 
                        <a href="#" class="btn">Learn More</a> 
                    </div> 
                </div> 
                 
                <!-- Project 3 --> 
                <div class="portfolio-item"> 
                    <div class="portfolio-img" style="background: #e74c3c;"> 
                        <i class="fas fa-warehouse"></i> 
                    </div> 
                    <div class="portfolio-content"> 
                        <h3>Warehouse Management System Optimization</h3> 
                        <p>Optimized logistics processes and WMS/ERP integration at Mytheresa, 
overseeing daily operations including picking, packing, and international shipping 
coordination.</p> 
                        <div class="portfolio-tags"> 
                            <span class="tag">Logistics</span> 
                            <span class="tag">WMS</span> 
                            <span class="tag">Process Optimization</span> 
                            <span class="tag">E-commerce</span> 
                        </div> 
                        <a href="#" class="btn">Learn More</a> 
                    </div> 
                </div> 
            </div> 
        </div> 
    </section> 
 
    <!-- Skills Section --> 
    <section id="skills"> 
        <div class="container"> 
            <h2>Skills & Expertise</h2> 
            <div class="skills-container"> 
                <!-- System Administration Skills --> 
                <div class="skill-category"> 
                    <h3><i class="fas fa-server"></i> System Administration</h3> 
                    <div class="skill-list"> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Windows/Linux Server Management</span> 
                                <span>90%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 90%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Network Configuration</span> 
                                <span>85%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 85%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>ERP System Integration</span> 
                                <span>80%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 80%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Helpdesk Support</span> 
                                <span>95%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 95%"></div> 
                            </div> 
                        </div> 
                    </div> 
                </div> 
                 
                <!-- Cybersecurity Skills --> 
                <div class="skill-category"> 
                    <h3><i class="fas fa-shield-alt"></i> Cybersecurity</h3> 
                    <div class="skill-list"> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Vulnerability Assessment</span> 
                                <span>85%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 85%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Network Scanning (Nmap)</span> 
                                <span>90%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 90%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Metasploit Framework</span> 
                                <span>80%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 80%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Security Hardening</span> 
                                <span>75%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 75%"></div> 
                            </div> 
                        </div> 
                    </div> 
                </div> 
                 
                <!-- Tools & Technologies --> 
                <div class="skill-category"> 
                    <h3><i class="fas fa-tools"></i> Tools & Technologies</h3> 
                    <div class="skill-list"> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Nmap & Metasploit</span> 
                                <span>90%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 90%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>Microsoft Server/AD</span> 
                                <span>85%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 85%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>VMware/VirtualBox</span> 
                                <span>80%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 80%"></div> 
                            </div> 
                        </div> 
                        <div class="skill-item"> 
                            <div class="skill-name"> 
                                <span>WMS/ERP Systems</span> 
                                <span>85%</span> 
                            </div> 
                            <div class="skill-bar"> 
                                <div class="skill-level" style="width: 85%"></div> 
                            </div> 
                        </div> 
                    </div> 
                </div> 
            </div> 
        </div> 
    </section> 
 
    <!-- Blog Section --> 
    <section id="blog" style="background: #f8f9fa;"> 
        <div class="container"> 
            <h2>Cybersecurity Insights</h2> 
            <p style="text-align: center; max-width: 800px; margin: 0 auto 50px;">Sharing 
knowledge from my hands-on experience with vulnerability assessment and system 
administration.</p> 
             
            <div class="blog-posts"> 
                <!-- Article 1 --> 
                <article class="blog-post"> 
                    <div class="blog-img"> 
                        <i class="fas fa-search"></i> 
                    </div> 
                    <div class="blog-content"> 
                        <div class="blog-meta"> 
                            <span><i class="far fa-calendar"></i> December 2025</span> 
                            <span><i class="far fa-clock"></i> 5 min read</span> 
                        </div> 
                        <h3>Getting Started with Nmap for Security Assessments</h3> 
                        <p>A practical guide to using Nmap for network discovery and vulnerability 
scanning, based on my Metasploitable 2 assessment project.</p> 
                        <div class="blog-tags"> 
                            <span style="background: #e8f4fc; color: #3498db; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 
8px;">Nmap</span> 
                            <span style="background: #e8f4fc; color: #3498db; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 8px;">Network 
Security</span> 
                            <span style="background: #e8f4fc; color: #3498db; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 8px;">Beginner 
Guide</span> 
                        </div> 
                        <a href="#" class="btn">Read Article</a> 
                    </div> 
                </article> 
                 
                <!-- Article 2 --> 
                <article class="blog-post"> 
                    <div class="blog-img" style="background: linear-gradient(135deg, #e74c3c 0%, 
#c0392b 100%);"> 
                        <i class="fas fa-lock"></i> 
                    </div> 
                    <div class="blog-content"> 
                        <div class="blog-meta"> 
                            <span><i class="far fa-calendar"></i> November 2025</span> 
                            <span><i class="far fa-clock"></i> 7 min read</span> 
                        </div> 
                        <h3>Common System Administration Security Mistakes</h3> 
                        <p>From my experience in system administration, here are the most common 
security oversights I've encountered and how to fix them.</p> 
                        <div class="blog-tags"> 
                            <span style="background: #fde8e8; color: #e74c3c; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 8px;">System 
Admin</span> 
                            <span style="background: #fde8e8; color: #e74c3c; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 
8px;">Security</span> 
                            <span style="background: #fde8e8; color: #e74c3c; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 8px;">Best 
Practices</span> 
                        </div> 
                        <a href="#" class="btn">Read Article</a> 
                    </div> 
                </article> 
                 
                <!-- Article 3 --> 
                <article class="blog-post"> 
                    <div class="blog-img" style="background: linear-gradient(135deg, #27ae60 0%, 
#219653 100%);"> 
                        <i class="fas fa-graduation-cap"></i> 
                    </div> 
                    <div class="blog-content"> 
                        <div class="blog-meta"> 
                            <span><i class="far fa-calendar"></i> October 2025</span> 
                            <span><i class="far fa-clock"></i> 8 min read</span> 
                        </div> 
                        <h3>Transitioning from System Admin to Cybersecurity</h3> 
                        <p>My personal journey and practical advice for system administrators 
looking to move into cybersecurity roles.</p> 
                        <div class="blog-tags"> 
                            <span style="background: #e8f8ef; color: #27ae60; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 
8px;">Career</span> 
                            <span style="background: #e8f8ef; color: #27ae60; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 8px;">Learning 
Path</span> 
                            <span style="background: #e8f8ef; color: #27ae60; padding: 5px 10px; 
border-radius: 20px; font-size: 0.8rem; margin-right: 8px; margin-bottom: 8px;">Personal 
Experience</span> 
                        </div> 
                        <a href="#" class="btn">Read Article</a> 
                    </div> 
                </article> 
            </div> 
             
            <div style="text-align: center; margin-top: 40px;"> 
                <a href="#" class="btn">View All Articles</a> 
            </div> 
        </div> 
    </section> 
 
    <!-- Certifications Section --> 
    <section id="certifications"> 
        <div class="container"> 
            <h2>Education & Certifications</h2> 
             
            <div class="cert-grid"> 
                <!-- Formal Education --> 
                <div class="cert-card"> 
                    <h3 style="color: var(--primary); margin-bottom: 25px; display: flex; align-items: 
center;"> 
                        <i class="fas fa-graduation-cap" style="margin-right: 10px; color: 
var(--secondary);"></i> 
                        Formal Education 
                    </h3> 
                     
                    <div style="margin-bottom: 25px; padding-bottom: 20px; border-bottom: 1px 
solid #eee;"> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">Bachelor of Science in 
Computer Science</h4> 
                        <p style="color: var(--secondary); font-weight: 600;">Madonna University, 
Elele, Nigeria</p> 
                        <p style="color: var(--gray);">2011</p> 
                    </div> 
                     
                    <div style="margin-bottom: 25px; padding-bottom: 20px; border-bottom: 1px 
solid #eee;"> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">Cybersecurity 
Studies</h4> 
                        <p style="color: var(--secondary); font-weight: 600;">State University of 
Telecommunications, Kyiv, Ukraine</p> 
                        <p style="color: var(--gray);">2021 (Pending)</p> 
                    </div> 
                     
                    <div> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">German Language 
Courses (A1-B1)</h4> 
                        <p style="color: var(--secondary); font-weight: 600;">Technical University 
Dresden</p> 
                        <p style="color: var(--gray);">2022</p> 
                    </div> 
                </div> 
                 
                <!-- Certifications --> 
                <div class="cert-card"> 
                    <h3 style="color: var(--primary); margin-bottom: 25px; display: flex; align-items: 
center;"> 
                        <i class="fas fa-certificate" style="margin-right: 10px; color: 
var(--secondary);"></i> 
                        Certifications & Training 
                    </h3> 
                     
                    <div style="margin-bottom: 25px; padding-bottom: 20px; border-bottom: 1px 
solid #eee;"> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">BAMF 
Integrationskurs</h4> 
                        <p style="color: var(--secondary); font-weight: 600;">Pscherer Academy</p> 
                        <p style="color: var(--gray);">July 2025</p> 
                        <span style="background: #e8f4fc; color: var(--secondary); padding: 3px 
10px; border-radius: 20px; font-size: 0.8rem;">Completed</span> 
                    </div> 
                     
                    <div style="margin-bottom: 25px; padding-bottom: 20px; border-bottom: 1px 
solid #eee;"> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">Advanced Cybersecurity 
Course</h4> 
                        <p style="color: var(--secondary); font-weight: 600;">Online Training 
Program</p> 
                        <p style="color: var(--gray);">2024-2025</p> 
                        <span style="background: #e8f4fc; color: var(--secondary); padding: 3px 
10px; border-radius: 20px; font-size: 0.8rem;">In Progress</span> 
                    </div> 
                     
                    <div> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">IT Support 
Fundamentals</h4> 
                        <p style="color: var(--secondary); font-weight: 600;">Practical Internship</p> 
                        <p style="color: var(--gray);">Bundesmedizinisches Zentrum 
(SERVICOM)</p> 
                        <span style="background: #e8f8ef; color: #27ae60; padding: 3px 10px; 
border-radius: 20px; font-size: 0.8rem;">Completed</span> 
                    </div> 
                </div> 
                 
                <!-- In Progress --> 
                <div class="cert-card"> 
                    <h3 style="color: var(--primary); margin-bottom: 25px; display: flex; align-items: 
center;"> 
                        <i class="fas fa-spinner" style="margin-right: 10px; color: 
var(--secondary);"></i> 
                        Currently Pursuing 
                    </h3> 
                     
                    <div style="margin-bottom: 25px; padding-bottom: 20px; border-bottom: 1px 
solid #eee;"> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">CompTIA Security+</h4> 
                        <p style="color: var(--gray);">Expected completion: Q2 2025</p> 
                        <div style="background: #f1f1f1; height: 8px; border-radius: 4px; margin-top: 
10px;"> 
                            <div style="background: var(--secondary); width: 60%; height: 100%; 
border-radius: 4px;"></div> 
                        </div> 
                    </div> 
                     
                    <div style="margin-bottom: 25px; padding-bottom: 20px; border-bottom: 1px 
solid #eee;"> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">German B2 
Certification</h4> 
                        <p style="color: var(--gray);">Expected completion: Q3 2025</p> 
                        <div style="background: #f1f1f1; height: 8px; border-radius: 4px; margin-top: 
10px;"> 
                            <div style="background: var(--secondary); width: 40%; height: 100%; 
border-radius: 4px;"></div> 
                        </div> 
                    </div> 
                     
                    <div> 
                        <h4 style="color: var(--dark); margin-bottom: 5px;">Practical Cybersecurity 
Labs</h4> 
                        <p style="color: var(--gray);">Continuous hands-on training with:</p> 
                        <ul style="margin-top: 10px; padding-left: 20px;"> 
                            <li>Metasploitable 2/3</li> 
                            <li>TryHackMe & HackTheBox</li> 
                            <li>Home lab environment</li> 
                        </ul> 
                    </div> 
                </div> 
            </div> 
        </div> 
    </section> 
 
    <!-- Services Section --> 
    <section id="services" style="background: #f8f9fa;"> 
        <div class="container"> 
            <h2>Services & Expertise</h2> 
            <p style="text-align: center; max-width: 800px; margin: 0 auto 50px;">Combining 
system administration experience with cybersecurity skills to provide comprehensive IT 
solutions.</p> 
             
            <div class="services-grid"> 
                <!-- Service 1 --> 
                <div class="service-card"> 
                    <div class="service-icon"> 
                        <i class="fas fa-shield-alt"></i> 
                    </div> 
                    <h3>Vulnerability Assessment</h3> 
                    <p>Comprehensive security scanning and vulnerability identification for 
networks and systems using tools like Nmap and Metasploit.</p> 
                </div> 
                 
                <!-- Service 2 --> 
                <div class="service-card"> 
                    <div class="service-icon"> 
                        <i class="fas fa-server"></i> 
                    </div> 
                    <h3>System Administration</h3> 
                    <p>Windows/Linux server management, network configuration, and IT 
infrastructure support with a focus on security best practices.</p> 
                </div> 
                 
                <!-- Service 3 --> 
                <div class="service-card"> 
                    <div class="service-icon"> 
                        <i class="fas fa-network-wired"></i> 
                    </div> 
                    <h3>Network Security</h3> 
                    <p>Network configuration, firewall setup, and security monitoring to protect 
against unauthorized access and threats.</p> 
                </div> 
                 
                <!-- Service 4 --> 
                <div class="service-card"> 
                    <div class="service-icon"> 
                        <i class="fas fa-tools"></i> 
                    </div> 
                    <h3>IT Support & Helpdesk</h3> 
                    <p>Technical support, troubleshooting, and user assistance with ticketing 
systems and remote support tools.</p> 
                </div> 
                 
                <!-- Service 5 --> 
                <div class="service-card"> 
                    <div class="service-icon"> 
                        <i class="fas fa-database"></i> 
                    </div> 
                    <h3>ERP/WMS Integration</h3> 
                    <p>System integration and optimization for enterprise resource planning and 
warehouse management systems.</p> 
                </div> 
                 
                <!-- Service 6 --> 
                <div class="service-card"> 
                    <div class="service-icon"> 
                        <i class="fas fa-user-shield"></i> 
                    </div> 
                    <h3>Security Hardening</h3> 
                    <p>System hardening, security configuration, and implementation of security 
controls to reduce attack surface.</p> 
                </div> 
            </div> 
        </div> 
    </section> 
 
    <!-- Contact Section --> 
    <section id="contact"> 
        <div class="container"> 
            <h2>Get In Touch</h2> 
            <div class="contact-container"> 
                <div class="contact-info"> 
                    <h3>Contact Information</h3> 
                    <p>I'm currently open to new opportunities in system administration, 
cybersecurity, or IT support roles. Feel free to reach out!</p> 
                     
                    <div class="contact-item"> 
                        <div class="contact-icon"> 
                            <i class="fas fa-envelope"></i> 
                        </div> 
                        <div> 
                            <h4>Email</h4> 
                            <p>contact@okumudeh-tech.com</p> 
                        </div> 
                    </div> 
                     
                    <div class="contact-item"> 
                        <div class="contact-icon"> 
                            <i class="fas fa-map-marker-alt"></i> 
                        </div> 
                        <div> 
                            <h4>Location</h4> 
                            <p>Germany</p> 
                            <p>Open to remote/hybrid positions</p> 
                        </div> 
                    </div> 
                     
                    <div class="contact-item"> 
                        <div class="contact-icon"> 
                            <i class="fas fa-language"></i> 
                        </div> 
                        <div> 
                            <h4>Languages</h4> 
                            <p>English (Fluent)</p> 
                            <p>German (B1 Level)</p> 
                        </div> 
                    </div> 
                     
                    <div class="contact-item"> 
                        <div class="contact-icon"> 
                            <i class="fas fa-briefcase"></i> 
                        </div> 
                        <div> 
                            <h4>Availability</h4> 
                            <p>Open to full-time, part-time, or contract work</p> 
                            <p>Immediate start possible</p> 
                        </div> 
                    </div> 
                </div> 
                 
                <div class="contact-form"> 
                    <h3>Send Me a Message</h3> 
                    <form id="contactForm"> 
                        <div class="form-group"> 
                            <label for="name">Full Name</label> 
                            <input type="text" id="name" name="name" required> 
                        </div> 
                         
                        <div class="form-group"> 
                            <label for="email">Email Address</label> 
                            <input type="email" id="email" name="email" required> 
                        </div> 
                         
                        <div class="form-group"> 
                            <label for="subject">Subject</label> 
                            <input type="text" id="subject" name="subject" required> 
                        </div> 
                         
                        <div class="form-group"> 
                            <label for="message">Your Message</label> 
                            <textarea id="message" name="message" required></textarea> 
                        </div> 
                         
                        <button type="submit" class="btn">Send Message</button> 
                    </form> 
                </div> 
            </div> 
        </div> 
    </section> 
 
    <!-- Footer --> 
    <footer> 
        <div class="container"> 
            <div class="footer-content"> 
                <div class="logo" style="color: white;">Okum <span style="color: 
#3498db;">Udeh</span></div> 
                 
                <div class="social-links"> 
                    <a href="#" title="LinkedIn"><i class="fab fa-linkedin"></i></a> 
                    <a href="#" title="GitHub"><i class="fab fa-github"></i></a> 
                    <a href="#" title="Twitter"><i class="fab fa-twitter"></i></a> 
                </div> 
            </div> 
             
            <div class="copyright"> 
                <p>&copy; 2025 Okum Udeh. All rights reserved.</p> 
                <p>System Administrator & Cybersecurity Specialist</p> 
            </div> 
        </div> 
    </footer> 
 
    <!-- JavaScript for Interactive Elements --> 
    <script> 
        // Mobile menu toggle 
        const menuToggle = document.getElementById('menuToggle'); 
        const navMenu = document.getElementById('navMenu'); 
         
        menuToggle.addEventListener('click', () => { 
            navMenu.classList.toggle('active'); 
        }); 
         
        // Close menu when clicking a link 
        document.querySelectorAll('#navMenu a').forEach(link => { 
            link.addEventListener('click', () => { 
                navMenu.classList.remove('active'); 
            }); 
        }); 
         
        // Smooth scrolling for navigation links 
        document.querySelectorAll('a[href^="#"]').forEach(anchor => { 
            anchor.addEventListener('click', function(e) { 
                e.preventDefault(); 
                 
                const targetId = this.getAttribute('href'); 
                if(targetId === '#') return; 
                 
                const targetElement = document.querySelector(targetId); 
                if(targetElement) { 
                    window.scrollTo({ 
                        top: targetElement.offsetTop - 80, 
                        behavior: 'smooth' 
                    }); 
                } 
            }); 
        }); 
         
        // Simple form submission (for demo purposes) 
        document.getElementById('contactForm').addEventListener('submit', function(e) { 
            e.preventDefault(); 
            alert('Thank you for your message! I will get back to you soon.'); 
            this.reset(); 
        }); 
         
        // Add active class to nav links on scroll 
        window.addEventListener('scroll', () => { 
            let current = ''; 
            const sections = document.querySelectorAll('section'); 
             
            sections.forEach(section => { 
                const sectionTop = section.offsetTop; 
                const sectionHeight = section.clientHeight; 
                if(scrollY >= (sectionTop - 100)) { 
                    current = section.getAttribute('id'); 
                } 
            }); 
             
            document.querySelectorAll('nav ul li a').forEach(link => { 
                link.classList.remove('active'); 
                if(link.getAttribute('href') === `#${current}`) { 
                    link.classList.add('active'); 
                } 
            }); 
        }); 
</script> 
</body> 
</html>
