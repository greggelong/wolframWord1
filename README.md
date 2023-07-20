# Wolfram mapping words to neighborhood states

how about mapping a one dimensional cellular automata to words 

ChatGPT
Mapping a one-dimensional cellular automaton to words can be an interesting and unique creative coding project. Cellular automata are computational models that exhibit fascinating emergent behaviors from simple rules applied to a grid of cells. By associating words with specific cell states, you can create dynamic and meaningful visualizations. Here's a general outline to get you started:

Project Concept: Word Automata

Overview:
Word Automata is a creative coding project that represents a one-dimensional cellular automaton using words. Each cell state corresponds to a word, and the evolution of the automaton generates meaningful visual patterns from simple rules.

I talked with chat GPT about it, great for getting ideas, but total crap for producing usable code. All code except for word arrays are from me and my past influences.  

Let's represent cell states with binary digits: 0 for "off" or "dead," and 1 for "on" or "alive."

111: 111 represents the configuration when the current cell and both of its neighbors are alive (1). (e.g., "Alive-Alive-Alive")

110: 110 represents the configuration when the current cell is alive (1), and both of its neighbors are dead (0). (e.g., "Alive-Alive-Dead")

101: 101 represents the configuration when the current cell is alive (1), its left neighbor is alive, and the right neighbor is dead. (e.g., "Alive-Dead-Alive")

100: 100 represents the configuration when the current cell is alive (1), and both of its neighbors are dead (0). (e.g., "Alive-Dead-Dead")

011: 011 represents the configuration when the current cell is dead (0), and both of its neighbors are alive (1). (e.g., "Dead-Alive-Alive")

010: 010 represents the configuration when the current cell is dead (0), and its left neighbor is alive while the right neighbor is dead. (e.g., "Dead-Alive-Dead")

001: 001 represents the configuration when the current cell is dead (0), and its left neighbor is dead while the right neighbor is alive. (e.g., "Dead-Dead-Alive")

000: 000 represents the configuration when the current cell and both of its neighbors are dead (0). (e.g., "Dead-Dead-Dead")

 ```javascript
 const wordMapping = [
  "自",  // Nature (Zì)
  "技",  // Technology (Jì)
  "艺",  // Art (Yì)
  "科",  // Science (Kē)
  "和",  // Peace (Hé)
  "战",  // War (Zhàn)
  "梦",  // Dream (Mèng)
  "实",  // Reality (Shí)
];
 
 ```