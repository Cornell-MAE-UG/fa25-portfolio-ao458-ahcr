---
layout: project
title: 2250 Portfolio
description: SLF Removal
technologies: 
image: 
---

## Table of Contents
- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)

---

## Client Pitch
<a name="client-pitch"></a>

**During Harvest SLF Removal**

**Client(s):** Cornell CALS Extension / E&J Gallo Winery / National Grape

**Problem Statement**  
Spotted Lanternflies (SLF) are devastating wineries and grape processors in New York and nearby regions, with losses reaching $8.8 million in three years (ref link). During short, high-volume harvest periods, post-harvesting facilities must remove SLF quickly, yet current methods continue to miss insects, risking contamination, and regulatory noncompliance. Without more effective post-harvest separation systems, facilities face rising financial risks and operational strain.

**Impact**  
Solving post-harvest SLF contamination would protect the entire wine supply chain. An effective removal system would help growers in New York preserve crop value while enabling processors to increase throughput, reduce labor, and lower losses, stabilizing supply for distributors and retailers. This keeps regional producers competitive, strengthens the broader agricultural economy, and ensures millions of consumers continue to access quality wine.

**Proposed Directions**

**Concept A:** Filtering Brushes  

**What it is:** A car wash like machine where motors will brush off the SLF on the conveyor belt. Brushes will be tuned in stiffness to be able to remove SLF while minimizing product loss.   

**How it would be used:**
* Grapes enter post-processing conveyor belt
* Product passes through brush module, where brushes knock SLF off of harvested grapes
* Grapes exit module and continue on conveyor belt. 

**Why it’s better than the status quo:**  
* This is a mechanically simple mechanism that could still prove to be effective.
* It is also easily integrated into pre-existing post-harvest processing conveyors. 

**End-of-semester proof-of-concept:** A simple motor mechanism with spinning brushes will model grapes and SLF, and a force gauge can test the force of the brush.

**Concept B:** Wind-Sorting Unit   

**What it is:** A controlled airflow module that removes lighter SLF from heavier grapes moving along a conveyor belt.  

**How it would be used:**  
* Grapes enter on a conveyor belt.
* Product passes through the wind-sorting mechanism, where airflow is used to blow SLF off the harvested grapes.
* Grapes exit on the conveyor belt and continue to be processed.  

**Why it’s better than the status quo:**  
* No direct contact with grapes is needed, so grapes will not be harmed during the process.
* The unit is easy to automate and integrate with existing processing equipment.  

**End-of-semester proof-of-concept:** We will build an airflow unit that uses small air guns or fans to blow SLF off the grapes. We can test the product by simulating SLF on grapes and using airspeed sensors to measure the force of air. 

**Key Risks / Unknowns**  
* Risk 1: For the car wash mechanism, there could be clogging near the walls of the conveyor belt or dead SLF laying on the conveyor belt passing through under the brushes. We will test this by comparing with existing processes.
* Risk 2: For the wind-sorting unit, airflow intensity and direction will need to be tuned to ensure grape quality does not degrade. We will test this by simulating grape processing and testing the airflow module under variable conditions.
* Risk 3: Both proposed solutions include the possibility of excessive grape removal or damage. We will test this by experimenting with different brush stiffnesses, rotation speeds, and airflow intensities.  

**Questions for the Client**  
1. Are SLF entering post-harvest processing primarily alive and intact, or dead and fragmented within the grape stream?  
*Decision affected:* Determines whether mechanical separation is viable or if removal must occur earlier, since fragmented SLF may be harder to remove.
2. What does a typical processing layout look like, and where would sanitation, space, or workflow constraints limit adding equipment?  
*Decision affected:* Defines integration limits so the design fits operational and regulatory realities, and supports solutions that can scale across facilities without major infrastructure changes.
3. Which forms of product damage are least acceptable (juice release, skin breakage, berry loss, or cluster disruption)? Please rank if possible.  
*Decision affected:* Sets force and contact limits, guiding mechanism selection and tuning so the design minimizes losses within acceptable damage tolerances.

**References**  
* https://news.cornell.edu/stories/2025/01/spotted-lanternflies-could-cost-nys-grape-industry-millions 

---

## Functional Prototype
<a name="functional-prototype"></a>

**Design Documentation**

Our functional prototype is a filtering brush mechanism designed to remove Spotted Lanternflies (SLF) from grapes during harvest processing. Grapes travel along a conveyor belt and pass beneath a rotating brush mounted above the product stream. The brush lightly contacts the grapes, applying enough force to dislodge SLF while minimizing grape damage and product loss.

**Key Components**
* Laser-cut acrylic mounting plates, bases, and supports (in-house fabrication)
* 1" diameter oak shaft (cut to 12 in.)
* Spiral-mounted strip brushes (1", 2", and 3" bristle lengths tested)
* Steel ball bearings (for rotational support)
* Hex bolt interface for drill-driven rotation

**Assembly Overview**
* Mount structure assembled using acrylic supports and adhesive  
* Oak shaft fitted with evenly spaced brush supports  
* Bearings press-fit onto shaft ends for smooth rotation  
* Strip brushes threaded in a spiral pattern along the shaft  
* System driven using a drill coupled to a hex bolt  

**Design Tests**

We evaluated our prototype through controlled experiments focused on brush performance and system stability.

**Test 1: Brush Length Optimization**

* **1” (stiffest):**  
  High SLF removal force, but caused significant grape displacement and potential damage.  

* **2” (moderate):**  
  Improved balance, but still caused occasional grape movement, especially at higher speeds.  

* **3” (most flexible):**  
  Consistently removed SLF while maintaining stable grape flow. Minimal displacement and best overall performance.

**Conclusion:**  
The 3” brush provided the best performance and will be used in future iterations.

**Test 2: Rotation Speed and Direction**

* **Clockwise rotation:** Effective SLF removal (up to 6/8 removed at higher speeds)  
* **Counterclockwise rotation:** Ineffective (0/8 removed consistently)  
* **Higher speeds (~2000 RPM):** Increased removal but caused mount instability (>5 mm movement)

**Conclusion:**  
* Clockwise rotation significantly improves SLF removal  
* Current mounting system lacks stability at high speeds  
* Future designs must improve structural rigidity and shaft alignment  

**Success Criteria**

“A machine that can be attached to current harvester conveyor belts to remove SLF from grapes during post-processing,” and:
* **≤ 5% grape damage**  
* **≥ 90% SLF removal in a single pass**  
* **Stable operation up to 2500 RPM (≤ 5 mm movement)**  
* **Adaptable brush geometry (≥ 90% debris clearance)**  
* **Operates at conveyor speeds of ~1 m/s**  

**How We Measure Success**
* Count SLF before and after passing through the prototype  
* Measure grape damage rate after processing  
* Track rotational speed (RPM) and mount displacement  
* Evaluate performance using a mock conveyor system  

**Key Takeaways**
* Brush flexibility is critical—longer bristles improve performance and reduce damage  
* Rotation direction significantly impacts SLF removal effectiveness  
* Structural stability is the main limitation of the current prototype  
* The concept is feasible and promising, with clear paths for refinement  