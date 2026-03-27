---
layout: page
title: Zork Explorer using ZIL Parser
---

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

## What I did

I wrote an app that:
- extends an open source ZIL parser
- translates syntaxes, rooms, objects, etc. to JSON
- provides a website to explore the internals of the game

### Create maps from room code

<div class="project-grid">
  <div class="project-card">
    <img
      src="/assets/images/zork-playground/zork-map-code.png"
      alt="ZIL code: West of House"
      class="project-thumb"
    />
    <h2>ZIL code: West of House</h2>
    <p>ZIL code snippet for defining a "room" in the game.</p>
  </div>
  <div class="project-card">
    <img
      src="/assets/images/zork-playground/zork-map.png"
      alt="Zork Map"
      class="project-thumb"
    />
    <h2>Zork Map</h2>
    <p>App shows the room and its adjoining rooms</p>
  </div>
</div>

### Explore syntaxes

<div class="project-grid">
  <div class="project-card">
    <img
      src="/assets/images/zork-playground/zork-syntaxes-code.png"
      alt="ZIL code: Syntaxes"
      class="project-thumb"
    />
    <h2>ZIL code: Syntaxes</h2>
    <p>ZIL code snippet for sentence structures supported.</p>
  </div>
  <div class="project-card">
    <img
      src="/assets/images/zork-playground/zork-syntaxes.png"
      alt="Zork Syntaxes"
      class="project-thumb"
    />
    <h2>Syntaxes</h2>
    <p>App shows which "sentence structures" cause which "verb routines" to be called.</p>
  </div>
</div>

### Explore objects like the sword

<div class="project-grid">
  <div class="project-card">
    <img
      src="/assets/images/zork-playground/zork-sword-code.png"
      alt="ZIL code: Sword Object"
      class="project-thumb"
    />
    <h2>ZIL code: Sword Object</h2>
    <p>ZIL code: Sword Object</p>
    <p class="project-tags">
      <span>ZIL code snippet for defining the sword object in the game.</span>
    </p>
  </div>
  <div class="project-card">
    <img
      src="/assets/images/zork-playground/zork-sword.png"
      alt="Zork Sword"
      class="project-thumb"
    />
    <h2>Sword</h2>
    <p>App shows the sword object and its characteristics.</p>
    <p>You can substitute "Glamdring" for sword!</p>
  </div>
</div>

## Tech used
- ZIL computer language
- C#.NET for `zil-to-json` language parser
- JSON for metadata
- Angular 11 for `explore` web app

## Status
- Publicly available: - <a href="https://zork-playground.github.io/explore">Zork Explorer web app</a>
  - <a href="https://www.reddit.com/r/zork/comments/noiw7w/explore_zork_internals_from_your_browser/">Reddit announcement</a>
- Source code in github:
  - `zil-to-json`: <a hreef="https://github.com/zork-playground/zil-to-json">https://github.com/zork-playground/zil-to-json</a>
  - JSON metadata: <a href="https://github.com/zork-playground/zil-to-json/tree/main/data/">https://github.com/zork-playground/zil-to-json/tree/main/data/</a>
  - `explore` web app: <a href="https://github.com/zork-playground/explore">https://github.com/zork-playground/explore</a>

## What This Demonstrates
- my interest in human linguistics
- my ability to learn esoteric technology
- my ability to make ancient tech modernly accessible
- simple web app development
