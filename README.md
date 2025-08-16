# Jake-sales-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stop Competing on Price Forever | Jake Setterlun</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html, body {
            overflow-x: hidden;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background: #000;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .section {
            padding: 60px 0;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #000 0%, #1a1a1a 100%);
            color: white;
            text-align: center;
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
        }
        
        .preheader {
            font-size: 14px;
            color: #ff6b35;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 20px;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 25px;
            background: linear-gradient(135deg, #fff 0%, #ff6b35 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .hero .subheader {
            font-size: 1.4rem;
            color: #ccc;
            margin-bottom: 40px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .vsl-container {
            margin: 40px 0;
        }
        
        .vsl-icon {
            position: relative;
            display: inline-block;
            cursor: pointer;
            transition: transform 0.3s ease;
        }
        
        .vsl-icon:hover {
            transform: scale(1.05);
        }
        
        .vsl-thumbnail {
            width: 300px;
            height: 169px;
            background: linear-gradient(135deg, #ff6b35 0%, #ff8c42 100%);
            border-radius: 15px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 20px 40px rgba(255, 107, 53, 0.3);
        }
        
        .play-button {
            width: 60px;
            height: 60px;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }
        
        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 20px solid #ff6b35;
            border-top: 12px solid transparent;
            border-bottom: 12px solid transparent;
            margin-left: 5px;
        }
        
        .vsl-text {
            margin-top: 15px;
            font-size: 16px;
            color: #ff6b35;
            font-weight: 600;
        }
        
        .cta-button {
            background: linear-gradient(135deg, #ff6b35 0%, #ff8c42 100%);
            color: white;
            padding: 18px 40px;
            border: none;
            border-radius: 50px;
            font-size: 18px;
            font-weight: 700;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s ease;
            box-shadow: 0 10px 30px rgba(255, 107, 53, 0.4);
            margin-top: 30px;
        }
        
        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 40px rgba(255, 107, 53, 0.6);
        }
        
        /* Problem Section */
        .problem {
            background: #111;
            color: white;
        }
        
        .problem h2 {
            font-size: 2.5rem;
            color: #ff6b35;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .problem-content {
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.2rem;
            line-height: 1.8;
        }
        
        .problem-content p {
            margin-bottom: 25px;
        }
        
        /* Origin Story */
        .origin {
            background: #000;
            color: white;
        }
        
        .origin h2 {
            font-size: 2.5rem;
            color: #ff6b35;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .origin-content {
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.2rem;
            line-height: 1.8;
        }
        
        .origin-content p {
            margin-bottom: 25px;
        }
        
        /* Solution Section */
        .solution {
            background: #111;
            color: white;
        }
        
        .solution h2 {
            font-size: 2.5rem;
            color: #ff6b35;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .solution-content {
            max-width: 900px;
            margin: 0 auto;
        }
        
        .mechanism-box {
            background: linear-gradient(135deg, #ff6b35 0%, #ff8c42 100%);
            padding: 40px;
            border-radius: 20px;
            margin: 40px 0;
            text-align: center;
        }
        
        .mechanism-box h3 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: white;
        }
        
        .bullets {
            list-style: none;
            margin: 30px 0;
        }
        
        .bullets li {
            padding: 15px 0;
            font-size: 1.1rem;
            border-bottom: 1px solid #333;
        }
        
        .bullets li:before {
            content: "✓";
            color: #ff6b35;
            font-weight: bold;
            margin-right: 15px;
        }
        
        /* Product Section */
        .product {
            background: #000;
            color: white;
        }
        
        .product h2 {
            font-size: 2.5rem;
            color: #ff6b35;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }
        
        .product-card {
            background: #111;
            padding: 30px;
            border-radius: 15px;
            border: 2px solid #333;
            transition: all 0.3s ease;
        }
        
        .product-card:hover {
            border-color: #ff6b35;
            transform: translateY(-5px);
        }
        
        .product-card h3 {
            color: #ff6b35;
            font-size: 1.5rem;
            margin-bottom: 20px;
        }
        
        /* Offer Section */
        .offer {
            background: #111;
            color: white;
            text-align: center;
        }
        
        .offer h2 {
            font-size: 2.5rem;
            color: #ff6b35;
            margin-bottom: 30px;
        }
        
        .guarantee-box {
            background: linear-gradient(135deg, #ff6b35 0%, #ff8c42 100%);
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        /* FAQ Section */
        .faq {
            background: #000;
            color: white;
        }
        
        .faq h2 {
            font-size: 2.5rem;
            color: #ff6b35;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .faq-item {
            background: #111;
            margin: 20px 0;
            border-radius: 10px;
            overflow: hidden;
        }
        
        .faq-question {
            background: #222;
            padding: 20px;
            cursor: pointer;
            font-weight: 600;
            font-size: 1.1rem;
        }
        
        .faq-answer {
            padding: 20px;
            display: none;
        }
        
        .faq-answer.active {
            display: block;
        }
        
        /* Responsive Design */
        @media (max-width: 1024px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .section {
                padding: 40px 0;
            }
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 0 15px;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero .subheader {
                font-size: 1.1rem;
            }
            
            .vsl-thumbnail {
                width: 250px;
                height: 141px;
            }
            
            .problem h2, .origin h2, .solution h2, .product h2, .offer h2, .faq h2 {
                font-size: 2rem;
            }
            
            .product-grid {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 480px) {
            .hero h1 {
                font-size: 1.8rem;
            }
            
            .vsl-thumbnail {
                width: 200px;
                height: 112px;
            }
            
            .play-button {
                width: 50px;
                height: 50px;
            }
            
            .play-button::after {
                border-left: 15px solid #ff6b35;
                border-top: 10px solid transparent;
                border-bottom: 10px solid transparent;
            }
        }
        
        .highlight {
            color: #ff6b35;
            font-weight: bold;
        }
        
        .italic {
            font-style: italic;
        }
        
        .bold {
            font-weight: bold;
        }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <div class="preheader">ATTENTION: Agency Owners, Coaches & High-Ticket Service Providers</div>
            
            <h1>Turn Your Business Into A "Category of One" That Sells Itself In 90 Days Using The Purple Ocean Offer™</h1>
            
            <div class="subheader">
                Finally escape the price war hellscape... without chasing every new marketing tactic or burning through your ad budget on offers that don't convert.
            </div>
            
            <div class="vsl-container">
                <a href="https://docs.google.com/document/d/17tZGRr7IOVO7eko7vjxCeAKVe5mZk0rHjACdEFZcQBI/edit?usp=sharing" class="vsl-icon" target="_blank">
                    <div class="vsl-thumbnail">
                        <div class="play-button"></div>
                    </div>
                    <div class="vsl-text">Click Here To See The: VSL I WROTE FOR YOU</div>
                </a>
            </div>
            
            <a href="#offer" class="cta-button">Apply For 1-on-1 Coaching Now</a>
        </div>
    </section>

    <!-- PROBLEM IDENTIFICATION -->
    <section class="problem section">
        <div class="container">
            <h2>Why Smart Business Owners Are Still Drowning In A Sea Of "Me Too" Competitors</h2>
            
            <div class="problem-content">
                <p>You've tried everything...</p>
                
                <p>You've spent <span class="highlight">thousands</span> on Facebook ads that got you lukewarm leads who ghost you the moment you mention price.</p>
                
                <p>You've hired "experts" who promised you the <span class="italic">secret sauce</span>... only to deliver the same recycled tactics every other agency is using.</p>
                
                <p>You've watched competitors slash their prices to the bone while you're stuck trying to justify why you're worth more than the guy charging half your rate.</p>
                
                <p><span class="bold">And every day that passes...</span></p>
                
                <p>You feel that knot in your stomach getting tighter.</p>
                
                <p>Because deep down, you know that if something doesn't change <span class="highlight">fast</span>, you'll either burn out competing in this race to the bottom... or watch your business slowly suffocate in a market that treats you like a commodity.</p>
                
                <p>But what if I told you there was a way to step out of this nightmare completely?</p>
                
                <p>What if you could position your offer so uniquely that price becomes irrelevant... and prospects actually <span class="italic">thank you</span> for charging premium rates?</p>
            </div>
        </div>
    </section>

    <!-- ORIGIN STORY -->
    <section class="origin section">
        <div class="container">
            <h2>How I Went From Price War Prisoner To Building Six 7-Figure Agencies</h2>
            
            <div class="origin-content">
                <p>Three years ago, I was exactly where you are right now.</p>
                
                <p>Running an agency that was technically "successful" but felt like I was constantly swimming upstream.</p>
                
                <p>Every pitch meeting felt like an uphill battle. Prospects would nod along, then hit me with: <span class="italic">"Your competitor quoted us 40% less..."</span></p>
                
                <p>I was working 70-hour weeks, stressed out of my mind, and wondering if this entrepreneurship thing was just a fancy word for "professional masochist."</p>
                
                <p>Then something clicked during a conversation with a prospect who chose a competitor charging <span class="highlight">triple</span> what I was asking.</p>
                
                <p>I asked him why.</p>
                
                <p>His answer changed everything: <span class="italic">"They didn't sell me marketing services. They sold me a path to becoming the undisputed leader in my industry."</span></p>
                
                <p>That's when I realized the fatal flaw in 99% of business offers...</p>
                
                <p>They're focused on features and benefits instead of <span class="bold">transformation and identity.</span></p>
                
                <p>Over the next 18 months, I completely rebuilt my approach. I developed what I now call the <span class="highlight">Purple Ocean Offer™</span> framework.</p>
                
                <p>The results? Six different agencies scaled to 7 figures. Clients hitting 9-figure ad revenues. And me? I stopped competing and started dictating terms.</p>
            </div>
        </div>
    </section>

    <!-- SOLUTION REVELATION -->
    <section class="solution section">
        <div class="container">
            <h2>The Purple Ocean Offer™: Your Escape From The Price War Prison</h2>
            
            <div class="solution-content">
                <p style="font-size: 1.2rem; text-align: center; margin-bottom: 40px;">Here's the truth nobody wants to tell you about why your offers aren't converting...</p>
                
                <div class="mechanism-box">
                    <h3>The Purple Ocean Offer™</h3>
                    <p>A proven methodology that positions your business as the <span class="bold">only logical choice</span> in your market by creating a category so unique, so compelling, that price comparison becomes impossible.</p>
                </div>
                
                <p>While everyone else is fighting in the bloody "Red Ocean" of price wars and feature battles...</p>
                
                <p>You'll be swimming alone in your own "Purple Ocean" where you set the rules, dictate the terms, and prospects actually feel <span class="italic">grateful</span> to pay your premium rates.</p>
                
                <p><span class="bold">Here's what makes this different from every other "positioning" strategy you've heard:</span></p>
                
                <ul class="bullets">
                    <li><span class="bold">Customer-Centric Framework →</span> Stop guessing what your market wants and start speaking their exact internal language → <span class="italic">Become the obvious choice in their mind</span></li>
                    
                    <li><span class="bold">Identity-Based Positioning →</span> Position your offer as who they become, not what they get → <span class="italic">Command premium prices for transformation</span></li>
                    
                    <li><span class="bold">Category Creation Blueprint →</span> Build your own market instead of fighting for scraps → <span class="italic">Eliminate competition by making it irrelevant</span></li>
                    
                    <li><span class="bold">Conversion Psychology Mastery →</span> Craft offers that feel inevitable to your ideal prospects → <span class="italic">Close deals without pushy sales tactics</span></li>
                </ul>
                
                <p style="text-align: center; font-size: 1.3rem; margin-top: 40px;"><span class="highlight">Real Result:</span> Clients regularly hitting $1M+ months while charging 2-3x their competitors.</p>
            </div>
        </div>
    </section>

    <!-- PRODUCT INTRODUCTION -->
    <section class="product section">
        <div class="container">
            <h2>Your Complete Business Domination System</h2>
            
            <div class="product-grid">
                <div class="product-card">
                    <h3>Setterlun University™</h3>
                    <p>The complete Purple Ocean Offer™ training system delivered through our exclusive Skool community.</p>
                    <br>
                    <p><span class="bold">What you get:</span> Step-by-step modules, live masterclasses, peer community, and direct access to the frameworks that built six 7-figure agencies.</p>
                </div>
                
                <div class="product-card">
                    <h3>1-on-1 Coaching & Mentorship</h3>
                    <p>Weekly strategy sessions where I personally guide you through implementing your Purple Ocean Offer™.</p>
                    <br>
                    <p><span class="bold">What you get:</span> Custom action plans, real-time feedback, lifestyle guidance, and the accountability that ensures you actually execute (not just consume).</p>
                </div>
                
                <div class="product-card">
                    <h3>C-Board Partner Program</h3>
                    <p>For established entrepreneurs ready to hit $1M+ months consistently.</p>
                    <br>
                    <p><span class="bold">What you get:</span> High-level strategic partnership, advanced scaling techniques, and direct access to my network of 8 and 9-figure operators.</p>
                </div>
            </div>
            
            <p style="text-align: center; font-size: 1.2rem; margin-top: 40px;">This isn't another course you'll buy and forget about. This is a complete business operating system designed to make you <span class="highlight">competition-proof.</span></p>
        </div>
    </section>

    <!-- OFFER STRUCTURE -->
    <section class="offer section" id="offer">
        <div class="container">
            <h2>Your Investment In Market Domination</h2>
            
            <p style="font-size: 1.3rem; margin-bottom: 30px;">Here's the reality check you need to hear...</p>
            
            <p style="font-size: 1.1rem; margin-bottom: 30px;">You could spend the next two years trying to figure this out on your own. Testing different offers, burning through ad spend, watching competitors eat your lunch while you play catch-up.</p>
            
            <p style="font-size: 1.1rem; margin-bottom: 30px;"><span class="bold">Conservative estimate:</span> That'll cost you at least $200K in lost revenue and wasted ad spend.</p>
            
            <p style="font-size: 1.1rem; margin-bottom: 40px;">Or you could fast-track the entire process by working directly with someone who's already cracked the code.</p>
            
            <div class="guarantee-box">
                <h3 style="margin-bottom: 20px;">My Personal Guarantee</h3>
                <p>If you implement the Purple Ocean Offer™ framework and don't see a dramatic improvement in your offer's conversion rate within 90 days, I'll work with you for free until you do.</p>
            </div>
            
            <p style="font-size: 1.2rem; margin: 30px 0;"><span class="bold">But here's the thing...</span></p>
            
            <p style="font-size: 1.1rem; margin-bottom: 30px;">I only work with 12 new clients per quarter. Not because I'm trying to create fake scarcity, but because this level of personal attention is impossible to scale beyond that number.</p>
            
            <p style="font-size: 1.1rem; margin-bottom: 40px;">Applications close this Friday at midnight, and based on the interest we're seeing, spots will be gone before then.</p>
            
            <a href="https://jakesetterlun.com" class="cta-button" style="font-size: 20px; padding: 20px 50px;">Apply For 1-on-1 Coaching Now</a>
            
            <p style="font-size: 14px; margin-top: 20px; opacity: 0.8;">Note: This is an application, not a purchase. We'll review your business and goals to ensure this is the right fit for both of us.</p>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="faq section">
        <div class="container">
            <h2>Questions That Keep Coming Up</h2>
            
            <div class="faq-item">
                <div class="faq-question">Q: How is this different from other positioning courses?</div>
                <div class="faq-answer">
                    <p>Most positioning courses teach you to find a "gap" in the market. The Purple Ocean Offer™ teaches you to <span class="bold">create</span> your own market. We're not looking for empty spaces - we're building new categories where you're the only player that matters.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: What if my industry is too saturated?</div>
                <div class="faq-answer">
                    <p>The more saturated your industry, the bigger the opportunity. When everyone looks the same, standing out becomes incredibly valuable. I've helped clients dominate in everything from real estate to digital marketing to fitness coaching.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: How much time does this require?</div>
                <div class="faq-answer">
                    <p>Plan on 5-8 hours per week. This includes our weekly calls, implementing the frameworks, and engaging with the community. The question isn't whether you have time - it's whether you can afford NOT to make this change.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question">Q: What if I'm just starting out?</div>
                <div class="faq-answer">
                    <p>Perfect. It's easier to build the right foundation from the start than to rebuild later. However, you should have at least some revenue coming in and a clear vision of who you want to serve.</p>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 50px;">
                <p style="font-size: 1.2rem; margin-bottom: 30px;">Still have questions? The application process includes a strategy call where we'll address everything specific to your situation.</p>
                
                <a href="https://jakesetterlun.com" class="cta-button">Apply Now - Limited Spots Remaining</a>
            </div>
        </div>
    </section>

    <script>
        // FAQ Functionality
        document.querySelectorAll('.faq-question').forEach(question => {
            question.addEventListener('click', () => {
                const answer = question.nextElementSibling;
                const isActive = answer.classList.contains('active');
                
                // Close all answers
                document.querySelectorAll('.faq-answer').forEach(ans => {
                    ans.classList.remove('active');
                });
                
                // Open clicked answer if it wasn't active
                if (!isActive) {
                    answer.classList.add('active');
                }
            });
        });

        // Smooth scrolling for anchor links
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
    </script>
</body>
</html>
