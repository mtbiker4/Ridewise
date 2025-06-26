<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>RideWise: The Ultimate Biking Hub</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f0f4f2;
      color: #333;
    }
    header {
      background-color: #2b4c3f;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    nav {
      display: flex;
      background: #406857;
      padding: 0.5rem;
      justify-content: center;
      gap: 2rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    main {
      max-width: 1000px;
      margin: auto;
      padding: 2rem;
    }
    section {
      margin-bottom: 3rem;
    }
    h2 {
      color: #2b4c3f;
      border-bottom: 2px solid #ccc;
      padding-bottom: 0.5rem;
    }
    ul {
      line-height: 1.8;
    }
    footer {
      background: #2b4c3f;
      color: white;
      text-align: center;
      padding: 1rem;
    }

    /* Chatbot styling */
    #chatbot {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 320px;
      height: 420px;
      background: white;
      border: 1px solid #aaa;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
      display: flex;
      flex-direction: column;
      z-index: 999;
      font-family: Arial, sans-serif;
    }
    #chatbot-header {
      background: #2b4c3f;
      color: white;
      padding: 10px;
      text-align: center;
      font-weight: bold;
      border-radius: 10px 10px 0 0;
      user-select: none;
    }
    #chat-log {
      flex-grow: 1;
      overflow-y: auto;
      padding: 10px;
      background: #fff;
      border-bottom: 1px solid #ccc;
      font-size: 14px;
    }
    #chat-log p {
      margin: 5px 0;
    }
    #chat-log p strong {
      color: #2b4c3f;
    }
    #user-input {
      border: none;
      border-top: 1px solid #ccc;
      padding: 10px;
      resize: none;
      font-size: 14px;
      outline: none;
      width: calc(100% - 80px);
      box-sizing: border-box;
    }
    #chat-controls {
      display: flex;
      border-top: 1px solid #ccc;
    }
    #send-btn {
      width: 80px;
      background: #2b4c3f;
      color: white;
      border: none;
      cursor: pointer;
      font-weight: bold;
      transition: background 0.3s ease;
    }
    #send-btn:hover {
      background: #3a6653;
    }
  </style>
</head>
<body>

<header>
  <h1>RideWise: The Ultimate Biking Hub</h1>
  <p>Your all-in-one resource for biking mastery, gear, safety, and exploration</p>
</header>

<nav>
  <a href="#skills">Skills</a>
  <a href="#maintenance">Maintenance</a>
  <a href="#gear">Gear</a>
  <a href="#trails">Trails</a>
  <a href="#training">Training</a>
  <a href="#safety">Safety</a>
  <a href="#subscribe">Subscribe</a>
</nav>

