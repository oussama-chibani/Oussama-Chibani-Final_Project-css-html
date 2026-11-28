# 404: Voice Not Found

*When your voice is silenced online, we help you be heard.*

## Overview

In web terminology, **404** means something is missing or unreachable. **404: Voice Not Found** borrows that idea to address a real issue in Morocco: people—especially women and girls—getting pushed into silence by online harassment, blackmail, fake accounts, or image-based abuse.

This project is a responsive, 3-page front-end web application built with **HTML5**, **CSS3**, and **Tailwind CSS v4**. Instead of overwhelming visitors with legal jargon or intimidating warnings, the site walks users calmly through three stages: understanding digital violence, recognizing what is happening to them, and taking practical steps at their own pace.

---

## Context in Morocco

The content and guidance inside the site are grounded in the current reality of digital violence in Morocco:

* **Scale of the issue:** According to Morocco's High Commission for Planning (**HCP**), nearly **1.5 million women** in Morocco experience cyber-violence, accounting for **19%** of all violence against women. Younger groups are hit hardest: **34%** among girls aged 15–19 and **28%** among women aged 20–24.
* **The reporting gap:** Many victims hesitate to speak up out of fear of judgment, stigma, or having private material exposed. Others block the abuser immediately without saving URLs, dates, or screenshots first—losing crucial proof.
* **Legal & support framework:** Morocco's **Law 103.13** (on combating violence against women) established dedicated support units inside courts, police stations, and the Royal Gendarmerie, alongside official cybercrime reporting via **E-BLAGH** (DGSN) and 24/7 listening support via **Kolona Maak (8350)**.

**404: Voice Not Found** brings these scattered steps and Moroccan resources together in one calm, easy-to-navigate place.

---

## Page-by-Page Walkthrough

### 1. Home (`index.html`)
Introduces the platform and sets a safe, non-judgmental tone from the first screen:
* **Hero section** framing the mission with direct entry points (*I Need Help* and *Learn More*).
* **What is digital violence?** section defining online abuse clearly and plainly.
* **How we can Support you** 3-card overview (*Understand*, *Take Action*, *Find Support*).
* **Support in Morocco** callout banner leading visitors toward local resources.

### 2. I Need Help (`public/pages/I-need-help.html`)
Helps visitors put a name to what they are experiencing without feeling blamed:
* **Recognize the Signs** grid breaking digital abuse into **6 clear categories**:
  1. Online Harassment
  2. Cyberstalking
  3. Threats & Blackmail
  4. Impersonation
  5. Image-Based Abuse
  6. Account Hacking
* **Urgent Support CTA** directing visitors straight to Moroccan support channels.
* **Reassurance banner** (*"You are not alone. What you're feeling is valid, and support is available."*).

### 3. Take Action (`public/pages/take-Action.html`)
Built for practical, step-by-step action at the user's own pace:
* **Protect yourself online** — Six interactive nested accordions built with native HTML `<details>` and `<summary>` tags (zero JavaScript needed). Each category opens into two color-coded sub-panels:
  * **What You Can Do** (soft green): immediate steps like preserving evidence before blocking, turning off location sharing, enabling 2FA, or hashing intimate images privately.
  * **Specialized Help in Morocco** (warm orange): matching the exact issue to the right local or digital channel.
* **Confidential Incident Report & Privacy Card** — A two-part section pairing a clean incident form (*Share What Happened*) with a dark reassurance card (`PRIVATE & CONFIDENTIAL`) that emphasizes anonymity, user control, and immediate phone support via **Kolona Maak (8350)**.


---

## Design & Tech Stack

### Visual Choices
Most safety sites rely on harsh reds and heavy warning banners that can spike anxiety. **404: Voice Not Found** intentionally uses a warm, grounded palette to keep visitors calm while they read or submit a report:

* **Page Canvas:** `#fdf6ef` (warm off-white)
* **Primary Accent:** `#F47732` / `#EE782E` (hopeful warm orange)
* **Dark Contrast Cards & Footer:** `#2C2625` / `#2a2629` (deep charcoal with `#E6DFDA` body text)
* **Typography:** Editorial serif headings paired with clean sans-serif body copy

### Technical Stack
* **HTML5** — Semantic multi-page layout and native `<details>`/`<summary>` interactive accordions
* **Tailwind CSS v4** — Compiled via Tailwind CLI (`@import "tailwindcss";` in `input.css` -> `output.css`)
* **Custom CSS Media Queries** — Handled hero background images and mobile positioning via `@media (max-width: 768px)`
* **Responsive Strategy** — Desktop-first layout adapted cleanly for tablets and phones using Tailwind `max-md:` utilities, Flex, and CSS Grid
* **Inline SVGs** — Custom lightweight icons embedded directly without external icon library overhead

---

## Folder Map

```text
Oussama-Chibani-Final_Project-css-html/
├── index.html                      
├── README.md                       
└── public/
    ├── css/
    │   ├── input.css               
    │   └── output.css              
    ├── images/
    │   ├── 404-voice.png           
    │   ├── Hopeful.png             
    │   ├── laptop-sec-2.png        
    │   ├── banner-img.png          
    │   ├── sec-hero-pg2.jpg        
    │   ├── bg-last-sec.jpg         
    │   └── sec-hero-P3.jpg        
    └── pages/
        ├── I-need-help.html       
        └── take-Action.html        
```