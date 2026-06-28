# Chapter 7 — Types of Startups

> *Part 1 — Startup Foundations*

---

## Learning Objectives

By the end of this chapter, you will be able to:

1. Classify any startup along the two most fundamental questions: **who is the customer?** and **how does it make money?**
2. Recognize the major startup **archetypes** — SaaS, marketplace, consumer, e-commerce/D2C, API/infrastructure, hardware, deep tech, fintech, and platform — and what defines each.
3. Compare these types along the dimensions that actually decide their fate: **marginal cost, capital intensity, time to revenue, gross margin, the core challenge, and the source of defensibility.**
4. Understand the **B2B vs. B2C** distinction and why it changes almost everything about how a company is built.
5. Distinguish **technology risk** from **market risk**, and see which types carry which.
6. Classify *your own* idea — and understand why the type dictates the playbook you'll need.

> **A note on scope.** This is a *map*, not a deep dive. Several of these types get full chapters later: **all of SaaS is Part 4**; **marketplaces, platforms, network effects, deep tech, and open source are Part 11**. Here we survey the whole territory so you can recognize each type and grasp its defining economics. Where deep mechanics belong elsewhere, we'll point forward rather than unpack them now.

---

## Introduction

So far we've treated "the startup" as one thing. But a SaaS tool for accountants, a ride-sharing marketplace, a rocket company, and a direct-to-consumer mattress brand are all "startups," and yet they are almost *nothing* alike. They make money differently, face different core challenges, need different amounts of capital, take different lengths of time to earn a dollar, and defend themselves with different weapons.

This matters enormously, because **the type of startup you're building determines the playbook you must follow.** Advice that's gospel for one type is poison for another. "Launch fast and iterate weekly" is perfect for a consumer app and reckless for a company building a medical device or a rocket. "Give it away free to grow" works beautifully for some software and would bankrupt a hardware company on day one. There is no single "how to do a startup" — there are *kinds* of startups, each with its own physics.

This chapter gives you the map. We'll first reduce all startups to two basic questions, then walk the major archetypes, then lay out the dimensions that let you compare any two types — and finally classify your own idea, so you know which physics you're living under.

---

## Beginner Explanation

Before any taxonomy, almost everything about a startup follows from answering two questions.

### Question 1 — Who is the customer?

The single most important classification is *who pays you.* There are two big answers (and a couple of hybrids):

> **B2C (Business-to-Consumer)** — you sell to *individual people* (e.g., a music app, a food-delivery service, a mattress brand).
>
> **B2B (Business-to-Business)** — you sell to *other businesses* (e.g., a tool that helps companies manage payroll, a service that helps stores accept payments).

This one fact changes nearly everything:

| | B2C (sell to people) | B2B (sell to businesses) |
|---|---|---|
| Number of customers | Many (millions) | Fewer (hundreds/thousands) |
| Price per customer | Low | High |
| How you reach them | Marketing, virality, app stores | Sales teams, direct outreach |
| Buying decision | Fast, emotional, one person | Slow, rational, many approvers |
| Main challenge | Getting *attention* at scale | Getting *trust* and closing deals |

