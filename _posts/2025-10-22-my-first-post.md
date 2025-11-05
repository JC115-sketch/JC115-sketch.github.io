---
layout: post
title: "Let's make a few projects from my childhood"
date: 2025-10-22
---
It is a rainy day outside, so let's continue working on our journey of programming the first things that ever made me say "how did they do that".

![The Vicious Curved Sword in Question]()

My journey making the classic dragon scimitar cursor executable, of course it all started here...

A little javascript/html attempt:

<!-- 🐉 Dragon Scimitar Cursor Demo -->
<!-- 🐉 Dragon Scimitar Cursor Toggle Demo -->
<style>
  .demo-area {
    width: 100%;
    height: 300px;
    background: radial-gradient(circle at center, #1a1a1a, #000);
    border-radius: 10px;
    box-shadow: inset 0 0 10px #222;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    font-family: 'Trebuchet MS', sans-serif;
  }

  .cursor-button {
    margin-top: 1rem;
    padding: 0.5rem 1rem;
    border: none;
    background: #e63946;
    color: white;
    border-radius: 6px;
    cursor: pointer;
    transition: background 0.2s;
  }

  .cursor-button:hover {
    background: #ff5555;
  }
</style>

<div class="demo-area">
  <p>Click below to activate the Dragon Scimitar cursor </p>
  <button id="activate" class="cursor-button">Activate Cursor</button>
  <button id="restore" class="cursor-button" style="display:none;">Restore Default</button>
</div>

<script>
  const activateBtn = document.getElementById('activate');
  const restoreBtn = document.getElementById('restore');
  const scimitarURL = '/assets/dscim_cursor.png'; // adjust if in subfolder

  activateBtn.addEventListener('click', () => {
    document.body.style.cursor = `url(${scimitarURL}) 10 28, auto`;
    activateBtn.style.display = 'none';
    restoreBtn.style.display = 'inline-block';
  });

  restoreBtn.addEventListener('click', () => {
    document.body.style.cursor = 'auto';
    restoreBtn.style.display = 'none';
    activateBtn.style.display = 'inline-block';
  });
</script>

Of course, the real one changed the cursor system wide. I am legitmately curious if there was a built in way to revert back to the default Windows cursor in the most available dragon scimitar cursor program circa 2010 or so. Well fear not! I have created my own. It's totally safe of course, just a joke way of making a replica of a 'Java drive by' or drive by download program that got at least one kid at every middle school in the US and Britain into some sort of trouble. 

<p>
  <a class="btn-demo" href="/fake-installer.html" target="_blank" rel="noopener">
    But it was from dragonscimitarcursorofficial.com!! 
  </a>
</p>

<style>
  .btn-demo {
    display:inline-block;
    padding:10px 14px;
    background:#e63946;
    color:white;
    border-radius:6px;
    text-decoration:none;
    font-weight:600;
  }
  .btn-demo:hover { opacity:0.95; }
</style>
