---
layout: post
title: "Let's make a few projects from my childhood"
date: 2025-10-22
---
It is a rainy day outside, so let's continue working on our journey of programming the first things that ever made me say "how did they do that".

![The Vicious Curved Sword in Question]()

My journey making the classic dragon scimitar cursor executable, and the wavy and flashing text generator program...

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
  const scimitarURL = '/assets/dscim_img.png'; // adjust if in subfolder

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

