+++
title = "AI-Powered Diary"
date = "2025-11-14"
author = "Marco Szeidenleder"
description = "Building an AI-Powered Life Coach from Your Daily Voice Notes"
tags = ["automation", "coaching", "ai"]
+++



![](hero.jpg)



I've discovered something that feels genuinely transformative: using AI as my personal diary and life coach. What started as a simple automation experiment has become more insightful than any coaching session I've experienced.

## The Workflow

Every night, I spend 2-20 minutes recording my thoughts on my phone—what happened during the day, what's on my mind, challenges I'm facing, things I'm looking forward to. Just free-flowing audio captured in the moment.

Here's what happens then:

1. **Audio recording** on my phone
2. **Automatic transcription** using Whisper (via Replicate's API)
3. **Append to Google Docs** - every recording adds to the same continuously growing document
4. **Periodic sync** - I download the text file and upload it to a ChatGPT project that contains all my previous entries

That's it. Now I have an AI that knows my entire journey, my patterns, my challenges, and my aspirations.

## The Setup

As a programmer, I built this in Python and deployed it on Cloud Run, but you could easily accomplish the same thing using n8n or similar no-code tools. The key components are:

- **Whisper API** through Replicate for transcription
- **Google Docs API** for storage
- **ChatGPT Projects** for the AI analysis layer


## Why This Works So Well

Having an AI that knows my complete history is like having the world's most patient listener with perfect memory. I can ask questions like:

- "What patterns do you see in my challenges over the past three months?"
- "Based on what I've shared, what do you think I should focus on?"
- "What advice would you give me about this situation I'm facing?"

What excites me most is that we're barely scratching the surface of what's possible. This simple workflow—record, transcribe, analyze—is just the beginning. 