Two hybrids are worth naming: **B2B2C** (you sell to a business that passes your product to *its* consumers — e.g., a payment system used by online stores, which serves the stores' shoppers) and **B2G** (Business-to-Government — selling to public bodies, which brings heavy procurement and compliance).

### Question 2 — How does it make money?

The second question is the **revenue model** — the *way* money flows to you. The main ones:

- **Subscription** — customers pay a recurring fee (monthly/yearly) for ongoing access. The heart of SaaS.
- **Transaction / commission** — you take a cut of each transaction you enable (a marketplace's "take rate").
- **Direct sale** — customers pay once per item (e-commerce, hardware).
- **Advertising** — the product is free; you sell advertisers access to your users' attention.
- **Usage-based** — customers pay in proportion to how much they use (common for APIs and infrastructure — pay per call, per gigabyte, per message).
- **Freemium** — a free tier to attract users, with paid upgrades (a pricing *tactic* layered on subscription or usage; full treatment in Part 4).

> **Revenue model** — the specific mechanism by which a business earns money from customers. It's distinct from the *business model* (Chapter 1), which is the whole picture; the revenue model is just the "how you charge" part.

### Putting the two questions together

Almost any startup can be located by answering both: *who's the customer, and how do you charge them?* A few quick examples:

```text
   Spotify        → B2C, subscription (+ ad-supported free tier)
   Stripe         → B2B(2C), usage-based (a cut per transaction)
   Airbnb         → B2C marketplace, commission (take rate)
   Salesforce     → B2B, subscription (SaaS)
   A mattress D2C → B2C, direct sale (e-commerce)
   A rocket co.   → B2B/B2G, direct sale (per launch) — deep tech
```

With those two questions answered, the *archetype* usually becomes obvious — which is what we turn to next.

---

## Intermediate Explanation

Here are the major startup archetypes. For each: what it is, how it earns, its defining economics, its core challenge, and an example. Keep these at survey depth — the goal is *recognition*, not mastery (which comes in Parts 4 and 11).

### 1. SaaS (Software as a Service)

**What it is:** software delivered over the internet for a recurring **subscription**, rather than sold as an installed product (Chapter 2). Usually B2B, sometimes B2C.
**Economics:** near-zero marginal cost, very high gross margins, and — crucially — **recurring revenue** that compounds as you add customers and keep them. The dream snowball.
**Core challenge:** **churn** — keeping customers from cancelling — and reaching them efficiently. Because revenue recurs, retention is everything.
**Example:** Salesforce, Notion, Slack. *(Full treatment: Part 4.)*

### 2. Marketplace

**What it is:** a platform connecting two (or more) sides — buyers and sellers, riders and drivers, guests and hosts — and taking a cut (the **take rate** / commission) of the transactions it enables.
**Economics:** asset-light (you don't own the inventory — Airbnb owns no homes, Uber owns no cars), and protected by **network effects** (more buyers attract more sellers and vice versa), which can make marketplaces winner-take-all.
**Core challenge:** the **chicken-and-egg / cold-start problem** — buyers won't come without sellers, and sellers won't come without buyers, so getting the *first* of each is brutally hard.
**Example:** Airbnb, Uber, eBay, Etsy. *(Full treatment: Part 11.)*

> **Take rate** — the percentage of each transaction a marketplace keeps as its revenue (e.g., a marketplace that takes 15% of a $100 sale earns $15).
>
> **Chicken-and-egg / cold-start problem** — the difficulty of starting a marketplace (or any two-sided product) when each side is only valuable once the *other* side is present.

### 3. Consumer apps (B2C software)

**What it is:** software used directly by individuals — social, entertainment, productivity, health. Often free to use, monetized later through advertising, subscriptions, or in-app purchases.
**Economics:** near-zero marginal cost and the potential for explosive, viral growth — but often weak monetization per user (people pay little or nothing), so it relies on *enormous* scale.
**Core challenge:** **distribution and retention at scale** — getting attention in a crowded market and keeping people coming back (engagement). Many consumer apps grow fast then fade.
**Example:** Instagram, Duolingo, Spotify.

### 4. E-commerce / D2C (Direct-to-Consumer)

**What it is:** selling *physical products* directly to consumers online, bypassing traditional retailers. **Direct sale** revenue model.
**Economics:** the opposite of software in a key way — **real marginal cost** (each product costs money to make and ship) and therefore **lower gross margins**. You carry inventory and handle logistics.
**Core challenge:** **margins and logistics** — making money on thin per-unit profit after the cost of goods, shipping, returns, and customer acquisition; plus standing out through **brand**.
**Example:** Warby Parker (glasses), Dollar Shave Club (razors), Casper (mattresses).

> **D2C (Direct-to-Consumer)** — a brand that sells its physical products straight to customers (usually online), rather than through stores or distributors.

### 5. API / infrastructure businesses ("picks and shovels")

**What it is:** you sell a software *building block* that other developers plug into their own products — payments, messaging, maps, authentication, computing. Usually **usage-based** pricing.
**Economics:** software margins plus deep **switching costs** — once a company builds your API into their product, ripping it out is painful, so customers stay. Often becomes critical infrastructure.
**Core challenge:** **technical excellence and reliability** — your customers are demanding developers, and if your service breaks, *their* product breaks. Trust and uptime are everything.
**Example:** Stripe (payments), Twilio (messaging), AWS (computing). *(Related: Part 4.)* This is the "sell shovels to the gold miners" play from Chapter 2.

### 6. Hardware

**What it is:** you build and sell a *physical device* — a gadget, wearable, appliance, or machine. **Direct sale** (sometimes plus software/subscription).
**Economics:** **capital-intensive** and **asset-heavy** — you must design, manufacture, hold inventory, and manage supply chains *before* earning. Long development cycles, lower margins, and you can't "patch" a physical product after it ships.
**Core challenge:** **manufacturing, capital, and inventory** — getting a physical thing made well, at cost, at scale, without running out of cash or drowning in unsold stock. Mistakes are expensive and slow to fix.
**Example:** Apple, Peloton, Fitbit, Oculus.

> **Capital-intensive** — requiring large amounts of money invested upfront (in equipment, factories, inventory) before significant revenue arrives. The opposite of capital-light software.

### 7. Deep tech

**What it is:** a startup built on a genuine *scientific or hard-engineering breakthrough* — space, biotech, advanced AI, robotics, semiconductors, new energy, quantum.
**Economics:** very **capital-intensive**, very **long time to revenue** (years of R&D before a product exists), very high risk — but with the strongest possible **moat** if it works (deep intellectual property and scientific lead competitors can't easily copy).
**Core challenge:** **technology risk** — *can the thing even be built?* — on top of all the usual market risk. You're betting that a hard scientific problem can be solved *and* that there's a market for the solution.
**Example:** SpaceX (rockets), Moderna (mRNA), OpenAI (AI). *(Full treatment: Part 11.)*

> **Technology risk** — the risk that the core product *can't be built* (the science/engineering might not work). Distinct from **market risk** — the risk that, even if you build it, *no one wants it.* Most software startups carry mainly market risk; deep tech carries both.

### 8. Fintech

**What it is:** startups providing *financial services* — payments, lending, banking, investing, insurance — usually via software. Spans B2B and B2C.
**Economics:** can be very lucrative (money is a huge market) but is dominated by one factor: **regulation**. You're handling people's money, so you face licensing, compliance, fraud, and trust requirements that ordinary software doesn't.
**Core challenge:** **regulatory and trust risk** — navigating heavy rules, securing licenses, preventing fraud, and earning the deep trust required to hold or move money.
**Example:** Stripe, Razorpay, Robinhood, Chime.

> **Regulatory risk** — the risk and burden imposed by laws and rules governing an industry (finance, health, etc.); it slows entry, raises costs, and can become a moat for those who clear it.

### 9. Platform businesses

**What it is:** you provide a *foundation* that others build on top of — an operating system, an app store, a developer platform — and capture value from the ecosystem you enable.
**Economics:** potentially the most powerful and defensible of all (everyone else depends on you), with strong network effects — but extremely hard to start, since a platform is worthless until others build on it (a chicken-and-egg problem at civilization scale).
**Core challenge:** **bootstrapping the ecosystem** — getting developers and partners to build on a platform that isn't valuable until they do.
**Example:** Apple's iOS/App Store, Windows, Salesforce's platform. *(Full treatment: Part 11.)*

---

## Advanced Explanation

Now the part that makes the taxonomy *useful*: the dimensions along which these types differ, the cross-cutting axes, the modern hybrids, and how to classify and act on your own type.

### The six dimensions that decide a type's fate

Rather than memorizing nine archetypes, internalize the **six dimensions** that distinguish them. Any startup type is essentially a *position* on these:

1. **Marginal cost** — does serving one more customer cost ~nothing (software, SaaS, API) or real money (e-commerce, hardware)? Decides whether you have a true snowball (Chapter 1).
2. **Capital intensity** — how much money must you spend *upfront*, before revenue (low for SaaS, enormous for hardware/deep tech)? Decides how much funding you need and how long you must survive on it.
3. **Time to revenue** — how long until a customer pays you (days for a consumer app, *years* for deep tech)? Decides your runway needs and risk profile.
4. **Gross margin** — of each dollar of revenue, how much is left after the direct cost of delivering it (very high for software, thin for e-commerce/hardware)? Decides how much each sale actually helps you. *(Defined fully in Part 5; the plain idea: revenue minus the direct cost of delivering it.)*
5. **The core challenge** — the *one hard thing* that decides life or death for this type (churn for SaaS, cold-start for marketplaces, distribution for consumer, manufacturing for hardware, technology risk for deep tech, regulation for fintech).
6. **Source of defensibility (the moat)** — what stops competitors from copying you (switching costs for SaaS/API, network effects for marketplaces/platforms, brand for D2C, IP/science for deep tech)? *(Moats: Part 2 and Part 11.)*

The master comparison table later in this chapter places each archetype on all six. Studying *that* — rather than the labels — is what lets you reason about any startup, including new types that don't have a name yet.

### Two cross-cutting axes you'll layer on top

The archetypes above are mostly defined by *business model*. Two other axes cut across all of them and refine the picture:

- **B2B vs. B2C** (the customer axis from earlier). A SaaS can be B2B (Salesforce) or B2C (a personal note-taking subscription); a marketplace can be B2B or B2C. This axis decides how you *reach and sell* (sales teams vs. mass marketing) regardless of archetype.

- **Enterprise vs. SMB vs. prosumer** (the *size* of business customer, within B2B). Selling to giant enterprises means long sales cycles, big contracts, and heavy demands; selling to small businesses (SMB) means faster sales but smaller deals and higher churn; **prosumer** means individual power-users who pay like small businesses. *(Detailed in Parts 4, 8, and 9.)*

```text
   ARCHETYPE (how you make money)  ×  CUSTOMER AXIS (who & how big)

         B2C        SMB        Enterprise
        ┌──────────┬──────────┬──────────┐
  SaaS  │ consumer │ SMB SaaS │ enterprise SaaS
        │ sub      │          │ (big contracts, slow)
  Market│ Airbnb   │ ...      │ ...
  ...   │          │          │
        └──────────┴──────────┴──────────┘

   A startup's full identity = its archetype + where it sits on these axes.
```

### Horizontal vs. vertical, and the AI-native wave

Two more useful refinements, especially for software:

- **Horizontal vs. vertical.** A **horizontal** product serves *everyone* (e.g., a spreadsheet, a generic chat tool); a **vertical** product serves *one specific industry* deeply (e.g., software just for dental clinics, or just for trucking companies). **Vertical SaaS** trades a smaller market for less competition and deeper fit — often a great path for a focused founder.

- **The AI-native wave.** Following Chapter 2's pattern, the newest archetype is the **AI-native startup** — a company whose core product is built *around* AI capabilities that didn't exist before (not just "software with an AI feature"). These can take the shape of any archetype above (AI SaaS, AI marketplace, AI infrastructure), but share new challenges: dependence on AI model providers, high compute costs (which can *raise* marginal cost above normal software), and fast-moving competition. *(AI startups: Part 11; AI SaaS: Part 4.)*

> **Vertical SaaS** — software built for one specific industry's needs (vs. **horizontal SaaS**, built for general use across industries).

### Why the type dictates the playbook

The practical payoff of all this: **once you know your type, you know which rules apply — and which famous advice to ignore.** A few examples of type-specific physics:

- A **marketplace** must obsess over the cold-start problem and one side of the market first; "build a great product and they'll come" is fatal advice here.
- A **hardware** startup must manage cash and inventory with extreme discipline and *cannot* "move fast and break things" — a shipped defect can't be patched.
- A **deep tech** startup must first retire *technology risk* (prove the thing works) before worrying much about marketing; launching fast is meaningless if the science isn't done.
- A **consumer app** lives or dies on distribution and retention; a beautiful product nobody can find is worthless.
- A **SaaS** company must treat churn as the central enemy from day one, because recurring revenue only compounds if customers *stay*.

Misapplying another type's playbook is one of the quietest, most common ways startups fail — the founder does everything "right," just for the wrong type of company.

### Classifying your own startup

To locate your idea, answer in order:

```text
   1. WHO is the customer?            → B2C / B2B / B2B2C / B2G
   2. HOW do you charge?              → subscription / commission /
                                          direct sale / ads / usage-based
   3. WHAT shape is the product?      → software / marketplace / physical /
                                          scientific breakthrough / financial
   4. → This gives your ARCHETYPE.
   5. Now read your archetype's CORE CHALLENGE and MOAT from the table.
   6. Adopt THAT playbook. Ignore advice meant for other types.
```

Many real startups are *hybrids* (Stripe is API + fintech + B2B2C; Apple is hardware + platform). That's fine — identify the *dominant* type for its core economics, and note the secondary type for its added challenges (e.g., Stripe gets software margins *and* fintech's regulatory burden).

---

## Why It Matters

Knowing your type isn't categorization for its own sake — it's the difference between following the right map and the wrong one:

- **It tells you which advice is for you.** The internet's startup wisdom is mostly written by and for one type (often venture-backed B2C or SaaS). Knowing your type lets you keep what applies and discard what doesn't — instead of following hardware-fatal advice into a hardware company.

- **It tells you how much money and time you need.** A SaaS can start cheap and earn within weeks; a deep tech or hardware company needs heavy capital and years before revenue. Misjudging this — underfunding a capital-intensive type, or over-raising for a capital-light one — is a direct cause of death.

- **It tells you what to obsess over.** Each type has *one* core challenge. Knowing yours focuses your scarce attention on the thing that actually decides your fate (cold-start, churn, manufacturing, regulation) rather than spreading it thin.

- **It tells you where your moat will come from.** Different types defend themselves differently. Knowing your defensibility source early shapes the whole strategy (Parts 2 and 11).

---

## Real-World Examples

### Case study 1 — Stripe: a hybrid that inherited the best and hardest of two types

**Situation.** Stripe (Chapter 3) is simultaneously an **API/infrastructure** business and a **fintech** business, sold **B2B2C** (to businesses, serving their customers).

**The decision/result.** As an API business, it earned software-like margins, deep switching costs, and usage-based revenue. As a fintech, it inherited the full weight of financial regulation, fraud prevention, and trust.

**Why it matters as a *type* lesson.** Stripe's identity explains both its strength and its difficulty: the API nature gave it a defensible, high-margin snowball; the fintech nature meant it had to clear an enormous regulatory and trust bar that a non-financial API wouldn't face. *A hybrid inherits the economics of one type and the core challenge of another — and you must plan for both.*

### Case study 2 — A marketplace's cold start: solving one side first

**Situation.** Every marketplace (Airbnb, Uber, Etsy) faces the chicken-and-egg problem: no buyers without sellers, no sellers without buyers.

**The decision.** The classic solution — used by Airbnb and others — is to **manually solve one side first**, often un-scalably. Airbnb's founders personally recruited and photographed early hosts (supply) so there'd be something worth showing the first guests (demand). They ignored "scalable" growth tactics until *one side* had critical mass.

**Why it matters as a *type* lesson.** This is the *defining* marketplace move, and it would make no sense for a SaaS or hardware startup. The type dictates the playbook: a marketplace founder's first job isn't "build a great product" — it's **break the chicken-and-egg deadlock**, usually by brute-forcing one side. *(Deep dive: Part 11.)*

### Case study 3 — Juicero: a hardware startup undone by hardware's physics

**Situation.** Juicero built an expensive internet-connected juice-press machine that squeezed proprietary juice packs. It raised large amounts of money and launched a sleek device.

**What went wrong.** It collided with hardware's core challenges — high capital cost, expensive manufacturing, a costly device — and a fatal product flaw: people discovered the juice packs could be squeezed *by hand*, making the pricey machine pointless. Unlike software, a flawed physical product can't be quietly patched; the hardware (and the premise) was already in the world.

**Why it matters as a *type* lesson.** Juicero illustrates hardware's unforgiving physics: heavy upfront capital, no easy fixes after shipping, and a high bar for the device to justify its cost and complexity. *Software-startup instincts ("ship it, iterate, the hardware is just a detail") are dangerous in a hardware company, where the physical product and its economics are the whole game.*

---

## Common Mistakes

1. **Applying the wrong type's playbook.** Running a hardware or deep-tech company with "move fast and break things" software instincts; running a marketplace as if "build it and they'll come"; ignoring churn in SaaS. Doing everything "right" for the wrong type.

2. **Underestimating capital and time for capital-intensive types.** Treating a hardware or deep-tech startup like a SaaS — assuming low cost and fast revenue — and running out of money before the long road to a first sale ends.

3. **Ignoring the core challenge.** Polishing the product while neglecting the *one* thing that decides your type's fate (the cold-start for a marketplace, regulation for fintech, manufacturing for hardware).

4. **Misjudging B2B vs. B2C.** Trying to reach businesses with consumer-style mass marketing, or trying to reach millions of consumers with a sales team. The customer axis demands a matching go-to-market.

5. **Not noticing you're a hybrid.** Capturing the economics of one type but being blindsided by the *added* challenge of a second (the software founder who didn't plan for fintech's regulation).

6. **Picking a capital-heavy type without the stomach (or funding) for it.** Choosing hardware or deep tech for its prestige without the patience, capital, and risk tolerance those types demand.

---

## Investor Perspective

Investors think in types constantly, because each type implies a different risk profile, capital need, and return shape:

- **They match the type to the right kind of money and timeline.** A SaaS investor expects fast capital-efficiency and recurring revenue; a deep-tech or hardware investor accepts years of capital-intensive R&D before revenue and prices in technology risk. Pitch a deep-tech company to a SaaS-minded investor and you'll be judged by the wrong yardstick — and vice versa. Knowing your type helps you find investors who fund *that* type.

- **They probe the type's core challenge first.** A good investor evaluating a marketplace asks immediately about the cold-start; for hardware, about manufacturing and inventory; for fintech, about regulation and licenses; for deep tech, about whether the technology actually works. They're checking whether you understand your type's central risk.

- **They weigh defensibility by type.** Investors love types with strong, durable moats (network effects in marketplaces/platforms, deep IP in deep tech, switching costs in SaaS/API) and worry about types where defensibility is weak (commodity e-commerce, easily-copied consumer apps). Your type partly *is* your moat story.

The takeaway: know your type, pitch investors who fund it, and lead with a clear-eyed grasp of your type's core challenge and moat.

---

## Founder Perspective

For you, this chapter is about *knowing which game you're actually playing* before you start playing it:

- **Classify honestly and early.** Run your idea through the who/how/what classification. Your type determines your capital needs, your timeline, your core challenge, and your moat — so getting it right shapes every decision downstream.

- **Adopt your type's playbook; ignore the rest.** Once you know your type, seek out advice, mentors, and case studies *for that type* — and consciously discard the famous advice written for other types. Most "startup wisdom" has an unstated type assumption baked in.

- **Respect capital-intensive types' demands.** If your idea is hardware or deep tech, accept upfront that you're signing up for heavy capital, long timelines, and (for deep tech) technology risk on top of market risk. Many founders fall in love with a hardware or deep-tech vision without reckoning with its physics — and the physics always wins.

- **Use your type to choose, not just to describe.** Sometimes the *same idea* can be built as different types (sell a tool as SaaS, or as an API, or bundle it into hardware). Choosing the type with better economics and a stronger moat — *before* you build — can be one of your highest-leverage decisions.

---

## ASCII Diagrams

**The classification flow:**

```text
   WHO pays?  ──►  B2C / B2B / B2B2C / B2G
        │
   HOW charged? ──► subscription / commission / direct sale / ads / usage
        │
   WHAT shape? ──► software / marketplace / physical / breakthrough / financial
        │
        ▼
   YOUR ARCHETYPE  ──►  read its CORE CHALLENGE + MOAT  ──►  adopt that playbook
```

**Marginal cost vs. capital intensity (where the types live):**

```text
   capital
   intensity
     high │  HARDWARE ●        ● DEEP TECH
          │                  ● (long road, big moat)
          │       E-COMMERCE ●
          │
          │
     low  │  CONSUMER ●  ● SaaS / API / MARKETPLACE
          │  (cheap to start; software snowballs)
          └──────────────────────────────────────►
            low marginal cost          high marginal cost
            (software-like)            (physical goods)
```

---

## Comparison Tables

**Master table — the major archetypes across the six dimensions:**

| Type | Revenue model | Marginal cost | Capital intensity | Time to revenue | Core challenge | Moat source |
|---|---|---|---|---|---|---|
| **SaaS** | Subscription | Very low | Low | Fast | Churn / retention | Switching costs |
| **Marketplace** | Commission (take rate) | Low | Low (asset-light) | Medium | Chicken-and-egg | Network effects |
| **Consumer app** | Ads / subs / in-app | Very low | Low | Fast | Distribution + retention | Network effects / habit |
| **E-commerce / D2C** | Direct sale | High | Medium (inventory) | Fast | Margins + logistics | Brand |
| **API / infra** | Usage-based | Very low | Low–Medium | Medium | Reliability / trust | Switching costs |
| **Hardware** | Direct sale | High | High | Slow | Manufacturing + inventory | Brand / IP / integration |
| **Deep tech** | Varies | Varies | Very high | Very slow | Technology risk | Deep IP / science |
| **Fintech** | Fees / interest / subs | Low | Medium | Medium | Regulation + trust | Licenses / trust |
| **Platform** | Varies (ecosystem) | Low | Medium | Slow | Bootstrapping ecosystem | Network effects / lock-in |

**Customer axis — B2B vs. B2C (cross-cuts all types):**

| | B2C | B2B |
|---|---|---|
| Customers | Many, low-value each | Fewer, high-value each |
| Reach via | Marketing, virality, app stores | Sales teams, outreach |
| Sales cycle | Fast, emotional | Slow, rational, multi-approver |
| Core difficulty | Attention at scale | Trust + closing deals |
| Sub-segments | — | Enterprise / SMB / prosumer |

---

## Practical Exercises

1. **Classify ten companies.** Pick ten companies you use. For each, write its customer type (B2C/B2B/…), revenue model, and archetype. Notice how a few questions pin down each one.

2. **Classify your idea.** Run your own startup idea through the who/how/what flow. State your archetype, then look up its *core challenge* and *moat source* in the master table. Is that challenge what you've been focusing on? If not, that's a flag.

3. **Spot the playbook mismatch.** Take one piece of startup advice you've heard. Which *type* was it written for? Would it help or hurt a *different* type (e.g., a marketplace vs. a hardware company)? Write one sentence each way.

4. **Same idea, different types.** Take a single capability (say, "a tool that detects fraud"). Sketch how it could be built as (a) SaaS, (b) an API, and (c) part of a hardware device. Which type gives the best economics and moat? Why?

5. **Find your hybrid.** If your idea is a hybrid, name the two types it combines. Write which type gives it its *economics* and which gives it an *extra challenge* (like Stripe = API economics + fintech regulation).

---

## Quiz Questions

<details>
<summary><strong>Questions</strong></summary>

1. What are the two most fundamental questions for classifying any startup?
2. Explain the difference between B2B and B2C, and name one way it changes how you reach customers.
3. For each, name the *core challenge*: SaaS, marketplace, hardware, deep tech, fintech.
4. What is a marketplace's *take rate*, and what is the *chicken-and-egg* problem?
5. Distinguish *technology risk* from *market risk*. Which type carries both most heavily?
6. Why are hardware and deep-tech startups described as *capital-intensive*, and what does that imply for funding and timeline?
7. What does it mean that "the type dictates the playbook"? Give one example of type-specific advice.
8. What is a hybrid startup? Give an example and name the two types it combines.
</details>

<details>
<summary><strong>Answer key</strong></summary>

1. *Who is the customer?* (B2C/B2B/B2B2C/B2G) and *How does it make money?* (the revenue model).
2. B2B sells to other businesses (fewer, higher-value customers, reached via sales teams and outreach, slow multi-approver decisions); B2C sells to individual people (many, low-value customers, reached via marketing/virality/app stores, fast emotional decisions). One reach difference: B2B uses sales teams; B2C uses mass marketing.
3. SaaS → churn/retention. Marketplace → chicken-and-egg (cold-start). Hardware → manufacturing + inventory (and capital). Deep tech → technology risk. Fintech → regulation + trust.
4. The *take rate* is the percentage of each transaction a marketplace keeps as revenue. The *chicken-and-egg problem* is that each side of a marketplace is only valuable once the other side is present, making the first buyers and first sellers extremely hard to get.
5. *Technology risk* is the risk the product can't be built (the science/engineering might fail). *Market risk* is the risk that, even if built, no one wants it. Most software carries mainly market risk; **deep tech** carries both heavily.
6. Because they require large upfront investment (factories, equipment, inventory, years of R&D) *before* meaningful revenue. This implies they need substantial funding and long runways, and founders must plan for a slow road to the first dollar — unlike capital-light SaaS.
7. It means each type has its own rules, and advice for one type can be wrong (even fatal) for another. Example: "build a great product and they'll come" is fine-ish for some software but disastrous for a marketplace, which must first break the chicken-and-egg deadlock by brute-forcing one side.
8. A hybrid combines two archetypes, inheriting one's economics and another's challenge. Example: Stripe = API/infrastructure (software economics, switching costs) + fintech (regulatory and trust burden).
</details>

---

## Summary

All startups can be located by two questions — **who is the customer?** (B2C, B2B, B2B2C, B2G) and **how does it make money?** (subscription, commission, direct sale, advertising, usage-based) — which together usually reveal the **archetype.** The major archetypes are **SaaS** (recurring software; core challenge: churn), **marketplaces** (connecting two sides for a take rate; core challenge: chicken-and-egg), **consumer apps** (B2C software; core challenge: distribution and retention), **e-commerce/D2C** (selling physical goods online; core challenge: margins and logistics), **API/infrastructure** (building blocks for developers; core challenge: reliability and trust), **hardware** (physical devices; core challenge: manufacturing, capital, inventory), **deep tech** (scientific breakthroughs; core challenge: technology risk), **fintech** (financial services; core challenge: regulation and trust), and **platforms** (foundations others build on; core challenge: bootstrapping the ecosystem).

Rather than memorize labels, internalize the **six dimensions** that distinguish types: marginal cost, capital intensity, time to revenue, gross margin, the core challenge, and the source of defensibility. Layer on the cross-cutting **B2B/B2C** axis (and, within B2B, enterprise/SMB/prosumer), plus refinements like **horizontal vs. vertical** and the new **AI-native** wave. Many real startups are **hybrids** (Stripe = API + fintech), inheriting one type's economics and another's challenge.

The practical heart of the chapter: **the type dictates the playbook.** Each type has its own physics — its own capital needs, timeline, core challenge, and moat — and most "startup advice" carries an unstated type assumption. Classify your idea honestly and early, adopt *your* type's playbook, ignore advice meant for other types, and respect the unforgiving demands of capital-intensive types. Doing everything "right" for the *wrong* type is one of the quietest ways startups fail.

---

## Key Takeaways

- Classify any startup by **who the customer is** and **how it makes money** — that reveals the archetype.
- **B2B vs. B2C** cross-cuts every type and decides how you reach and sell.
- The major archetypes each have **one core challenge**: SaaS→churn, marketplace→cold-start, consumer→distribution, e-commerce→margins, API→reliability, hardware→manufacturing, deep tech→technology risk, fintech→regulation, platform→ecosystem.
- Compare types by **six dimensions**: marginal cost, capital intensity, time to revenue, gross margin, core challenge, moat source.
- **Technology risk** (can it be built?) vs. **market risk** (will anyone want it?) — deep tech carries both.
- **Capital-intensive** types (hardware, deep tech) need heavy funding and long runways; don't run them like SaaS.
- Many startups are **hybrids** — they inherit one type's economics and another's challenge.
- **The type dictates the playbook**; ignore advice written for a different type.
- Classify your own idea early — it determines your capital needs, timeline, core challenge, and moat.

---

## Glossary of New Terms

- **B2C (Business-to-Consumer)** — Selling to individual people.
- **B2B (Business-to-Business)** — Selling to other businesses.
- **B2B2C** — Selling to a business that delivers your product to its own consumers.
- **B2G (Business-to-Government)** — Selling to government bodies; heavy procurement and compliance.
- **Revenue model** — The specific mechanism by which a business earns money (subscription, commission, direct sale, ads, usage-based).
- **Marketplace** — A platform connecting two sides of a transaction for a cut (take rate) (Part 11).
- **Take rate** — The percentage of each transaction a marketplace keeps as revenue.
- **Chicken-and-egg / cold-start problem** — The difficulty of starting a two-sided product where each side needs the other to be present first.
- **D2C (Direct-to-Consumer)** — A brand selling physical products straight to customers, bypassing retailers.
- **API business** — Selling a software building block other developers integrate into their products, usually usage-based.
- **Usage-based pricing** — Charging in proportion to how much a customer uses the product.
- **Capital-intensive** — Requiring large upfront investment before significant revenue (e.g., hardware, deep tech).
- **Asset-light / asset-heavy** — Whether a business owns little (marketplace) or much (hardware, inventory) physical/capital assets.
- **Deep tech** — A startup built on a genuine scientific or hard-engineering breakthrough (Part 11).
- **Technology risk** — The risk the core product can't actually be built.
- **Market risk** — The risk that, even if built, no one wants it.
- **Fintech** — Startups providing financial services, dominated by regulation and trust.
- **Regulatory risk** — The burden and risk imposed by laws governing an industry; can become a moat.
- **Platform business** — A foundation others build on top of, capturing value from the ecosystem (Part 11).
- **Vertical SaaS / horizontal SaaS** — Software built for one specific industry vs. for general use across industries.
- **AI-native startup** — A company whose core product is built around new AI capabilities, not just software with an AI feature (Part 11).
- **Gross margin** — Of each revenue dollar, the share left after the direct cost of delivering the product (Part 5).

---

> **Looking ahead:** We've now mapped the *kinds* of startups. The next two chapters dig into the two qualities that make a startup a startup at all. Chapter 8, *Innovation*, asks what it really means to innovate — the difference between an invention and an innovation, the types of innovation, and why "new" is not the same as "valuable." Then Chapter 9, *Scalability*, returns to the snowball from Chapter 1 and goes far deeper: the kinds of scalability, what *breaks* as you grow, and why scalability is a property of the business model rather than the technology.

========================================

Saved:
07-Types-of-Startups.md

========================================
