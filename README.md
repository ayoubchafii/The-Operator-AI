# Hormozi-Style AI Business Advisor — A Claude Prompt Architecture

> Built by a 19-year-old founder in Morocco who got tired of AI advisors that talk in circles. This is the Claude setup I actually use to make decisions in my own business.

---

## Why this exists

I read all three of Alex Hormozi's $100M books — *Offers*, *Leads*, and *Money Models* — back to back over a few weeks while building my own startup ([Sellora AI](https://github.com/ayoubchafii), a WhatsApp AI receptionist for dental clinics in the Gulf).

The frameworks are clean. The thinking is sharp. But every time I tried to apply them to a real decision — *should I raise my price? is my offer weak or my leads weak? what should I fix first?* — I'd end up re-reading the same chapters, taking notes, drawing diagrams.

So I asked myself: what if the books could *talk back*?

I built this Claude Project setup over a few late nights. It turns Claude into a Hormozi-style advisor that diagnoses real business problems using actual frameworks — Value Equation, Core Four, LTGP:CAC, Money Model sequencing — instead of giving you generic MBA fluff.

It's not a chatbot pretending to be Alex. It's a strategic operator built from his public reasoning patterns, applied to *your* numbers.

---

## What this is (and isn't)

**This is:**
- A carefully engineered system prompt that forces Claude to reason like a blunt, framework-driven operator
- A structured knowledge base of frameworks, voice patterns, and operating principles
- A business context template that makes the advice tailored to *your* situation

**This is not:**
- A replacement for reading Hormozi's books — go read them, they're free at [acquisition.com/books](https://acquisition.com/books)
- An official Hormozi product or affiliated with Acquisition.com
- A magic button. The output quality scales with how honestly you fill out your business context.

---

## What makes this different from the average "Hormozi GPT"

Most prompt templates floating around are one paragraph that says *"act like Alex Hormozi"*. That's not engineering — that's a wish.

This project is different in three ways:

1. **Multi-file knowledge base architecture.** Frameworks, voice, beliefs, and your business context are split into separate files so Claude can route to the right one based on the question. Pricing question → frameworks file. Lead gen question → Core Four file. Your offer → your business file.

2. **Diagnosis-first reasoning pattern.** The system prompt forces Claude to name the bottleneck *before* recommending tactics. No "it depends." No five-bullet brainstorms. One real diagnosis, one next move.

3. **Built-in fallback rule.** If a question hits a gap in the knowledge files, Claude is allowed to draw on broader public Hormozi material — but only with explicit honesty about what's a framework vs. general business reasoning.

The result: an advisor that feels like a senior operator pressure-testing your business, not an AI hedging its way through your question.

---

## Setup — under 3 minutes

You'll need a [Claude Pro](https://claude.ai/upgrade) account to use the Projects feature.

### Step 1 — Create the project
1. Log into Claude
2. Click **Projects** in the bottom-left sidebar
3. Click **Create Project** and name it whatever you want (I named mine "Operator AI")

### Step 2 — Upload the knowledge base
1. Download the `knowledge-base` folder from this repo
2. In your new Claude Project, find the **Project Knowledge** section
3. Drag every `.md` file from `knowledge-base/` into it

### Step 3 — Add the system prompt
1. Open `system-prompt.md` in this repo
2. Copy the entire content
3. In your Claude Project, click **Edit Instructions** at the top
4. Paste and save

### Step 4 — Fill in your business context (this is the unlock)
1. Open `knowledge-base/00-my-business-TEMPLATE.md`
2. Fill it out honestly — your real prices, real numbers, real bottleneck
3. Save it as `00-my-business.md` and upload it to the project

The advisor will read that file at the start of every conversation and apply every framework through your business's actual context. This is the difference between *generic advice* and *advice that fits you*.

---

## Example interaction

**You:** *"I'm getting demo calls for my SaaS but most ghost after. I charge $497/mo."*

**Advisor:** *"That's not a sales problem. That's a Value Equation problem — specifically the Time Delay component. You're asking $497/mo before they experience a single win. Two fixes, in this order: (1) add a conditional guarantee tied to a result they can see in 7 days, (2) restructure the first month so something tangible happens in the first 48 hours. The price isn't the issue — the gap between paying and feeling progress is. Next move: list every result a buyer could feel in week one and pick the easiest to engineer."*

That's the bar. Real diagnosis, named framework, specific next move.

---

## Who this is for

- Founders building their first SaaS, agency, or service business
- Freelancers who want a strategist on call without paying $500/hr for a coach
- Operators who already know Hormozi's frameworks but want a faster way to apply them
- Students like me who are building in public on a budget

If you've never read the books, this tool will still help — but you'll get *significantly* more from it if you read them first. They're free.

---

## About the builder

I'm Ayoub Chafii, a first-year computer science engineering student at ISGA Rabat (Morocco). I'm building [Sellora AI](https://github.com/ayoubchafii) in parallel with my classes — a WhatsApp AI receptionist agency targeting dental clinics in Saudi Arabia and the UAE.

I made this because I needed it for myself. Sharing it because the cost of giving it away is zero, and someone, somewhere, is stuck on the same problem I was.

If it helps you, the best thing you can do is:
- ⭐ **Star this repo** — it costs nothing and helps other founders find it
- 📬 **Open an issue** if something doesn't work or could be sharper
- 🐦 **Tell me what you built** — I genuinely want to know

---

## Support the project

Building open-source from Morocco means traditional payment gateways like PayPal and Stripe aren't really an option for me. If this saved you hours of work or unlocked a real decision in your business and you want to send a coffee, crypto is the only route I can receive on:

**USDT (TRC-20)**
`THJ8CgiZfgjUCdnuwWPR9MTdSJUJeBdvM3`

<img src="assets/usdt-qr.png" alt="USDT TRC-20 QR Code" width="200"/>

**Binance Pay**

<img src="assets/binance-qr.png" alt="Binance Pay QR Code" width="200"/>

No pressure either way. The star is worth more to me than the tip.

---

## Roadmap

Things I'm planning to add as I keep using this:
- [ ] A "diagnosis-first" prompt template for one-shot offer reviews
- [ ] A landing page audit prompt
- [ ] Voice fidelity improvements (more Hormozi-pattern examples)
- [ ] Translations (Arabic, French)
- [ ] An equivalent setup for ChatGPT users

If there's something you want, open an issue.

---

## License

MIT. Use it, fork it, remix it, ship it. Just don't claim you built it from scratch — the frameworks belong to Hormozi, the architecture is mine.

---

*Independent educational project. Not affiliated with, endorsed by, or connected to Alex Hormozi or Acquisition.com. All frameworks referenced are public material discussed for educational and structural purposes. Buy his books — they're free at [acquisition.com/books](https://acquisition.com/books).*
