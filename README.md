⚔️ AI RPG Adventure: The Next Evolution of TTRPGs

Current Status: Prototype / Alpha

This repository outlines the architecture and vision for AI RPG Adventure, a revolutionary engine designed to solve the critical failures of current AI roleplaying games. Unlike existing platforms that function as glorified text predictors, this engine integrates a strict Rules Adjudication Layer with the narrative power of Large Language Models (LLMs), creating the first true AI Game Master.

View the active prototype in AI Studio: https://ai.studio/apps/drive/1UMc0eAEHrxtC_wKCNbMpqjZmk6xShvRL

🔒 Proprietary Notice

The source code is not provided in this repository because I intend to commercialize this project. My vision is that I have seen a unique opportunity to revolutionize the TTRPG experience through advanced AI integration, and I am currently developing the full commercial version.

💥 The Problem: Why Current AI RPGs Fail

The market is saturated with "AI Games" like AI Dungeon, NovelAI, and Character.ai, but they all suffer from the same fundamental flaws when trying to run a real Tabletop RPG:

Hallucination & Rule Breaking: Ask ChatGPT to run a game, and it will eventually let you jump to the moon or cast a spell you don't have. It prioritizes "Yes, and..." over game balance.

The "Goldfish Memory" Effect: Current LLMs lose track of inventory, health, and narrative threads after a few dozen turns.

Lack of Tactical Depth: There is no real game. There is no visual feedback for combat, no dice physics, and no resource management. It's just collaborative writing, not gaming.

🏆 Our Solution: The Competitive Advantage

We are not building a chatbot. We are building a Game Engine with a Soul.

1. The Micro-Agent Architecture (The "Brain")

Instead of relying on a single, confused prompt, our engine utilizes a sophisticated multi-agent system that separates duties, ensuring zero hallucination on mechanics:

The Adjudicator: A ruthless, logic-based agent that reads the Daggerheart rulebook. It validates every player action against their character sheet. If you try to fly without wings, it rejects the action before the story is even generated.

The Narrator: Frees the LLM to focus purely on evocative descriptions, knowing the math has already been checked.

The Bookkeeper: Silently manages the database state—HP, Gold, Stress, and Fear tokens—ensuring the world remains consistent 100% of the time.

2. True TTRPG Fidelity (The "System")

We don't just "pretend" to roll dice. We implement the full Daggerheart system mechanics:

Duality Dice Physics: A visual 3D dice roller that calculates Hope vs. Fear, triggering narrative consequences (Soft Moves vs. Hard Moves) exactly as the game designers intended.

Complex Damage Thresholds: Unlike simple HP bars, our engine handles Minor, Major, and Severe damage thresholds, armor slot usage, and stress mechanics automatically.

State-Aware Combat: A visual combat dashboard tracks initiative, enemy difficulty, and action economy. You don't type "I attack"; you click your Longsword, and the AI calculates the outcome based on your stats.

3. Visual & Interactive Hybrid (The "Experience")

We bridge the gap between video games and TTRPGs.

Dynamic UI: Inventory, Character Sheets, and Domain Cards are not text—they are interactive React components.

Visual Feedback: When you take damage, the screen reacts. When you spend Hope, the tokens deplete.

Tactical Depth: Manage your Domain Cards, exhaust abilities, and make strategic choices that matter.

🚀 Current Features

🧠 AI Game Master Core

Adjudicator Agent: Determines mechanical outcomes (e.g., "Roll Agility difficulty 12").

Narrator Agent: Transforms mechanical results into evocative storytelling.

Bookkeeper Agent: Manages state (Enemy HP, Player Stress, Inventory) in the background.

📜 Character Management

Interactive Builder: A 5-step wizard to create heroes (Class, Ancestry, Gear).

Automated Stats: auto-calculates Evasion and Damage Thresholds based on equipment.

Domain Cards: Digital tracking of abilities, spells, and exhaustion states.

⚔️ Tactical Combat System

Damage Resolver Modal: Implements specific Daggerheart damage rules (Minor/Major/Severe thresholds).

Combat Dashboard: Tracks enemy status, GM Fear pool, and one-click attacks.

Duality Dice Roller: Simulates "Hope vs. Fear" mechanics with critical success detection.

💾 Persistence & Memory

Chapter Archival: Summarizes gameplay into "Diary Entries" to maintain long-term context.

Local State: Full persistence of character data and campaign progress via local storage.

🔮 The Vision: Main Version Roadmap

The PoC is just the beginning. The commercial release will introduce Emergent Gameplay powered by Graph RAG.

🕸️ Knowledge Graphs: The game state will move from text to a Neo4j graph database, mapping every relationship between NPCs, factions, and items.

🧠 Graph Recall (RAG): The GM will perfectly recall a shopkeeper you met 500 turns ago or a promise made to a rival faction.

🦋 Emergent World: Killing a merchant will causally ripple through the graph, creating an economic crisis in a neighboring town that the AI detects and narrates.

Persistent Living World: A database that evolves even when the player isn't looking.
