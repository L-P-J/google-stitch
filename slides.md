---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Google Stitch Presentation
  Revolutionizing UI/UX design through intelligent automation

  From concept to functional interfaces in mintues.
# apply UnoCSS classes to the current slide
class: 'text-center bg-gradient-to-br from-blue-900 via-purple-900 to-indigo-900' 
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
colorSchema: dark
fonts:
  sans: 'Inter'
  serif: 'Crimson Pro'
  mono: 'JetBrains Mono'
seoMeta:
  ogImage: auto 
---

# Stitch

AI-Powered UI Generation for Mobile & Web

<div> becky </div>

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
   <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# What is Google Stitch

- Google Stitch is a tool announced at Google I/O 2025 that automatically generates user interfaces (UIs) for mobile and web applications.
  - Generates fronts-end UI designs and code from text or image prompts
  - Supports both mobile (Android, ios) and web platforms

<img src='' class='mx-auto mt-2 max-h-70'>


---
transition: slide-up
level: 2
---

# How Stitch AI works

Powered by Google's Gemini 2.5 Pro and Gemini 2.5 Flash, Stitch AI can understand and process text, image and visual structures.

### Generation Process

<div v-click class='flex flex-col items-center py-5'>
- Intent Parsing:
The AI analyzes the input (prompt or sketch) to understand the user's intent, context, and required components.
</div>
<div v-click class='flex flex-col items-center'>
- code and Design Rendering:
This abstract structure is then translated into specific front-end code (such as HTML/TAILWIND) and visual design, applying design principles, component hierarchy, and style.
</div>
---
class: 'flex flex-col items-center justify-center h-full'
---

# Mode

<div class='flex items-start justify-center gap-16 mt-8 w-full'>

<div v-click class='flex flex-col items-center'>

### Standard Mode

<div class='text-sm space-y-2 mt-4'>

- Model: Gemini 2.5 Flash
- Input: Primarily based on text prompts.
- Key Feature: Supports "Copy to Figma."
- Use Cases: Best for rapid ideation and iteration, as well as workflows that require designs to be delivered to Figma for optimization.
</div>
</div>

<div v-click class='flex flex-col items-center'>

### Experimental Mode
<div class='text-sm space-y-2 mt-4'>

- Model: Gemini 2.5 Pro
- Input: Supports multimodal input, including uploading hand-drawn wireframes, sketches, and screenshots.
- Key Limitation: "Copy to Figma" functionality is currently unavailable.
- Use Cases: Ideal for transforming existing visual concepts into refined digital designs and code.
</div>
</div>

</div>

---
layout: two-cols
layoutClass: gap-16
---

# Using

<img src='' class=''>

---
class: 'grid place-content-center text-center h-full'
---

# Thank You
Google Stitch -Making design ideation fast and easy

<div class='mt-8 text-xl'>
Questions & Discussion
</div>
