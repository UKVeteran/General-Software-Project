<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project Name</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            transition: background-color 0.3s, color 0.3s;
        }
        header {
            background: #333;
            color: white;
            padding: 20px 0;
            text-align: center;
            transition: background-color 0.3s;
        }
        header h1 {
            margin: 0;
        }
        .badge {
            margin: 0 5px;
            text-decoration: none;
            padding: 5px 15px;
            background-color: #555;
            color: white;
            border-radius: 5px;
            font-size: 14px;
        }
        .badge:hover {
            background-color: #333;
        }
        .toggle-btn {
            background-color: #555;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .toggle-btn:hover {
            background-color: #333;
        }
        .collapsible {
            background-color: #f1f1f1;
            color: #333;
            cursor: pointer;
            padding: 10px;
            width: 100%;
            border: none;
            text-align: left;
            outline: none;
            font-size: 15px;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .active, .collapsible:hover {
            background-color: #ccc;
        }
        .content {
            padding: 0 18px;
            display: none;
            overflow: hidden;
            background-color: #f9f9f9;
            border-radius: 5px;
        }
        .dark-mode {
            background-color: #333;
            color: white;
        }
        .dark-mode header {
            background-color: #222;
        }
        .dark-mode .badge {
            background-color: #444;
        }
        .dark-mode .badge:hover {
            background-color: #222;
        }
        .dark-mode .collapsible {
            background-color: #555;
            color: white;
        }
        .dark-mode .content {
            background-color: #444;
        }
        .feature-list {
            display: flex;
            flex-wrap: wrap;
        }
        .feature-list div {
            flex: 1 1 200px;
            padding: 10px;
            margin: 10px;
            background: #f4f4f4;
            border-radius: 8px;
            text-align: center;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #333;
            color: white;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        .demo-image {
            width: 100%;
            max-width: 800px;
            border-radius: 8px;
            margin-top: 20px;
        }
    </style>
</head>
<body>

<header>
    <h1>🚀 Project Name</h1>
    <button class="toggle-btn" onclick="toggleDarkMode()">Toggle Dark Mode</button>
    <div>
        <a href="https://github.com/username/repo-name" target="_blank" class="badge">Star on GitHub</a>
        <a href="https://github.com/username/repo-name/fork" target="_blank" class="badge">Fork</a>
        <a href="https://github.com/username/repo-name/issues" target="_blank" class="badge">Issues</a>
    </div>
</header>

<section class="table-of-contents">
    <h2>📜 Table of Contents</h2>
    <ul>
        <li><a href="#about">About the Project</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#usage">Usage</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#contributing">Contributing</a></li>
        <li><a href="#license">License</a></li>
        <li><a href="#acknowledgements">Acknowledgements</a></li>
    </ul>
</section>

<section id="about">
    <h2>🚀 About the Project</h2>
    <p>This project is a <strong>brief description of your project</strong>. It solves <em>problem description</em> by using <strong>technologies</strong>. This can be a great starting point for a lot of cool things!</p>
    <img src="https://via.placeholder.com/800x400?text=Project+Demo" alt="Demo Image" class="demo-image">
</section>

<section id="installation">
    <h2>🛠️ Installation</h2>
    <button class="collapsible">Click to view Installation steps</button>
    <div class="content">
        <p>To install this project locally, follow the steps below:</p>
        <pre>
git clone https://github.com/username/repo-name.git
cd repo-name
npm install
npm start
        </pre>
    </div>
</section>

<section id="usage">
    <h2>🎮 Usage</h2>
    <button class="collapsible">Click to view Usage steps</button>
    <div class="content">
        <p>Run the following commands to build and test the project:</p>
        <pre>
npm run build
npm test
        </pre>
    </div>
</section>

<section id="features">
    <h2>⭐ Features</h2>
    <div class="feature-list">
        <div>
            <h3>Feature 1</h3>
            <p>Feature description</p>
        </div>
        <div>
            <h3>Feature 2</h3>
            <p>Feature description</p>
        </div>
        <div>
            <h3>Feature 3</h3>
            <p>Feature description</p>
        </div>
    </div>
</section>

<section id="contributing">
    <h2>🤝 Contributing</h2>
    <p>We welcome contributions! To contribute, follow these steps:</p>
    <pre>
1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push your changes
5. Open a pull request
    </pre>
</section>

<section id="license">
    <h2>📜 License</h2>
    <p>This project is licensed under the MIT License. See the <a href="LICENSE">LICENSE</a> file for more details.</p>
</section>

<section id="acknowledgements">
    <h2>💡 Acknowledgements</h2>
    <p>Special thanks to the following:</p>
    <ul>
        <li><strong>Contributor 1</strong> - for valuable feedback.</li>
        <li><strong>Framework</strong> - for providing great tools.</li>
    </ul>
</section>

<footer>
    <p>Made with ❤️ by <a href="https://github.com/username" target="_blank">Your Name</a></p>
</footer>

<script>
    // Toggle Dark Mode
    function toggleDarkMode() {
        document.body.classList.toggle("dark-mode");
    }

    // Collapsible sections
    var coll = document.getElementsByClassName("collapsible");
    for (var i = 0; i < coll.length; i++) {
        coll[i].addEventListener("click", function() {
            this.classList.toggle("active");
            var content = this.nextElementSibling;
            if (content.style.display === "block") {
                content.style.display = "none";
            } else {
                content.style.display = "block";
            }
        });
    }
</script>

</body>
</html>
