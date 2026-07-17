# Project-L.A.S.N.A
The intersection of History, Neuroscience, and Space Logistics. Architecting the backbone of future human expansion.

# Project L.A.S.N.
**[Logistics, AI, Space, Neuroscience, Archive]**

> "Those who cannot remember the past are condemned to repeat it. Those who model the past can optimize the future."

## The Mission
L.A.S.N.A is an architectural framework designed to solve the ultimate puzzle: **How do we sustain human expansion into space?** 

By integrating **Historical Data (Archive)**, **Neural Decision Models (Neuroscience)**, and **Advanced Logistics Optimization (AI)**, this project aims to create a self-correcting supply chain system capable of operating in the high-latency, high-risk environments of the final frontier.

## Why L.A.S.N.A?
*   **Archive:** We treat history not as a story, but as a dataset of bottleneck events.
*   **Neuro:** We mimic human cognitive resilience to build AI that doesn't panic when the unexpected happens.
*   **Space:** Because the supply chain of the future won't fit on a map of Earth.

## Roadmap: The First Three Months
- [ ] **Phase 1 (Data Layer):** Mapping historical trade disruptions into Neo4j graphs.
- [ ] **Phase 2 (Neuro Layer):** Building reinforcement learning agents based on cognitive decision models.
- [ ] **Phase 3 (Space Layer):** Simulating logistics networks under deep-space communication constraints.

## Current Status
*Currently constructing the historical graph of global trade-route failures. We are teaching the machine why the Silk Road mattered, so it can build the Mars Road later.*

### Day 1: Foundation
* **Goal**: Established the basic network nodes and connection logic.
* **Key Components**: Created `Location` nodes and `CONNECTED_TO` relationships.

### Day 2: Data Enrichment
* **Goal**: Added logistics intelligence to the network.
* **Properties Added**: `transport` (method), `distance` (numerical value).
* **Execution**: Used `SET` command to update relationships without recreating nodes.

### Day 3: Time-Axis Integration
* **Goal**: Added historical context to enable time-slice analysis.
* **Properties Added**: `start_year`, `end_year`.
* **Key Analysis Query**: 
  ```cypher
  // Query to extract routes active in a specific year (e.g., 250 AD)
  MATCH (c)-[r:CONNECTED_TO]->(s)
  WHERE r.start_year <= 250 AND r.end_year >= 250
  RETURN c, r, s

### Day 4: Network Expansion & Pathfinding
* **Goal**: Expanded the network with intermediate hubs (Samarkand, Alexandria).
* **New Concepts**: 
  - Network diversification: Transitioned from linear routes to a multi-node mesh network.
  - Path exploration: Implemented variable-length pathfinding to visualize connectivity.
* **Key Query**:
  ```cypher
  // Explore paths up to 5 steps from Changan to Rome
  MATCH p = (start:Location {name: 'Changan'})-[:CONNECTED_TO*..5]->(end:Location {name: 'Rome'})
  RETURN p

---
*Built by Ririku Shirakawa(Stella), a developer who prefers hard problems over easy exits.*
