<!DOCTYPE html>
<html>
<head>
  <title>TopMediai Clone</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>TopMediai Tools</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="tools.html">Tools</a>
    </nav>
  </header>
  <main>
    <h2>Welcome to Your AI Tools Hub</h2>
    <p>This is a clone of TopMediai with Text to Speech, Voice Cloning, and more.</p>
    <a href="tools.html" class="button">Explore Tools</a>
  </main>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>AI Tools</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>AI Tools</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="tools.html">Tools</a>
    </nav>
  </header>
  <main>
    <ul class="tool-list">
      <li><a href="tts.html">Text to Speech</a></li>
      <li><a href="#">Voice Cloning (Coming Soon)</a></li>
      <li><a href="#">AI Music Generator (Coming Soon)</a></li>
    </ul>
  </main>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
  <title>Text to Speech</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Text to Speech</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="tools.html">Tools</a>
    </nav>
  </header>
  <main>
    <h2>Try Text to Speech</h2>
    <textarea id="inputText" rows="5" cols="40" placeholder="Type something..."></textarea><br>
    <button onclick="speak()">Speak</button>
  </main>

  <script>
    function speak() {
      const text = document.getElementById("inputText").value;
      const speech = new SpeechSynthesisUtterance(text);
      speech.lang = "en-US";
      window.speechSynthesis.speak(speech);
    }
  </script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: #f4f4f4;
}

header {
  background: #222;
  color: white;
  padding: 1rem;
  text-align: center;
}

nav a {
  margin: 0 1rem;
  color: white;
  text-decoration: none;
}

main {
  padding: 2rem;
  text-align: center;
}

.button {
  display: inline-block;
  padding: 1rem 2rem;
  background: #007BFF;
  color: white;
  text-decoration: none;
  border-radius: 5px;
}

.tool-list {
  list-style: none;
  padding: 0;
}

.tool-list li {
  margin: 1rem 0;
  font-size: 1.2rem;
}
