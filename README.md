# redesigned-winner
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Digital Wealth Hub - Your Passive Income Gateway</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            background: linear-gradient(45deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: #667eea;
        }

        main {
            margin-top: 80px;
            padding: 2rem 0;
        }

        .hero {
            text-align: center;
            padding: 4rem 0;
            color: white;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(45deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.3);
        }

        .income-streams {
            background: white;
            padding: 4rem 0;
            margin: 2rem 0;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .streams-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .stream-card {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s ease;
            cursor: pointer;
        }

        .stream-card:hover {
            transform: translateY(-5px);
        }

        .stream-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .affiliate-section {
            background: rgba(255, 255, 255, 0.95);
            padding: 3rem 0;
            margin: 2rem 0;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .affiliate-links {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .affiliate-card {
            background: linear-gradient(45deg, #4facfe 0%, #00f2fe 100%);
            color: white;
            padding: 1.5rem;
            border-radius: 10px;
            text-align: center;
            text-decoration: none;
            transition: transform 0.3s ease;
        }

        .affiliate-card:hover {
            transform: scale(1.05);
        }

        .content-section {
            background: white;
            padding: 3rem 0;
            margin: 2rem 0;
            border-radius: 20px;
        }

        .blog-preview {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .blog-card {
            border: 1px solid #eee;
            border-radius: 10px;
            overflow: hidden;
            transition: box-shadow 0.3s ease;
        }

        .blog-card:hover {
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .blog-card-content {
            padding: 1.5rem;
        }

        .newsletter-signup {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 3rem 0;
            margin: 2rem 0;
            border-radius: 20px;
            text-align: center;
        }

        .email-form {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
            flex-wrap: wrap;
        }

        .email-input {
            padding: 1rem;
            border: none;
            border-radius: 25px;
            width: 300px;
            font-size: 1rem;
        }

        .submit-btn {
            padding: 1rem 2rem;
            background: #ff6b6b;
            color: white;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.3s ease;
        }

        .submit-btn:hover {
            background: #ee5a24;
        }

        footer {
            background: rgba(0, 0, 0, 0.8);
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
        }

        .monetization-tips {
            background: rgba(255, 255, 255, 0.95);
            padding: 3rem 0;
            margin: 2rem 0;
            border-radius: 20px;
        }

        .tips-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .tip-card {
            background: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
            padding: 1.5rem;
            border-radius: 10px;
            color: #333;
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .nav-links {
                display: none;
            }
            
            .email-input {
                width: 100%;
            }
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #333;
        }

        .ad-placeholder {
            background: #f8f9fa;
            border: 2px dashed #dee2e6;
            padding: 2rem;
            text-align: center;
            margin: 2rem 0;
            border-radius: 10px;
            color: #6c757d;
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">Digital Wealth Hub</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#income">Income Streams</a></li>
                <li><a href="#blog">Blog</a></li>
                <li><a href="#resources">Resources</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero" id="home">
            <div class="container">
                <h1>Build Your Passive Income Empire</h1>
                <p>Discover proven strategies to generate money while you sleep - no upfront investment required!</p>
                <a href="#income" class="cta-button">Start Building Wealth Today</a>
            </div>
        </section>

        <div class="ad-placeholder container">
            <strong>Google AdSense Ad Space</strong><br>
            728x90 Leaderboard Ad - Premium placement for maximum revenue
        </div>

        <section class="income-streams container" id="income">
            <h2 class="section-title">Multiple Income Streams</h2>
            <div class="streams-grid">
                <div class="stream-card" onclick="showDetails('affiliate')">
                    <h3>🔗 Affiliate Marketing</h3>
                    <p>Promote products you love and earn commissions on every sale. No inventory, no customer service - just pure profit!</p>
                </div>
                <div class="stream-card" onclick="showDetails('adsense')">
                    <h3>💰 Google AdSense</h3>
                    <p>Monetize your content with targeted ads. Get paid every time someone clicks or views ads on your site.</p>
                </div>
                <div class="stream-card" onclick="showDetails('courses')">
                    <h3>🎓 Online Courses</h3>
                    <p>Create once, sell forever. Turn your knowledge into automated income with digital courses.</p>
                </div>
                <div class="stream-card" onclick="showDetails('email')">
                    <h3>📧 Email Marketing</h3>
                    <p>Build a loyal audience and monetize through newsletters, product launches, and exclusive offers.</p>
                </div>
            </div>
        </section>

        <section class="affiliate-section container">
            <h2 class="section-title">Recommended Tools & Services</h2>
            <p style="text-align: center; margin-bottom: 1rem;">These are the exact tools I use to generate passive income. Click to learn more!</p>
            <div class="affiliate-links">
                <a href="#" class="affiliate-card" onclick="trackClick('bluehost')">
                    <h3>🌐 Bluehost Hosting</h3>
                    <p>Professional website hosting starting at $2.95/month. Get your site online today!</p>
                </a>
                <a href="#" class="affiliate-card" onclick="trackClick('mailchimp')">
                    <h3>📬 Mailchimp</h3>
                    <p>Build your email list and automate your marketing. Free plan available!</p>
                </a>
                <a href="#" class="affiliate-card" onclick="trackClick('canva')">
                    <h3>🎨 Canva Pro</h3>
                    <p>Create stunning graphics and content. Essential for social media success!</p>
                </a>
                <a href="#" class="affiliate-card" onclick="trackClick('teachable')">
                    <h3>🏫 Teachable</h3>
                    <p>Create and sell online courses. Turn your expertise into recurring revenue!</p>
                </a>
            </div>
        </section>

        <div class="ad-placeholder container">
            <strong>Google AdSense Ad Space</strong><br>
            300x250 Medium Rectangle - High-converting ad placement
        </div>

        <section class="content-section container" id="blog">
            <h2 class="section-title">Latest Wealth-Building Content</h2>
            <div class="blog-preview">
                <article class="blog-card">
                    <div class="blog-card-content">
                        <h3>10 Ways to Make $100/Day Online</h3>
                        <p>Discover legitimate methods to earn money online that actually work. From freelancing to affiliate marketing...</p>
                        <a href="#" onclick="trackPageView('blog1')">Read More →</a>
                    </div>
                </article>
                <article class="blog-card">
                    <div class="blog-card-content">
                        <h3>Building Your First Sales Funnel</h3>
                        <p>Learn how to create automated sales systems that convert visitors into customers while you sleep...</p>
                        <a href="#" onclick="trackPageView('blog2')">Read More →</a>
                    </div>
                </article>
                <article class="blog-card">
                    <div class="blog-card-content">
                        <h3>Email Marketing That Actually Works</h3>
                        <p>Stop sending emails that get ignored. Master the art of email marketing that generates real revenue...</p>
                        <a href="#" onclick="trackPageView('blog3')">Read More →</a>
                    </div>
                </article>
            </div>
        </section>

        <section class="monetization-tips container">
            <h2 class="section-title">Zero-Cost Monetization Strategies</h2>
            <div class="tips-grid">
                <div class="tip-card">
                    <h3>🆓 Free Platform Strategy</h3>
                    <p>Start with free platforms like Medium, YouTube, or social media. Build your audience first, then monetize.</p>
                </div>
                <div class="tip-card">
                    <h3>📱 Social Media Leverage</h3>
                    <p>Use Instagram, TikTok, and Twitter to drive traffic to your monetized content. Viral content = passive income.</p>
                </div>
                <div class="tip-card">
                    <h3>🤝 Cross-Promotion</h3>
                    <p>Partner with other creators for mutual promotion. Grow faster by leveraging existing audiences.</p>
                </div>
                <div class="tip-card">
                    <h3>🔄 Content Repurposing</h3>
                    <p>Turn one piece of content into multiple income streams. One blog post becomes videos, podcasts, and courses.</p>
                </div>
            </div>
        </section>

        <section class="newsletter-signup container">
            <h2>Join 50,000+ Passive Income Earners</h2>
            <p>Get exclusive strategies, tools, and opportunities delivered to your inbox weekly</p>
            <form class="email-form" onsubmit="handleSignup(event)">
                <input type="email" class="email-input" placeholder="Enter your email address" required>
                <button type="submit" class="submit-btn">Get Free Guide</button>
            </form>
        </section>

        <div class="ad-placeholder container">
            <strong>Google AdSense Ad Space</strong><br>
            320x50 Mobile Banner - Optimized for mobile traffic
        </div>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2024 Digital Wealth Hub. Building passive income streams since 2024.</p>
            <p>Disclaimer: Results may vary. This site contains affiliate links.</p>
        </div>
    </footer>

    <script>
        // Analytics and tracking functions
        function trackClick(product) {
            console.log(`Affiliate click tracked: ${product}`);
            // In real implementation, send to Google Analytics
            alert(`You clicked on ${product}! In a real site, this would redirect to the affiliate link.`);
        }

        function trackPageView(page) {
            console.log(`Page view tracked: ${page}`);
            alert(`Loading ${page} content...`);
        }

        function showDetails(stream) {
            const details = {
                affiliate: "Affiliate marketing can generate $1000-$10000+ monthly. Start by joining Amazon Associates, ShareASale, or ClickBank.",
                adsense: "Google AdSense can earn $1-5 per 1000 page views. Focus on high-traffic, valuable content.",
                courses: "Online courses can generate $500-$50000+ in passive income. Use platforms like Teachable or Udemy.",
                email: "Email marketing has an average ROI of $42 for every $1 spent. Build your list early!"
            };
            alert(details[stream]);
        }

        function handleSignup(event) {
            event.preventDefault();
            const email = event.target.querySelector('input[type="email"]').value;
            alert(`Thank you for signing up with ${email}! You'll receive your free passive income guide shortly.`);
            // In real implementation, integrate with email service provider
        }

        // Smooth scrolling for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Simple visitor counter (in real site, use proper analytics)
        let visitorCount = localStorage.getItem('visitorCount') || 0;
        visitorCount++;
        localStorage.setItem('visitorCount', visitorCount);
        console.log(`Visitor #${visitorCount}`);
    </script>
</body>
</html>
