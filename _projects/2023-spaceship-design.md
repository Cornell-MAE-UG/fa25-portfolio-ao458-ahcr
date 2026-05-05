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
- [Client Report](#client-report)

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

**Design Documentation**. 
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

**Test 1: Brush Length Optimization**. 
* **1” (stiffest):**  
  High SLF removal force, but caused significant grape displacement and potential damage.    
* **2” (moderate):**  
  Improved balance, but still caused occasional grape movement, especially at higher speeds.    
* **3” (most flexible):**  
  Consistently removed SLF while maintaining stable grape flow. Minimal displacement and best overall performance.  
**Conclusion:**  
The 3” brush provided the best performance and will be used in future iterations.

**Test 2: Rotation Speed and Direction**. 
* **Clockwise rotation:** Effective SLF removal (up to 6/8 removed at higher speeds)  
* **Counterclockwise rotation:** Ineffective (0/8 removed consistently)  
* **Higher speeds (~2000 RPM):** Increased removal but caused mount instability (>5 mm movement)

**Conclusion:**  
* Clockwise rotation significantly improves SLF removal  
* Current mounting system lacks stability at high speeds  
* Future designs must improve structural rigidity and shaft alignment  

**Success Criteria**. 
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

---

## Client Report
<a name="client-report"></a>

**Context and Problem Statement**. 
During short, high-volume harvest periods, facilities must remove spotted lantern flies (SLFs) quickly, yet current methods continue to miss insects, risking contamination and regulatory noncompliance, which can lead to financial and operational strain. There are three opportunities to remove SLF: before, during, and after harvest processing. Our approach is implemented during the harvesting stage, when there is minimal grape juice on the conveyor. Operating at this point minimizes product loss, improves removal efficiency, and maintains compatibility with high-throughput processing conditions. The conveyor is also a single point where all harvested grapes pass though. By looking for solutions to apply at this stage, we reduce the number of devices needed to effectively remove SLF. 

**Final Prototype and Application**. 
Our concept is a filtering brush mechanism designed to remove SLF from grapes during the harvesting processing. Grapes will travel along the harvesting machine’s conveyor belt and pass through a rotating brush placed above. The brush will lightly contact the product stream, applying enough force to knock off the SLF from the grapes. Our prototype is designed to integrate directly with the conveyor rails via mounting brackets specifically fitted to the conveyor dimensions. It can be installed as an inline module within the harvesting process, operating continuously as grapes are transported through the processing line.

**Success Criteria**. 
Our design was a rotary brush tool that can be attached to current harvester conveyor belts to remove SLF from grapes just harvested from vines. The criteria we sought out was to ensure:
* The brushes should not damage, crush, or visibly harm more than 5% of grapes. Our clients have emphasized product loss as a major problem in current SLF removal systems.
* The brushes should be tuned to remove at least 90% of SLF from grapes in a single pass. High removal rates are a high priority to prevent product rejection.
* The system should be able to withstand realistic operation without shifting more than 5mm. Greater stability is a medium priority.
* The system should be able to process grapes on a conveyor belt at a speed of 1 m/s. Higher speeds are a medium priority.

**Testing and Results**. 
Our initial prototype consisted of food grade brushes rotating on a wooden dowel that is driven by a standard hand held drill. It is mounted above a conveyor system to simulate harvesting conditions. The main mechanical risks involve brush motion and structural stability. The following tests allowed us to identify three factors which strongly impacted performance: brush length, rotation speed, and rotation direction. During testing we made a mock conveyor belt and modeled grapes out of clay, each of the approximate weight of a grape (5-7g). We modeled SLF with loops of masking tape, approximating their weight and clinging tendency. Using the cordless drill to drive the brushes, we measured how many SLF were knocked off and how much our mounting moved. By changing the direction of the drill, we also tested whether a clockwise or counterclockwise brush rotation was more effective for SLF removal. Our testing highlighted several areas in need of improvement. For drill speeds >500 RPM, our prototype started shifting, indicating a need for a sturdier, more robust mounting design. As we deduced that 2000 RPM in the clockwise direction, as that least impacted the flow of the grapes, removed the most SLF, we needed sturdier mounts on future prototypes. We measured the grape flow and grape health more qualitatively, relative to each other. Unfortunately we could not simulate enough tests to come up with concrete numbers, however the testing was still fruitful. The 3” brush was identified as the most effective choice, as shown in Table 2, which should also be integrated in future configurations.

**Final Prototype**. 
The initial prototype established baseline estimates for dimensions, operating speed, and overall feasibility. The final prototype builds on this by closely replicating a real harvester conveyor system with an integrated rotary brush mechanism. A mock conveyor section was constructed with dimensions similar to an actual harvesting belt, using food-grade materials for the belt and brushes, along with 3D-printed components. The mounts are machined from aluminum, enabling precise placement within a 0.010-inch tolerance and ensuring structural stability. The system is driven by a 3000 RPM motor paired with a speed controller, allowing fine adjustment of operating speed to meet specific testing requirements. Reevaluation of mounting stability showed that for 2000 RPM operating speeds, the mounting did not shift. Additionally, the final prototype incorporates a shaft with an internal helical channel for mounting the brushes. This design increases stability by maximizing the brush mounting surface area. In contrast, the first prototype used four externally attached rod supports (shown in Figure 2), whereas the final design provides a continuous mounting interface.

**Conclusion and Reccomendation**. 
We researched the already existing harvesters and found the OXBO 6030 was already equipped with PREMIUMDESTEM and PREMIUMSORT technology that included a majority of what our product was trying to achieve. Therefore, as our results prove that the brush mechanisms are indeed brushing off SLF with increased success and efficiency, further improvements can be made to the already established technology. Future iterations should explore incorporating multiple brush stages with varying stiffness or rotational speeds to improve removal efficiency while minimizing damage to the grapes. Introducing a staged approach would allow for more controlled, gradual removal of SLF across the process. A practical implementation should include an integrated cleaning mechanism to prevent debris buildup and brush clogging, ensuring consistent performance and reducing maintenance requirements over time. Software-based control can also improve performance significantly; for example, a closed-loop feedback system, using vision-based sensors, could enable real-time adjustment brush speeds/torque based on SLF presence. 



