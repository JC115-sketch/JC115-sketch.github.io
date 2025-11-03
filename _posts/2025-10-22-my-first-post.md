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
<style>
  body {
    cursor: url('/assets/dragon_scimitar.png') 10 28, auto;
  }
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
    font-family: 'Trebuchet MS', sans-serif;
  }
</style>

<div class="demo-area">
  Move your cursor here 🐉
</div>
