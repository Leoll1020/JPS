---
layout: default
title: Proposal
---

## PROPOSAL FOR CS175 AI PROJECT
#### Met with professor on May 1, 2017


### Summary for Project

For our project, we chose our agent to solve a Jumping Puzzle. The Jumping Puzzle has a start and <br />
a destination block. The agent must get from the start to the destination block. However, unlike <br />
regular mazes, mazes in the Jumping Puzzle have missing blocks that the agent can fall through. The <br />
agent must avoid these gaps and successfully reach the destination block. Our input semantics will <br />
be the generated maze mission. The agent will not be aware of its environment and only has information <br />
about the current state. The output of each mission will be the path the agent found and a cost of <br />
the path the agent found from the optimal path. <br />

The ability for a character to jump is a key mechanism in many successful games. Jumping Puzzles <br />
takes this mechanism to a whole new level in which the player's knowledge of where to jump and <br />
when to jump can decide whether they pass the level or not. Games like Guild Wars and Assassin's <br />
creed implement this feature to some extent while games like Super Mario are based entirely on <br />
Jumping Puzzles. A Jumping Puzzle AI would allow game developers to test whether a Jumping Puzzle <br />
is able to be completed/whether it is too easy or hard. The field of robotics is fairly new but that <br />
doesn't stop researchers from having visions of robots saving people from catastrophes or fighting <br />
in wars in place of humans. Like Minecraft, the real world is not just flat lands. If a robot is <br />
going to perform those functions, it will need to be able to, not only walk, but to learn to climb <br />
and maybe even jump! That is why we find a Jumping Puzzle AI to be very interesting and we hope to <br />
potentially unearth many more applications it has on the world. <br />
    
### AI/ML Algorithms

We plan on using Monte Claro Policy Evaluation to find the optimal path of a puzzle. We then hope to <br /> 
use reinforcement learning to train our agent on the optimal path to be able to solve any Jumping Puzzle. <br />
    
### Evaluation Plans

Based on the optimal path and the path given by our agent at the end of the mission, we calculate <br />
the cost of the generated path. The reinforcement learning will optimize the cost and converge to <br />
an optimal value. To verify that our algorithm works, we will measure the error at each iteration <br />
and see whether it decreases monotonically and whether it converges to a final value. <br />

To verify if our agent is properly trained, we will give it a puzzle it has never seen before and <br />
ask it to solve it. We will consider the project a success if the cost generated is within a threshold <br />
from the optimal path. As a sanity case, we will use a simple maze. It will likely have a small number <br />
of blocks and a few missing blocks. It would not have to find the optimal path but only be able to solve <br />
the puzzle. Our moonshot case is solving a large puzzle with sparse blocks that have large gaps between <br />
blocks. It would find the optimal path. <br />
