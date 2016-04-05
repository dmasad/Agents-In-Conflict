# Agents in Conflict: Comparative Agent-Based Modeling of International Crises and Conflicts
### David Masad
### Computational Social Science, George Mason University

This repository contains the code I used in my dissertation research, as well as the text of the dissertation itself. This code should help verify and explain the contents of the dissertation, but unfortunately is not all currently ready to be run as-is. However, all the missing input data files are publicly available, or can be regenerated using the provided code.


# Organization

## Code
The code used in the dissertation research.

### WarReason
Code for **Chapter 2: Learning and War**. 

#### consul
Contains the overall framework used for modeling collections of agents interacting via two-player, extensive-form games with perfect information. Also includes three decisionmaking models: rational play using subgame-perfect equilibrium moves, reinforcement learning, and case-based reinforcement learning.

#### models
Contains the runs and analysis for the two models presented in Chapter 2: the Simple Crisis (*crisis_game*) and the full International Interaction Game (*war_reason_model*).  The IIG code also requires the output generated by [EUGene](http://www.eugenesoftware.org/).

### ExpectedUtilityModel

Code for **Chapter 3: BDM's EUM as ABM** and **Chapter 4: Modeling the Cold War**. This includes my implementation and extensions to Bruce Bueno de Mesquita's Expected Utility Model, as described in Chapter 3.

# Dissertation Abstract

Inter-state conflicts are a key area of study in international relations, and have been approached with a variety of techniques, from case studies of individual conflicts, to formal analysis of abstract models and statistical investigations of all such conflicts. In particular, there are a variety of theories as to how states make decisions in the face of conflicts -- such as when to threaten force, when to follow through, and when to capitulate to an opponent's demand. Some scholars have argued that states may be viewed as rational decisionmakers, while others emphasize the role of psychological biases affecting individual leaders. Decisionmaking is challenging to study in part because of its complexity: the decisionmakers may not just be individuals but organizations, following internal procedures and reflecting institutional memory. Furthermore, the decisions are often believed to be strategic, reflecting the decisionmakers' anticipation of multiple other actors' potential responses to each possible decision.

In this dissertation, I demonstrate that agent-based models (ABMs) provide a powerful tool to address this complexity, and advance their use as a bridge between different methodologies. Agents in ABMs can be used to represent countries and endowed with a variety of internal decisionmaking models which can operationalize a variety of theories drawn from case studies, psychological experiments or game-theoretic analysis. The specific decision model agents utilize may be changed without altering the sub-models governing how the agents interact with one another. This allows us to simulate the same overall interactions utilizing different decisionmaking theories and observe how the outcomes differ. Furthermore, if these interactions correspond to real-world events, we may directly see how much explanatory or predictive power the outputs of the model variants provide. If one variant's outputs correspond closer to the empirical data, it provides evidence supporting that variant's underlying theory.

I implement two agent-based models, extending well-established prior models of international conflict: the International Interaction Game (Bueno de Mesquita and Lalman, 1992) and the Expected Utility Model (Bueno de Mesquita, 2002). For each, I start with their original agent decisionmaking models, and develop several variants grounded in relevant theories. I then instantiate the models with historic, empirically-derived data and run them forward to generate sets of simulated outcomes, which I compare to empirical data on the relevant time periods. I find that non-rational models of decisionmaking in the International Interaction Game provide similar explanatory power to the purely rational model, and yield rich satisficing behavior absent in the original model. I also find that the Expected Utility Model variant implementing a Schelling (1966)-inspired model of coercion yields richer dynamics and greater explanatory power than the original model.