<main>
  <section id="skills">
    <h2>Skills & Techniques</h2>
    <ul>
      <li><a href="https://www.mbr.co.uk/how-to/skills" target="_blank" rel="noopener noreferrer">Basic and advanced MTB skills</a></li>
      <li><a href="https://www.bikeradar.com/advice/skills/how-to-descend-on-a-mountain-bike/" target="_blank" rel="noopener noreferrer">Descending techniques</a></li>
      <li><a href="https://www.youtube.com/watch?v=jr0f41Mg9rE" target="_blank" rel="noopener noreferrer">Manuals & Wheelies video</a></li>
    </ul>
  </section>

  <section id="maintenance">
    <h2>Maintenance & Repair</h2>
    <ul>
      <li><a href="https://www.rei.com/learn/expert-advice/bike-maintenance.html" target="_blank" rel="noopener noreferrer">Bike maintenance guide by REI</a></li>
      <li><a href="https://www.pinkbike.com/news/how-to-bleed-your-disc-brakes.html" target="_blank" rel="noopener noreferrer">Brake bleeding guide</a></li>
    </ul>
  </section>

  <section id="gear">
    <h2>Gear Guide</h2>
    <ul>
      <li><a href="https://www.bicycling.com/bikes-gear/a20048493/best-mountain-bikes/" target="_blank" rel="noopener noreferrer">Top mountain bikes</a></li>
      <li><a href="https://www.outdoorgearlab.com/topics/biking/best-mountain-bike-helmet" target="_blank" rel="noopener noreferrer">Best MTB helmets</a></li>
    </ul>
  </section>

  <section id="trails">
    <h2>Famous Trails Around the World</h2>
    <ul>
      <li><a href="https://www.whistlerblackcomb.com/explore-the-resort/activities-and-events/whistler-mountain-bike-park.aspx" target="_blank" rel="noopener noreferrer">Whistler Bike Park</a></li>
      <li><a href="https://utah.com/moab/slickrock-trail" target="_blank" rel="noopener noreferrer">Slickrock Trail, Utah</a></li>
    </ul>
  </section>

  <section id="training">
    <h2>Training & Performance</h2>
    <ul>
      <li><a href="https://www.trainingpeaks.com/blog/how-to-train-for-mountain-bike-racing/" target="_blank" rel="noopener noreferrer">MTB training plans</a></li>
      <li><a href="https://www.trainerroad.com/blog/strength-training-for-mountain-bikers/" target="_blank" rel="noopener noreferrer">Strength for mountain bikers</a></li>
    </ul>
  </section>

  <section id="safety">
    <h2>Safety & Best Practices</h2>
    <ul>
      <li><a href="https://www.imba.com/ride/imba-rules-of-the-trail" target="_blank" rel="noopener noreferrer">IMBA Trail Etiquette</a></li>
      <li><a href="https://www.sram.com/en/life/stories/first-aid-mountain-bike" target="_blank" rel="noopener noreferrer">First Aid for Riders</a></li>
    </ul>
  </section>

  <section id="subscribe">
    <h2>Subscribe for Pro Tips & Access</h2>
    <p>Join our RideWise PRO membership to get exclusive content, downloadable guides, and early access to new features.</p>
    <ul>
      <li><strong>Free:</strong> Access all public articles and chatbot help.</li>
      <li><strong>Pro ($4.99/month):</strong> Unlock over 1000 pro-level biking tips, videos, downloads, and advanced chatbot answers.</li>
    </ul>
    <form action="https://formsubmit.co/kpecks@gmail.com" method="POST" target="_blank">
      <label for="email">Email:</label><br />
      <input type="email" name="email" required placeholder="Enter your email" />
      <button type="submit">Subscribe</button>
    </form>
  </section>
</main>

<footer>
  <p>&copy; 2025 RideWise. Built for riders, by riders. Contact: <a style="color: #ffa;" href="mailto:kpecks@gmail.com">kpecks@gmail.com</a></p>
</footer>

<!-- Chatbot using OpenAI API -->
<div id="chatbot">
  <div id="chatbot-header">RideWise AI Chatbot</div>
  <div id="chat-log"></div>
  <div id="chat-controls">
    <textarea id="user-input" placeholder="Ask me anything about biking..."></textarea>
    <button id="send-btn">Send</button>
  </div>
</div>

<script>
  const OPENAI_API_KEY = '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
'; // Replace with your OpenAI API Key
  const chatLog = document.getElementById('chat-log');
  const input = document.getElementById('user-input');
  const sendBtn = document.getElementById('send-btn');

  function appendMessage(sender, text) {
    const p = document.createElement('p');
    p.innerHTML = '<strong>' + sender + ':</strong> ' + text;
    chatLog.appendChild(p);
    chatLog.scrollTop = chatLog.scrollHeight;
  }

  async function sendMessage() {
    const userText = input.value.trim();
    if (!userText) return;
    appendMessage('You', userText);
    input.value = '';
    sendBtn.disabled = true;
    sendBtn.textContent = '...';

    try {
      const response = await fetch('https://api.openai.com/v1/chat/completions', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
          'Authorization': 'Bearer ' + OPENAI_API_KEY
,
        },
        body: JSON.stringify({
          model: 'gpt-3.5-turbo',
          messages: [
            { role: 'system', content: 'You are RideWiseGPT, a biking expert who helps riders learn skills, trails, gear, and safety. Be friendly, detailed, and helpful.' },
            { role: 'user', content: userText }
          ],
        }),
      });

      const data = await response.json();
      if (data.choices && data.choices.length > 0) {
        appendMessage('RideWiseBot', data.choices[0].message.content);
      } else {
        appendMessage('RideWiseBot', 'Sorry, I couldn\'t get an answer. Please try again.');
      }
    } catch (error) {
      appendMessage('RideWiseBot', 'Error communicating with the server.');
    } finally {
      sendBtn.disabled = false;
      sendBtn.textContent = 'Send';
    }
  }

  sendBtn.addEventListener('click', sendMessage);
  input.addEventListener('keydown', (e) => {
    if (e.key === 'Enter' && !e.shiftKey) {
      e.preventDefault();
      sendMessage();
    }
  });
</script>

</body>
</html>

