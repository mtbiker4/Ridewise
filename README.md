<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>RideWise Mountain Biking Hub</title>
<style>
  :root {
    --primary-color: #1b3a2d;
    --accent-color: #f95c22;
    --bg-color: #f0f4f1;
    --text-color: #333;
    --header-bg: var(--primary-color);
    --header-text: white;
  }
  body {
    margin: 0; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: var(--bg-color); color: var(--text-color);
    display: flex; flex-direction: column; min-height: 100vh;
  }
  header {
    background: var(--header-bg);
    color: var(--header-text);
    padding: 1rem 2rem;
    text-align: center;
    box-shadow: 0 3px 8px rgba(0,0,0,0.3);
  }
  header h1 {
    margin: 0; font-weight: 700;
  }
  nav {
    background: #2e5d43;
    padding: 0.5rem 2rem;
    display: flex;
    gap: 1.5rem;
    justify-content: center;
  }
  nav a {
    color: white;
    text-decoration: none;
    font-weight: 600;
    font-size: 1rem;
  }
  nav a:hover {
    color: var(--accent-color);
  }
  main {
    flex: 1;
    max-width: 960px;
    margin: 2rem auto;
    padding: 0 1rem;
  }
  article {
    background: white;
    padding: 1.5rem 2rem;
    margin-bottom: 2rem;
    border-radius: 10px;
    box-shadow: 0 2px 8px rgb(0 0 0 / 0.1);
  }
  article h2 {
    margin-top: 0;
    color: var(--primary-color);
  }
  article p {
    line-height: 1.6;
  }
  footer {
    background: var(--header-bg);
    color: var(--header-text);
    text-align: center;
    padding: 1rem 2rem;
  }

  /* Chatbot styles */
  #chatbot-container {
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 320px;
    max-width: 90vw;
    font-family: Arial, sans-serif;
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    border-radius: 12px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    background: white;
    transition: transform 0.3s ease-in-out;
    transform: translateY(0);
  }
  #chatbot-header {
    background: var(--primary-color);
    color: white;
    padding: 0.75rem 1rem;
    cursor: pointer;
    user-select: none;
  }
  #chatbot-messages {
    flex: 1;
    padding: 1rem;
    overflow-y: auto;
    height: 280px;
    background: #e9f2eb;
  }
  .chatbot-message {
    margin-bottom: 1rem;
    padding: 0.5rem 0.75rem;
    border-radius: 12px;
    max-width: 80%;
    clear: both;
    font-size: 0.9rem;
    line-height: 1.3;
  }
  .chatbot-message.user {
    background: var(--accent-color);
    color: white;
    float: right;
    border-bottom-right-radius: 2px;
  }
  .chatbot-message.bot {
    background: #d1e7d9;
    color: #1b3a2d;
    float: left;
    border-bottom-left-radius: 2px;
  }
  #chatbot-input-container {
    display: flex;
    border-top: 1px solid #ccc;
  }
  #chatbot-input {
    flex: 1;
    border: none;
    padding: 0.75rem 1rem;
    font-size: 1rem;
    outline: none;
  }
  #chatbot-send {
    background: var(--accent-color);
    border: none;
    color: white;
    padding: 0 1.2rem;
    cursor: pointer;
    font-size: 1.1rem;
    font-weight: bold;
    transition: background 0.3s;
  }
  #chatbot-send:hover {
    background: #d44705;
  }
  #chatbot-container.minimized #chatbot-messages,
  #chatbot-container.minimized #chatbot-input-container {
    display: none;
  }
  #chatbot-container.minimized {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    bottom: 20px;
    right: 20px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    cursor: pointer;
  }
  #chatbot-container.minimized #chatbot-header {
    padding: 0;
    text-align: center;
    line-height: 50px;
  }
</style>
</head>
<body>

<header>
  <h1>RideWise Mountain Biking Hub</h1>
  <p>Your ultimate guide for mountain biking tips, gear, and trails</p>
</header>

<nav>
  <a href="#tips">Tips</a>
  <a href="#gear">Gear</a>
  <a href="#trails">Trails</a>
  <a href="#safety">Safety</a>
  <a href="#maintenance">Maintenance</a>
</nav>

