# bigpickleballs.com
Pickleball content network built on WordPress — court directory, social platform, gear blog, and hosting review site. Powered by the Anthropic API, Make.com automation, and Python data pipelines. Operated by Gregory de la Cruz, author of 25+ pickleball books.


# Big Pickle Balls — Site Network

>Honest, deeply researched pickleball content. No corporate fluff. No paid reviews pretending to be unbiased.

---

## Overview

This repository documents the architecture, tooling, and content systems behind the **Big Pickle Balls network** — a portfolio of interconnected pickleball and web publishing properties built and operated by [Gregory de la Cruz](https://gregorydelacruz.com).

---

## The Network

| Site | Purpose | Platform |
|------|---------|----------|
| [BigPickleBalls.com](https://bigpickleballs.com) | Pickleball gear, strategy, court culture, and content hub | WordPress |
| [USAPickleballs.com](https://usapickleballs.com) | National pickleball court directory — all 50 states | WordPress |
| [DinkerDates.com](https://dinkerdates.com) | America's dedicated pickleball social network | pH7Builder |
| [BaobabHosting.com](https://baobabhosting.com) | WordPress hosting reviews and comparisons | WordPress |

---

## Tech Stack

### Core
- **CMS:** WordPress (all sites) / pH7Builder (DinkerDates)
- **Theme:** Neve Pro
- **Hosting:** InterServer (primary), with DirectAdmin on DinkerDates
- **SEO:** AIOSEO Pro (migrated from Rank Math Pro across full network)

### Plugins & Tools
- **WPCode Pro** — code injection, author bio box deployment network-wide
- **WP Go Maps** — court map integration with custom infowindow badges (USAPickleballs)
- **Make.com** — automation pipelines (content distribution, RSS to social)
- **Google Tag Manager + GA4** — analytics (cleaned up per-site)
- **Neve Pro** — theme across all WordPress properties

### Content & Automation
- **Anthropic API** — bulk content generation via PromptBatch/Overnight Studio tool
- **Google Colab** — Python pipelines for court data processing (BeautifulSoup, CSV import)
- **Make.com + Airtable** — content generation pipeline (BaobabHosting, in active development)
- **AIOSEO Pro** — schema markup, sitemap, per-site SEO configuration

### Performance
- **WP Rocket** — caching and performance optimization
- PageSpeed optimization completed on BigPickleBalls.com (significant mobile score improvement)

---

## Site Architecture — USAPickleballs.com

The court directory uses a JavaScript-driven HTML template system:

- **50-state page architecture** — single template with one variable swap per state
- **City-level pages** — real court data sourced from Places2Play and Pickleheads
- **WP Go Maps integration** — custom CSV import pipeline, infowindow badge formatting
- **"Play & Stay" pages** — hotel booking pages for all 50 states (Expedia affiliate)
- **Court data pipeline** — Python/BeautifulSoup processing, state-by-state CSV import

---

## Content System — BigPickleBalls.com

- Long-form HTML blog posts using scoped `.bpb-article` wrapper
- Background color: `#c8cae8` (lavender) — consistent across all posts
- Scoped CSS — zero bleed into WordPress theme
- Author bio box — deployed via WPCode Pro, After Post Content
- Images generated via Grok, placed contextually per post
- AdSense approval in progress — E-E-A-T trust chain strategy:
  - Amazon Author Page → Personal Site → Feedspot listing → Social properties

---

## Affiliate Network — BaobabHosting.com

Active affiliate relationships:

| Partner | Type |
|---------|------|
| Kinsta | Managed WordPress hosting |
| SiteGround | Shared/cloud hosting |
| Cloudways | Cloud hosting |
| KnownHost | VPS hosting |
| InterServer | Budget/VPS hosting |
| UltaHost | Budget hosting |
| IONOS | Budget/business hosting |
| HostGator | Shared hosting |
| Bluehost | Shared hosting |
| JetHost | Specialty hosting |

Content uses an adversarial editorial voice — 300+ title library, prompt generator tool, batch HTML post generation via Anthropic API.

---

## Author

**Gregory de la Cruz** — Solo web entrepreneur, 22+ years WordPress experience, former Nortel Networks.

- 📚 [Amazon Author Page](https://www.amazon.com/author/gregorydelacruz) — 25+ published books
- 🌐 [GregorydelaCruz.com](https://gregorydelacruz.com)
- 💻 [GitHub](https://github.com/gregorydelacruz)
- 🏓 [Feedspot — Pickleball Blogs](https://blog.feedspot.com/pickleball_blogs/)

---

## License

All site content, templates, and tooling are proprietary.  
Code snippets and pipeline tools in this repository are for personal reference and portfolio documentation.

---

*Built with WordPress, Python, Make.com, and the Anthropic API.*  
*Inspired by a 91-year-old mother who still plays pickleball every day.*
