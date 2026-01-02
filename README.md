# ⚔️ AI RPG Adventure: Proof of Concept
**Current Status:** Prototype / Alpha

This repository contains the Proof of Concept (PoC) for an infinite, text-based Role-Playing Game engine. Currently powered by Google's Gemini API, this prototype demonstrates the core capability of a Large Language Model acting as a dynamic Game Master—generating descriptions, processing player intent, and managing basic narrative flow.

View the active prototype in AI Studio: [https://ai.studio/apps/drive/1UMc0eAEHrxtC_wKCNbMpqjZmk6xShvRL](https://ai.studio/apps/drive/1UMc0eAEHrxtC_wKCNbMpqjZmk6xShvRL)
Or in vercel: https://dagger-heart-gav2du468-leafargs-projects.vercel.app/
## 🚀 Current Features

This prototype implements a fully functional "Micro-Agent" architecture to handle complex RPG decision-making without breaking immersion.

### 🧠 AI Game Master Core
The system utilizes a multi-step cognitive process to run the game:
* **Adjudicator Agent:** Acts as the "Rules Lawyer," analyzing player intent against the Daggerheart ruleset to determine mechanical outcomes (e.g., "Roll Agility difficulty 12").
* **Narrator Agent:** Transforms dry mechanical results into evocative storytelling, describing the consequences of success or failure.
* **Bookkeeper Agent:** Manages state in the background, updating enemy HP, player stress, and inventory without manual input.

### 📜 Character Management
* **Interactive Builder:** A 5-step wizard to create heroes, guiding players through Class, Ancestry, and Gear selection.
* **Automated Stats:** Automatically calculates derived statistics like Evasion and Damage Thresholds based on equipment and features.
* **Domain Cards:** Digital tracking of abilities and spells, including resource costs (Hope) and exhaustion states.

### ⚔️ Tactical Combat System
* **Damage Resolver Modal:** Implements the specific Daggerheart damage rules, comparing incoming hits against Minor/Major/Severe thresholds and allowing players to spend Armor slots to mitigate harm.
* **Combat Dashboard:** A dedicated side panel for desktop users that tracks enemy status, manages the GM's Fear pool, and provides one-click attack rolls.
* **Duality Dice Roller:** A custom 3D-simulated dice roller that handles the "Hope vs. Fear" mechanic, automatically detecting critical successes and narrative complications.

### 💾 Persistence & Memory
* **Chapter Archival:** The AI automatically summarizes gameplay sessions into "Diary Entries," compressing long chat logs into narrative chapters to maintain context over long adventures.
* **Local State:** Full persistence of character data, chat history, and campaign progress via local storage.

## 🔮 The Vision: Main Version Roadmap
While this PoC demonstrates the narrative capabilities of Gemini, the upcoming Main Version is being architected to solve the "memory" and "consistency" problems inherent in LLM games.

The full release will integrate advanced data structures to power true Emergent Gameplay:

* **🕸️ Knowledge Graphs:** Moving beyond simple text history, the game state will be stored in a structured graph database (e.g., Neo4j). This maps relationships between every NPC, faction, location, and item.
* **🧠 Graph Recall (RAG):** The AI will utilize Retrieval-Augmented Generation against the knowledge graph. This ensures the GM perfectly recalls a shopkeeper you met 500 turns ago or a promise you made to a rival faction.
* **🦋 Emergent Gameplay:** World events will not be scripted. Using the graph, actions will ripple through the world organically—killing a merchant might cause an economic crisis in a neighboring town, detected and narrated by the AI.
* **Persistent World State:** A living, breathing database that evolves even when the player isn't looking.

## 🛡️ Run the Prototype
Follow these steps to run the current Proof of Concept locally.

**Prerequisites:** Node.js

### 1. Install Dependencies
Download the necessary libraries to run the LLM interface.

bash
npm install

### 2. Configure Credentials
You need a Gemini API Key to power the Game Master.

Create a file named .env.local.

Add your key: GEMINI_API_KEY=your_key_here

(Get your key here: Google AI Studio)

### 3. Launch the Adventure
Start the local development server.

Bash
npm run dev