<main>
  <article id="tips">
    <h2>Top Mountain Biking Tips</h2>
    <p>Mountain biking is thrilling but challenging. Here are some essential tips to improve your ride and stay safe:</p>
    <ul>
      <li>Wear a properly fitted helmet and protective gear.</li>
      <li>Keep your weight centered and stay relaxed on the bike.</li>
      <li>Look ahead on the trail to anticipate obstacles.</li>
      <li>Practice braking evenly and avoid skidding.</li>
      <li>Ride within your skill level and gradually push your limits.</li>
    </ul>
  </article>

  <article id="gear">
    <h2>Must-Have Mountain Biking Gear</h2>
    <p>Choosing the right gear can make or break your ride experience. Consider these essentials:</p>
    <ul>
      <li><strong>Helmet:</strong> Lightweight, well-ventilated, and safety-certified.</li>
      <li><strong>Gloves:</strong> For grip and protection.</li>
      <li><strong>Hydration pack:</strong> Stay hydrated on long rides.</li>
      <li><strong>Clipless pedals and shoes:</strong> For better control and efficiency.</li>
      <li><strong>Multi-tool kit:</strong> For quick repairs on the trail.</li>
    </ul>
  </article>

  <article id="trails">
    <h2>Best Mountain Biking Trails</h2>
    <p>Explore some of the most exciting trails for riders of all levels:</p>
    <ul>
      <li><strong>Moab, Utah:</strong> Famous for slickrock and stunning views.</li>
      <li><strong>Whistler, Canada:</strong> World-renowned trail networks and terrain parks.</li>
      <li><strong>Finale Ligure, Italy:</strong> Beautiful Mediterranean scenery and technical descents.</li>
      <li><strong>Downieville, California:</strong> Epic downhill and classic cross-country trails.</li>
      <li><strong>Forest of Dean, UK:</strong> Lush forests with well-maintained trails.</li>
    </ul>
  </article>

  <article id="safety">
    <h2>Mountain Biking Safety Tips</h2>
    <p>Your safety comes first! Always keep these in mind:</p>
    <ul>
      <li>Check your bike’s brakes, tires, and chain before each ride.</li>
      <li>Ride with a buddy or tell someone your planned route.</li>
      <li>Carry a basic first aid kit and know how to use it.</li>
      <li>Respect trail rules and wildlife.</li>
      <li>Be prepared for changing weather conditions.</li>
    </ul>
  </article>

  <article id="maintenance">
    <h2>Basic Bike Maintenance</h2>
    <p>Keep your bike in top shape with regular maintenance:</p>
    <ul>
      <li>Clean and lubricate your chain regularly.</li>
      <li>Check tire pressure and inflate to recommended levels.</li>
      <li>Inspect brakes for wear and proper function.</li>
      <li>Tighten bolts and check headset play.</li>
      <li>Service suspension components periodically.</li>
    </ul>
  </article>
</main>

<footer>
  <p>Contact: <a href="mailto:kpecks@gmail.com" style="color: var(--accent-color)">kpecks@gmail.com</a> | &copy; 2025 RideWise</p>
</footer>

<!-- Chatbot -->
<div id="chatbot-container" class="minimized" title="Chat with RideWise bot!">
  <div id="chatbot-header">💬</div>
  <div id="chatbot-messages"></div>
  <div id="chatbot-input-container">
    <input id="chatbot-input" type="text" placeholder="Ask me anything about mountain biking..." />
    <button id="chatbot-send">&#9658;</button>
  </div>
</div>

<script>
  const chatbot = document.getElementById('chatbot-container');
  const header = document.getElementById('chatbot-header');
  const messages = document.getElementById('chatbot-messages');
  const input = document.getElementById('chatbot-input');
  const sendBtn = document.getElementById('chatbot-send');

  // Toggle chatbot open/close
  header.addEventListener('click', () => {
    chatbot.classList.toggle('minimized');
  });

  // Basic preset responses for demo
  const responses = {
    "hello": "Hey there! How can I help you with your mountain biking questions?",
    "hi": "Hi! Ask me anything about biking tips, gear, or trails.",
    "help": "Sure! I can answer questions about biking safety, gear recommendations, and trail suggestions.",
    "helmet": "Always wear a properly fitting helmet! Safety first.",
    "trails": "Some great trails are Moab, Whistler, and Downieville. What region are you interested in?",
    "maintenance": "Keep your chain clean and lubricated, and check your tire pressure regularly.",
    "thanks": "You’re welcome! Ride safe!",
    "default": "Sorry, I’m still learning. Could you please ask something else?"
  };

  function appendMessage(text, sender) {
    const msg = document.createElement('div');
    msg.classList.add('chatbot-message', sender);
    msg.textContent = text;
    messages.appendChild(msg);
    messages.scrollTop = messages.scrollHeight;
  }

  function getResponse(inputText) {
    const text = inputText.toLowerCase();
    for (const key in responses) {
      if (text.includes(key)) {
        return responses[key];
      }
    }
    return responses["default"];
  }

  function sendMessage() {
    const userText = input.value.trim();
    if (!userText) return;
    appendMessage(userText, 'user');
    input.value = '';
    setTimeout(() => {
      appendMessage(getResponse(userText), 'bot');
    }, 700);
  }

  sendBtn.addEventListener('click', sendMessage);
  input.addEventListener('keydown', e => {
    if (e.key === 'Enter') sendMessage();
  });
</script>

</body>
</html>
