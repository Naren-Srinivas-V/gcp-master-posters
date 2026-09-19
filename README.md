# GCP, Explained in Pictures
### One repo, two versions — pick based on who's looking

This repo holds a small set of standalone posters that explain the entire 7-chapter GCP learning series in pictures. There are two versions:

- **`simple/`** — zero jargon, for someone with no tech background at all. Uses a city, a pizza order, and your own front door as the only "technology" you need to already understand.
- **root folder** — the full technical version, using real GCP concepts and terminology, for anyone following the series itself or wanting something to share professionally (LinkedIn, a portfolio, etc.).

Both versions tell the same underlying story. Start with whichever matches your audience.

---

## 🟢 The Simple Version — For Anyone, No Tech Background Needed

If you can picture a city, a pizza order, and your own front door, you already have everything you need.

### Picture 1 — It's Just a City
![Imagine a City](simple/A-the-city.svg)

Think of "the cloud" as a well-run city. Every part has an ordinary, human job: **the Guard** checks IDs before anyone does anything, **the Roads** connect every building safely, **the Workshops** do the actual work, **the Storerooms** keep everything safe, **the Factories** turn raw information into insight, **the Delivery Crew** ships updates automatically, and **the Watchtower** keeps an eye on everything and writes it all down. That's it — a company running their app "on the cloud" is just renting a few buildings in a city like this one.

### Picture 2 — It Works Like Ordering a Pizza
![It Works Like Ordering a Pizza](simple/B-ordering-a-pizza.svg)

Almost everything an app does follows this same simple chain: **you call to order** → **"is this a real customer?"** (if not, the call is just refused, nothing bad happens) → **the kitchen gets to work** → **grabs the ingredients** → **delivered to your door**. Quietly, the Watchtower writes every step down, so if anything ever goes wrong, someone can look back and see exactly what happened.

### Picture 3 — The Four Rules Behind All of It
![The Four Rules Behind All of It](simple/C-four-rules.svg)

None of this is really about complicated technology — it's four rules you already use at home: **don't trust a stranger by default**, **hand out the smallest key that works**, **actually test the lock**, and **write down who came and went**. Everything "technical" is just one of these four rules, applied a bit more carefully than we usually bother to.

**Putting it together:** the city (Picture 1) is *what* it's made of. The pizza order (Picture 2) is *how* something happens, step by step. The four rules (Picture 3) are *why* it's trustworthy. That's genuinely the whole idea.

---

## 🔵 The Technical Version — For Following the Series or Sharing Professionally

These use the real GCP terms and tie directly back to the 7 chapters of the full learning series.

### 1. Why GCP Exists
![Why GCP Exists](01-why-gcp-exists.svg)

The shift from buying and maintaining your own servers to renting exactly the capacity you need, with Google handling the physical layer under the Shared Responsibility Model (Chapter 1).

### 2. What GCP Is — The Complete Map
![What Is GCP](02-what-is-gcp-city-map.svg)

The technical version of the city: IAM as City Hall, Networking as the roads, Compute/Storage/Data-AI/DevOps as four districts, and Observability as the watchtower — all seven chapters in one map.

### 3. How It All Works Together
![How a Request Flows](03-how-a-request-flows.svg)

A real request traced through Load Balancer → Firewall → IAM check → Cloud Run → Firestore → Pub/Sub, with the denied-request branch shown, and every step logging back to Cloud Logging.

### 4. When You Actually Need Each Piece
![When — A Maturity Ladder](04-when-a-maturity-ladder.svg)

A 4-stage maturity ladder — solo project → real product → shipping team → production at scale — showing each chapter is additive, never a replacement for what came before.

### 5. The Golden Thread
![The Golden Thread](05-the-golden-thread.svg)

The one repeated philosophy behind every chapter — deny by default, grant the smallest thing that works, prove it with a real test, log everything — shown as eight nodes (all seven chapters plus the logging discipline itself) circling one shared mantra.

---

## 📁 Repo Structure

```
gcp-master-posters/
├── README.md                        (this file)
├── 01-why-gcp-exists.svg
├── 02-what-is-gcp-city-map.svg
├── 03-how-a-request-flows.svg
├── 04-when-a-maturity-ladder.svg
├── 05-the-golden-thread.svg
└── simple/
    ├── A-the-city.svg
    ├── B-ordering-a-pizza.svg
    └── C-four-rules.svg
```

---

*Part of a self-directed GCP learning series — the full technical chapters live in their own repos: [gcp-iam-least-privilege-lab](../gcp-iam-least-privilege-lab) · [gcp-compute-least-privilege-lab](../gcp-compute-least-privilege-lab) · [gcp-firestore-least-privilege-lab](../gcp-firestore-least-privilege-lab) · [gcp-networking-deep-dive](../gcp-networking-deep-dive) · [gcp-data-ai-deep-dive](../gcp-data-ai-deep-dive) · [gcp-devops-cicd-deep-dive](../gcp-devops-cicd-deep-dive) · [gcp-observability-deep-dive](../gcp-observability-deep-dive)*
