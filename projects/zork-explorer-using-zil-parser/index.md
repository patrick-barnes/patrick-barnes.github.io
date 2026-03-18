---
layout: page
title: Zork Explorer using ZIL Parser
---

# Zork Explorer using ZIL Parser

## Background

I vividly remember the first time I saw a computer.

In 1985, my Uncle Mikey brought home an IBM 5150 and
showed me a game called Zork.

<div class="project-grid">
  <div class="project-card">
    <img
      src="/assets/images/ibm-5150.webp"
      alt="IBM 5150"
      class="project-thumb"
    />
    <h2>IBM 5150</h2>
    <p>My first computer</p>
    <p class="project-tags">
      <span>IBM 5150</span>
    </p>
  </div>
  <div class="project-card">
    <img
      src="/assets/images/zork-box-art.jpg"
      alt="Zork I Box Art"
      class="project-thumb"
    />
    <h2>Zork I</h2>
    <p>My first computer game</p>
    <p class="project-tags">
      <span>Zork</span>
    </p>
  </div>
  <div class="project-card">
    <img
      src="/assets/images/zork-gameplay.png"
      alt="Zork I Gameplay"
      class="project-thumb"
    />
    <h2>Zork I gameplay</h2>
    <p>What it's like to play</p>
    <p class="project-tags">
      <span>ZIL</span>
    </p>
  </div>
</div>

Infocom created a lot of games like these in the 1980s.
The most famous ones are the Zork trilogy and Enchanter trilogy.
The way they worked is, you (the player) type commands like:
- `open the mailbox`
- `attack the troll with the sword `
...and the game would carry out your action.

Parsing human language was a very impressive capability
for the computers in the 1980s because they were so limited!
The genius behind it is the ZIL programming language.

TODO:
- Screenshot of sample of ZIL program excerpt

## What I did

I wrote an app that:
- extends an open source ZIL parser
- translates syntaxes, rooms, objects, etc. to JSON
- provides a website to explore the internals of the game

TODO:
- Screenshots of various pages from the app

## Tech used
- ZIL computer language
- C#.NET for `zil-to-json` language parser
- JSON for metadata
- Angular 11 for `explore` web app

## Status
- Publicly available
- Reddit announcement: https://www.reddit.com/r/zork/comments/noiw7w/explore_zork_internals_from_your_browser/
- Zork Explorer web app: https://zork-playground.github.io/explore
- Source code in github:
  - `zil-to-json`: https://github.com/zork-playground/zil-to-json
  - JSON metadata: https://github.com/zork-playground/zil-to-json/tree/main/data/
  - `explore`: https://github.com/zork-playground/explore

## What This Demonstrates
- my interest in human linguistics
- my ability to learn esoteric technology
- my ability to make ancient tech modernly accessible
- simple web app development
