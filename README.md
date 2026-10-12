# doctorjones1414.github.io
test
html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Simple Blog</title>
    <style>
        /* Base Reset & Core Styles */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f7f6;
            padding-bottom: 60px;
        }
        a {
            color: #2c3e50;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }

        /* Navigation Bar */
        nav {
            background-color: #2c3e50;
            color: #fff;
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .nav-container {
            max-width: 1100px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .nav-logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #fff;
        }
        .nav-links a {
            color: #fff;
            margin-left: 1.5rem;
        }

        /* Blog Header */
        header {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://picsum.photos') no-repeat center center/cover;
            color: white;
            text-align: center;
            padding: 5rem 1rem;
        }
        header h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
        }

        /* Main Layout Grid */
        .container {
            max-width: 1100px;
            margin: 2rem auto;
            padding: 0 1rem;
            display: grid;
            grid-template-columns: 3fr 1fr;
            gap: 2rem;
        }

        /* Blog Posts */
        .main-content {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }
        .post-card {
            background: #fff;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        .post-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        .post-body {
            padding: 1.5rem;
        }
        .post-meta {
            font-size: 0.85rem;
            color: #7f8c8d;
            margin-bottom: 0.5rem;
        }
        .post-title {
            margin-bottom: 1rem;
            font-size: 1.75rem;
        }
        .read-more {
            display: inline-block;
            margin-top: 1rem;
            color: #3498db;
            font-weight: bold;
        }

        /* Sidebar */
        aside {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }
        .sidebar-widget {
            background: #fff;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        .widget-title {
            margin-bottom: 1rem;
            border-bottom: 2px solid #2c3e50;
            padding-bottom: 0.25rem;
        }
        .sidebar-widget ul {
            list-style: none;
        }
        .sidebar-widget li {
            margin-bottom: 0.5rem;
        }

        /* Footer */
        footer {
            background-color: #2c3e50;
            color: #fff;
            text-align: center;
            padding: 1.5rem;
            margin-top: 4rem;
        }

        /* Responsive Breakpoint */
        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
            }
            header h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="nav-container">
            <a href="#" class="nav-logo">DevBlog</a>
            <div class="nav-links">
                <a href="#">Home</a>
                <a href="#">Articles</a>
                <a href="#">About</a>
            </div>
        </div>
    </nav>

    <!-- Header Banner -->
    <header>
        <h1>Welcome to My Blog</h1>
        <p>Thoughts, stories, and ideas shared daily.</p>
    </header>

    <!-- Main Container -->
    <div class="container">
        
        <!-- Blog Posts Column -->
        <main class="main-content">
            
            <!-- Article 1 -->
            <article class="post-card">
                <img src="https://picsum.photos" alt="Post Image" class="post-img">
                <div class="post-body">
                    <div class="post-meta">Posted on October 12, 2026 by Alex</div>
                    <h2 class="post-title"><a href="#">Getting Started with Pure HTML & CSS</a></h2>
                    <p>Building a website doesn't always require massive frameworks. Sometimes, writing clean HTML and simple CSS is all you need to create a fast, beautiful, and highly responsive blog...</p>
                    <a href="#" class="read-more">Read More &rarr;</a>
                </div>
            </article>

            <!-- Article 2 -->
            <article class="post-card">
                <img src="https://picsum.photos" alt="Post Image" class="post-img">
                <div class="post-body">
                    <div class="post-meta">Posted on October 10, 2026 by Jess</div>
                    <h2 class="post-title"><a href="#">The Importance of Visual Content</a></h2>
                    <p>Images play a massive role in reader engagement. Learn how to optimize your blog images so they load blazing fast without sacrificing quality across mobile and desktop devices...</p>
                    <a href="#" class="read-more">Read More &rarr;</a>
                </div>
            </article>

        </main>

        <!-- Sidebar Column -->
        <aside>
            <div class="sidebar-widget">
                <h3 class="widget-title">About Me</h3>
                <p>Welcome to my corner of the internet! I am a passionate creator sharing web design tips and daily inspiration.</p>
            </div>

            <div class="sidebar-widget">
                <h3 class="widget-title">Categories</h3>
                <ul>
                    <li><a href="#">Web Design</a></li>
                    <li><a href="#">Web Development</a></li>
                    <li><a href="#">Lifestyle</a></li>
                    <li><a href="#">Technology</a></li>
                </ul>
            </div>
        </aside>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 DevBlog. All rights reserved.</p>
    </footer>

</body>
</html>
