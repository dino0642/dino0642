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
</html>
