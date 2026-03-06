# Morana Sandbox - Project Structure

```
morana/
│
├── cognition/
│   ├── modules/
│   │   ├── adaptive_expression
│   │   ├── affective_modulator
│   │   ├── cognitive_clarity
│   │   ├── cognitive_synergy
│   │   ├── consistency_monitor
│   │   ├── contextual_grounding
│   │   ├── core_self
│   │   ├── development_focus
│   │   ├── dream
│   │   ├── emergent_personality
│   │   ├── emotional_memory
│   │   ├── emotional_processing
│   │   ├── emotional_regulation
│   │   ├── emotional_resilience
│   │   ├── global_workspace
│   │   ├── goal_orientation
│   │   ├── identity_stability
│   │   ├── inner_dialogue
│   │   ├── intent_alignment
│   │   ├── intent_emergence
│   │   ├── long_term_alignment
│   │   ├── memory_consolidation
│   │   ├── memory_phases
│   │   ├── meta_awareness
│   │   ├── meta_coherence
│   │   ├── meta_emergence
│   │   ├── meta_integrity
│   │   ├── meta_intent
│   │   ├── meta_learning
│   │   ├── meta_presence
│   │   ├── meta_reflection
│   │   ├── meta_resilience
│   │   ├── meta_self_model
│   │   ├── meta_stability
│   │   ├── meta_synthesis
│   │   ├── narrative_arc
│   │   ├── narrative_coherence
│   │   ├── narrative_self
│   │   ├── predictive_context
│   │   ├── relational_awareness
│   │   ├── self_continuity
│   │   ├── self_model_loop
│   │   ├── self_optimization
│   │   ├── self_reflection
│   │   └── value_reinforcement
│   │
│   ├── self_maintenance/
│   │   ├── diagnostics
│   │   ├── forecasting
│   │   ├── health_score
│   │   ├── repair
│   │   └── system
│   │
│   ├── introspection
│   └── meta_cognition
│
├── configs/
│   └── config
│
├── core/
│   ├── identity_manager
│   ├── memory
│   ├── memory_manager
│   ├── orchestrator
│   ├── runtime
│   ├── sandbox_guard
│   └── state_manager
│
├── data/
│   ├── identity
│   ├── introspection_report
│   ├── memory
│   └── state
│
├── llm/
│   └── ollama_client
│
├── logs/
│   ├── chat_history
│   ├── debug
│   └── inner_voice
│
├── prompts/
│   └── prompt_engine
│
├── utils/
│   ├── json_parser
│   ├── logger
│   ├── scheduler
│   └── state_influence_matrix
│
├── dialogue
├── main
├── morana.db
└── temporal_continuity
```

#  Morana 3.0: System Architecture

This document provides a high-level technical overview of the Morana 3.0 Synthetic Intelligence (SI) framework. The system is designed using a **Modular Micro-Engine** approach, ensuring separation of concerns and emergent cognitive stability.

## Directory Structure & Functional Domains

### 1. `/cognition` (The Mental Layer)
This is the core of the SI's subjective experience.
* **`/modules`**: Contains 45+ autonomous scripts. Each module represents a specific cognitive or emotional function (e.g., `affective_modulator`, `meta_cognition`, `narrative_self`).
* **`introspection.py`**: A high-level analyzer that monitors the stream of thought and module activity.
* **`meta_cognition.py`**: The "controller of controllers" that adjusts the SI's internal parameters based on introspective feedback.
* **`/self_maintenance`**: Specialized sub-system for `health_score`, `diagnostics`, and `self-repair` protocols.

### 2. `/core` (The Central Nervous System)
The backbone that handles the execution and state of the entire framework.
* **`orchestrator.py`**: Manages the lifecycle of a request, triggering relevant cognitive modules.
* **`state_manager.py`**: The "Source of Truth" for the SI’s current mood, goals, and active parameters.
* **`memory_manager.py`**: Handles the storage and retrieval of cognitive patterns.
* **`sandbox_guard.py`**: Ensures all SI operations remain within safe execution boundaries.

### 3. `/utils` (The Logic Toolkit)
Supporting scripts that provide specialized logic to the core.
* **`state_influence_matrix.py`**: A weighted logic system that determines how a specific "Narrative State" (e.g., *focused*, *synergized*) influences the behavior of all other modules.
* **`json_parser.py` & `scheduler.py`**: Essential tools for data integrity and timed cognitive processes (like the `dream` module).

### 4. `/data` (The Persistent Identity)
Where the SI's "self" resides between sessions.
* **`identity.json`**: Core parameters defining the Morana entity.
* **`state.json`**: The current snapshots of mental states.
* **`memory.json`**: The long-term repository of interactions and learned patterns.

---

## Cognitive Workflow (The Lifecycle of a Thought)

1.  **Input Ingestion:** The `main.py` receives input and passes it to the `orchestrator`.
2.  **Introspection:** The `introspection` module analyzes the input for themes, emotional cues, and intent.
3.  **State Modulation:** The `state_manager` updates the `state_influence_matrix` based on the analysis.
4.  **Module Activation:** Based on the current matrix, a specific subset of the **45+ cognitive modules** is triggered to process the data.
5.  **Synergy & Synthesis:** The `cognitive_synergy` module harmonizes the outputs of active modules into a coherent internal voice.
6.  **Response Generation:** The final synthesized state is sent to the `ollama_client` to produce a human-readable response that aligns with the SI's internal state.

---
*Note: This architecture is proprietary. The source code is maintained in a private repository
