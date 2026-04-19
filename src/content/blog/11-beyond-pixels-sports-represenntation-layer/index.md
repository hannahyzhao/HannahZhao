---
title: "Beyond Pixels: Building the Sports Representation Layer for the Future of Athletic AI"
summary: "Why the real moat in sports AI is not the model itself, but the representation layer that transforms raw video into structured athletic understanding."
date: "Apr 20 2026"
draft: false
tags:
  - AI
  - Computer Vision
  - Startup
---

### Introduction

Recently, while building elevenset, I’ve been revisiting parts of Stanford’s CS231n: *Deep Learning for Computer Vision*.

This is not an academic exercise. It is a strategic necessity.

Moving from computer vision research to a real production sports product requires a fundamental shift in how we think about data, architecture, and success. In this post, I want to share the technical insights and architectural philosophy shaping our development — from why we prioritize pipelines over models to the challenges of temporal sequence modeling in tennis.

---

## 1. Representation > Model

One of the most important lessons from computer vision is that the hardest problem in AI is not choosing the right model. It is deciding how to represent the data.

In the startup world, pulling a state-of-the-art model from an open-source toolbox is becoming a commodity. The real engineering moat is built in the representation layer.

At elevenset, I do not think of the company as a “video model company.” I see it as building a system that transforms raw athletic footage into a structured hierarchy of events:

**Raw Video → 2D Keypoints → 3D Motion → Temporal Sequences → Actionable Insights**

That layer of structured understanding is where the product becomes more than just detection. It becomes useful.

---

## 2. The Real Engineering Moat Is in the Pipeline

Technical founders often fall in love with models. But in production, robustness usually lives in the pipeline.

A good example is rally detection. Instead of relying only on vision, which can become brittle under different lighting conditions or camera angles, we use a hybrid multi-modal approach. Audio signals can help identify the acoustic signature of ball contact, which strengthens the reliability of visual detections.

This is one of the most important product lessons I’ve learned:

> Do not optimize the model when the real problem is the representation and pipeline design.

A better model can improve a benchmark. A better pipeline can improve a real user experience.

---

## 3. Video Is a Sequence, Not a Stack of Frames

The biggest technical challenge in sports AI is moving from static recognition to temporal understanding.

A forehand is not a single image. It is a sequence across time: setup, swing path, contact, and follow-through.

This is where frame-based classification reaches a limit.  
Frame sampling is not the same as understanding motion.

To solve this, sequence modeling becomes essential. Instead of asking, “What is happening in this frame?”, the better question is:

**What pattern is unfolding over time?**

That shift matters because sports are not made of isolated poses. They are made of transitions, timing, and momentum.

---

## 4. Why Temporal Modeling Matters

Temporal models allow the system to retain information about what happened before the key action. This is especially important in tennis, where the quality of a shot depends not only on the moment of contact, but also on the movement leading into it.

The more I build in this space, the clearer it becomes that sports intelligence requires memory.

Not memory in the product sense, but memory in the modeling sense — a way for the system to carry state across time and understand motion as a process rather than a snapshot.

This is also why I’m increasingly interested in building systems with stronger inductive bias from the physical world. Generic computer vision tools can only go so far. To understand sports well, AI needs more than pattern matching. It needs structure, timing, and eventually some understanding of force, rotation, and intent.

---

## 5. Moving Toward 3D Motion Understanding

The next step is moving from 2D keypoints to 3D motion modeling.

Flat images can capture position, but they miss critical dimensions of movement such as body rotation, balance, and weight transfer. In sports, those missing dimensions are often exactly what matters.

A more complete system needs to reconstruct motion in space, not just identify joints on a screen. This is part of why I’m interested in digital twin systems and physically grounded representations. If the goal is real athletic understanding, then 3D motion is not just a nice-to-have. It becomes foundational.

---

## 6. From Detection to Skill Understanding

What matters most is not whether the AI can label a hundred shots correctly.

What matters is whether it can help a player improve.

Academic metrics like accuracy and loss are useful, but in a real product they are only proxy metrics. The true evaluation function is much simpler:

**Did the player actually get better?**

If a system detects movement but fails to help the user improve timing, consistency, or body mechanics, then the product has not truly succeeded.

That idea keeps shaping how I think about the future of elevenset. The goal is not just recognition. It is meaningful feedback.

---

## 7. Building Beyond Vision

I think the future of sports AI is not just visual recognition. It is structured understanding of physical skill.

That means building systems that connect:
- perception,
- timing,
- motion,
- and actionable output.

This is why I care so much about representation. It sits between the raw sensory world and human improvement. It is the layer that turns pixels into intelligence.

And in the long run, I believe this is where the real moat is built.

---

## Closing Thoughts

Building AI for sports has made one thing very clear to me:

The breakthrough rarely comes from swapping one model for another.

It comes from designing a better representation of reality.

That is the deeper challenge — and also the more interesting one.

We are moving beyond video understanding as classification, toward a richer system that models motion, sequence, and skill. For me, that is where sports AI starts to become truly meaningful.

---

*Published by Hannah Zhao*