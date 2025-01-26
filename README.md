<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Promote your Twitch channel with this dynamic and visually engaging website. Follow, watch, and join the fun.">
    <title>AddywithaBlick</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #1e1e2e;
            color: #ffffff;
            line-height: 1.6;
            transition: background-color 0.3s, color 0.3s;
        }

        body.light-mode {
            background-color: #ffffff;
            color: #000000;
        }

        header.hero {
            text-align: center;
            background-color: #9146ff;
            padding: 60px 20px;
        }

        header h1 {
            font-size: 3rem;
        }

        header p {
            margin-top: 10px;
            font-size: 1.2rem;
        }

        header .cta-button {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 30px;
            background-color: #ff4500;
            color: #ffffff;
            text-decoration: none;
            font-size: 1.2rem;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        header .cta-button:hover {
            background-color: #ff6347;
        }

        section {
            padding: 40px 20px;
            text-align: center;
        }

        section h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .about p, .schedule ul {
            font-size: 1.2rem;
            margin: 0 auto;
            max-width: 600px;
        }

        .schedule ul {
            list-style: none;
            padding: 0;
        }

        .schedule li {
            margin: 10px 0;
        }

        iframe {
            border: none;
            width: 80%;
            height: 400px;
            margin: 20px auto;
            display: block;
        }

        footer {
            background-color: #333333;
            color: #bbbbbb;
            text-align: center;
            padding: 20px 0;
        }

        footer a {
            color: #9146ff;
            text-decoration: none;
            margin: 0 10px;
            font-size: 1.2rem;
        }

        footer a:hover {
            text-decoration: underline;
        }

        .countdown {
            font-size: 1.5rem;
            margin-top: 20px;
        }

        .contact-form {
            max-width: 600px;
            margin: 20px auto;
        }

        .contact-form input, .contact-form textarea, .contact-form button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }

        .contact-form button {
            background-color: #9146ff;
            color: white;
            cursor: pointer;
        }

        .contact-form button:hover {
            background-color: #ff4500;
        }

        .faq ul {
            list-style: none;
            padding: 0;
            text-align: left;
            max-width: 600px;
            margin: 0 auto;
        }

        .faq li {
            margin-bottom: 20px;
        }

        .newsletter {
            margin-top: 20px;
        }

        .newsletter form input, .newsletter form button {
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }

        .newsletter form button {
            background-color: #9146ff;
            color: white;
            cursor: pointer;
        }

        .newsletter form button:hover {
            background-color: #ff4500;
        }

        .toggle-mode {
            margin: 20px;
            cursor: pointer;
        }

        .merch-section {
            text-align: center;
            margin: 40px 20px;
        }
    </style>
</head>
<body>
    <header class="hero">
        <h1>Welcome to addywithablick's Twitch Channel!</h1>
        <p>Come catch the wild adventures with the boys on the game and IRL</p>
        <a href="https://www.twitch.tv/addywithablick" class="cta-button" target="_blank">Watch Now</a>
        <p id="live-status">Checking live status...</p>
        <p id="follower-count">Fetching follower count...</p>
        <button class="toggle-mode" onclick="toggleMode()">Toggle Dark/Light Mode</button>
    </header>

    <section class="about">
        <h2>About Us</h2>
        <p>Just two childhood friends out in the real world showing our outdoor, party, cooking, and gaming adventures. Come join!</p>
    </section>

    <section class="schedule">
        <h2>Streaming Schedule</h2>
        <ul>
            <li>7 Days a Week: 7 PM Central - Midnight (and sometimes later!)</li>
        </ul>
        <div class="countdown">
            <h3>Next Stream Starts In:</h3>
            <p id="timer">Loading...</p>
        </div>
    </section>

    <section class="highlights">
        <h2>Fan Clip Gallery</h2>
        <p>Submit your favorite moments to be featured!</p>
        <div class="gallery">
            <p>No clips submitted yet. Be the first!</p>
        </div>
    </section>

    <section class="faq">
        <h2>Frequently Asked Questions</h2>
        <ul>
            <li><strong>Q:</strong> What games do you stream?<br><strong>A:</strong> We stream a mix of outdoor, party, cooking, and popular video games.</li>
            <li><strong>Q:</strong> How can I support your channel?<br><strong>A:</strong> Follow us, subscribe, and share our channel with friends!</li>
        </ul>
    </section>

    <section class="merch-section">
        <h2>Merchandise</h2>
        <p>Coming Soon! Stay tuned for our exclusive merch.</p>
    </section>

    <section class="contact">
        <h2>Contact Us</h2>
        <form class="contact-form" action="mailto:addyandnickclips@gmail.com" method="POST" enctype="text/plain">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" rows="4" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <section class="newsletter">
        <h2>Subscribe to Our Weekly Newsletter</h2>
        <p>Releases at 1,000 Twitch subscribers!</p>
        <form action="#">
            <input type="email" placeholder="Enter your email" required>
            <button type="submit" disabled>Subscribe</button>
        </form>
    </section>

    <section class="social-media">
        <h2>Follow Us on Social Media</h2>
        <p>
            <a href="https://discord.gg/yPeEk4gm" target="_blank">Join our Discord</a>
        </p>
        <div>
            <blockquote class="tiktok-embed" cite="https://www.tiktok.com/@addywithablickofficial" data-unique-id="addywithablickofficial" data-embed-type="creator" style="max-width: 780px; min-width: 288px;">
                <section>
                    <a target="_blank" href="https://www.tiktok.com/@addywithablickofficial?refer=creator_embed">@addywithablickofficial</a>
                </section>
            </blockquote>
            <script async src="https://www.tiktok.com/embed.js"></script>
            <iframe src="https://www.instagram.com/addywithablick/embed" title="Instagram Feed" width="320" height="500" style="border:none;overflow:hidden;"></iframe>
        </div>
    </section>

    <footer>
        <p>Follow us: 
            <a href="https://instagram.com/addywithablick" target="_blank"><i class="fab fa-instagram"></i> Instagram</a> | 
            <a href="https://www.tiktok.com/@addywithablickofficial" target="_blank"><i class="fab fa-tiktok"></i> TikTok</a>
        </p>
        <p>&copy; 2025 addywithablick. All Rights Reserved.</p>
    </footer>

    <script>
        // Toggle Dark/Light Mode
        function toggleMode() {
            document.body.classList.toggle('light-mode');
        }

        // Countdown timer
        const targetTime = new Date();
        targetTime.setHours(19, 0, 0); // 7 PM Central

        function updateTimer() {
            const now = new Date();
            const diff = targetTime - now;

            if (diff > 0) {
                const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((diff % (1000 * 60)) / 1000);
                document.getElementById('timer').textContent = `${hours}h ${minutes}m ${seconds}s`;
            } else {
                document.getElementById('timer').textContent = "We are live now!";
            }
        }

        setInterval(updateTimer, 1000);
    </script>
</body>
</html>
