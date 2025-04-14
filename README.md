<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>guanxiainc开发者</h1>
    <nav>
      <ul>
        <li><a href="#home">首页</a></li>
        <li><a href="#about">关于</a></li>
        <li><a href="#contact">联系</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section id="home">
      <h2>首页</h2>
      <p>这是开发项目示例。</p>
    </section>
    <section id="about">
      <h2>关于</h2>
      <p>这个网站是用HTML、CSS和JavaScript构建的。</p>
    </section>
    <section id="contact">
      <h2>联系</h2>
      <form id="contactForm">
        <label for="name">名称:</label>
        <input type="text" id="name" name="name" required>
        
        <label for="message">信息:</label>
        <textarea id="message" name="message" required></textarea>
        
        <button type="submit">提交</button>
      </form>
    </section>
  </main>
  <footer>
    <p>&copy; 2025 guanxia inc </p>
  </footer>
  <script src="script.js"></script>
</body>
</html>
98197408<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>欢迎来到我的网站</h1>
    <nav>
      <ul>
        <li><a href="#home">首页</a></li>
        <li><a href="#about">关于</a></li>
        <li><a href="#contact">联系</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section id="home">
      <h2>首页</h2>
      <p>这是一个简单的网站示例。</p>
    </section>
    <section id="about">
      <h2>关于</h2>
      <p>这个网站是用HTML、CSS和JavaScript构建的。</p>
    </section>
    <section id="contact">
      <h2>联系</h2>
      <form id="contactForm">
        <label for="name">名称:</label>
        <input type="text" id="name" name="name" required>
        
        <label for="message">信息:</label>
        <textarea id="message" name="message" required></textarea>
        
        <button type="submit">提交</button>
      </form>
    </section>
  </main>
  <footer>
    <p>&copy; 2025 我的简单网站</p>
  </footer>
  <script src="script.js"></script>
</body>
</html>body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  color: #333;
  background-color: #f4f4f4;
}

header {
  background: #35424a;
  color: #ffffff;
  padding: 1rem 0;
  text-align: center;
}

header h1 {
  margin: 0;
}

nav ul {
  list-style: none;
  padding: 0;
}

nav ul li {
  display: inline;
  margin: 0 10px;
}

nav ul li a {
  color: #ffffff;
  text-decoration: none;
}

section {
  padding: 20px;
  margin: 20px 0;
  background: #ffffff;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

footer {
  text-align: center;
  padding: 10px 0;
  background: #35424a;
  color: #ffffff;
}document.getElementById("contactForm").addEventListener("submit", function (e) {
  e.preventDefault();
  const name = document.getElementById("name").value;
  const message = document.getElementById("message").value;

  alert(`谢谢您的留言, ${name}! 我们已收到您的信息: "${message}"`);
});const express = require('express');
const bodyParser = require('body-parser');
const app = express();

app.use(express.static('public'));
app.use(bodyParser.json());

app.post('/submit', (req, res) => {
  const { name, message } = req.body;
  console.log(`收到来自 ${name} 的信息: ${message}`);
  res.json({ status: 'success', message: '信息已收到！' });
});

const PORT = 3000;
app.listen(PORT, () => {
  console.log(`服务器已启动：http://localhost:${PORT}`);
});/project-folder
  ├── public/
  │   ├── index.html
  │   ├── style.css
  │   └── script.js
  ├── server.js
  ├── package.json
