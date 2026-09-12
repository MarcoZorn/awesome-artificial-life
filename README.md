# Awesome Artificial Life [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

> Software, simulators and research about systems that are alive enough to surprise you.

Artificial life asks what living systems do rather than what they are made of. The
same question turns up as cellular automata, evolved creatures, swarms, growing
neural networks and open-ended sandboxes with no goal at all. This list collects
the things you can actually run, read and learn from.

Every entry here has been opened and checked. Nothing is listed because it sounds
impressive.

## Contents

- [Simulators and sandboxes](#simulators-and-sandboxes)
- [Cellular automata and continuous life](#cellular-automata-and-continuous-life)
- [Neuroevolution](#neuroevolution)
- [Evolutionary computation](#evolutionary-computation)
- [Quality diversity and open-endedness](#quality-diversity-and-open-endedness)
- [Swarms and collective behaviour](#swarms-and-collective-behaviour)
- [Run it in a browser](#run-it-in-a-browser)
- [Biology-grade simulation](#biology-grade-simulation)
- [Papers](#papers)
- [Books](#books)
- [Communities and events](#communities-and-events)
- [Contributing](#contributing)

## Simulators and sandboxes

Worlds you start and then watch.

- [ALIEN](https://github.com/chrxh/alien) - CUDA-powered particle physics world where self-replicating machines emerge from soup. Probably the most visually spectacular ALife project in existence. C++/CUDA.
- [biosim4](https://github.com/davidrmiller/biosim4) - Small creatures with evolved neural wiring solve spatial survival challenges on a grid. Famous for the accompanying video that explains every line. C++.
- [primordial](https://github.com/MarcoZorn/primordial) - Dish of identical cells with two independently mutating genomes and no fitness function anywhere in the codebase. Organisms only have to stay solvent long enough to divide. Python.
- [ecosim](https://github.com/connor-brooks/ecosim) - Interactive predator/prey ecosystem you can poke while it runs. C and OpenGL.
- [Creatures](https://github.com/thopit/Creatures) - Evolution simulator with physical bodies and energy budgets. Java.
- [Avida](https://github.com/devosoft/avida) - Digital evolution platform used in peer-reviewed evolutionary biology for two decades. Self-replicating programs mutate and compete for CPU time. C++.

## Cellular automata and continuous life

- [Lenia](https://github.com/Chakazul/Lenia) - Continuous generalisation of the Game of Life. Produces smooth, gliding, unmistakably creature-like patterns. The reference implementation from the paper's author. Python/JS.
- [lenia_ca](https://github.com/BirdbrainEngineer/lenia_ca) - Fast Lenia core in Rust, for when the Python version is the bottleneck.
- [Growing Neural Cellular Automata](https://github.com/google-research/self-organising-systems) - Cells that learn, by gradient descent, to grow into a target shape and repair it when you cut it in half. From the Distill article.
- [Growing NCA in PyTorch](https://github.com/chenmingxiang110/Growing-Neural-Cellular-Automata) - Clean standalone reproduction, easier to read than the original.
- [physarum](https://github.com/fogleman/physarum) - Slime mold transport networks from three simple agent rules. The output looks like it was grown, not rendered. Go.
- [interactive-physarum](https://github.com/Bleuje/interactive-physarum) - Real-time physarum you can steer with your mouse.
- [slime-sim-webgpu](https://github.com/SuboptimalEng/slime-sim-webgpu) - Same idea on the GPU via WebGPU. TypeScript.
- [particle-life](https://github.com/hunar4321/particle-life) - Four particle types, an attraction matrix, and nothing else. Cells, membranes and chasing behaviour fall out anyway.

## Neuroevolution

Evolving the network instead of training it.

- [neat-python](https://github.com/CodeReclaimers/neat-python) - The standard Python NEAT implementation. Where most people start.
- [tensorneat](https://github.com/EMI-Group/tensorneat) - NEAT on the GPU via JAX. Orders of magnitude faster populations.
- [MultiNEAT](https://github.com/peter-ch/MultiNEAT) - Portable C++ NEAT with HyperNEAT and ES-HyperNEAT, Python bindings included.
- [SharpNEAT](https://github.com/colgreen/sharpneat) - Mature, carefully engineered NEAT for .NET. Worth reading even if you write no C#.
- [PyTorch-NEAT](https://github.com/uber-research/PyTorch-NEAT) - Bridges NEAT genomes to PyTorch networks, including adaptive HyperNEAT.
- [deep-neuroevolution](https://github.com/uber-research/deep-neuroevolution) - Uber AI's distributed GA and evolution strategies code showing that plain genetic algorithms can train deep networks for Atari.
- [neataptic](https://github.com/wagenaartje/neataptic) - Neuroevolution in the browser with an architecture-free API. Unmaintained but still the easiest JS starting point.
- [neat-from-scratch](https://github.com/MarcoZorn/neat-from-scratch) - NEAT implemented from nothing in dependency-free JavaScript, with a live browser demo, a running view of the leader's network, and tracks you draw yourself. Written to be read.
- [cars](https://github.com/MarcoZorn/cars) - NEAT drives cars around procedurally generated tracks using only raycast distances. No hand-written driving logic. Python.
- [Cephalopods](https://github.com/jobtalle/Cephalopods) - Evolved swimming squids. A good example of body and controller evolving together.

## Evolutionary computation

General-purpose engines you can point at anything.

- [DEAP](https://github.com/DEAP/deap) - Distributed evolutionary algorithms in Python. Genetic programming, strategies, multi-objective, all explicit rather than hidden behind a facade.
- [PyGAD](https://github.com/ahmedfgad/GeneticAlgorithmPython) - Genetic algorithms with a gentle API and Keras/PyTorch integration.
- [evosax](https://github.com/RobertTLange/evosax) - Evolution strategies in JAX. CMA-ES, OpenES, and thirty more, all jittable.
- [EvoJAX](https://github.com/google/evojax) - Hardware-accelerated neuroevolution toolkit from Google Brain.
- [nevergrad](https://github.com/facebookresearch/nevergrad) - Gradient-free optimisation platform from Meta. Useful as a baseline harness.
- [estool](https://github.com/hardmaru/estool) - Compact evolution strategies reference that accompanies David Ha's writing on the topic.

## Quality diversity and open-endedness

Searching for a wide collection of good solutions instead of one best one.

- [pyribs](https://github.com/icaros-usc/pyribs) - Bare-bones quality diversity library. MAP-Elites and CMA-ME without the framework tax.
- [QDax](https://github.com/adaptive-intelligent-robotics/QDax) - Accelerated quality diversity on JAX, built for massive parallel evaluation.
- [pymap_elites](https://github.com/resibots/pymap_elites) - The reference MAP-Elites implementation from the authors of the Nature paper.
- [POET](https://github.com/uber-research/poet) - Paired Open-Ended Trailblazer. Co-evolves problems alongside the agents that solve them, so the curriculum never runs out.
- [Darwin Godel Machine](https://github.com/jennyzzt/dgm) - Agents that rewrite their own code and keep an archive of every ancestor. Open-ended evolution applied to software rather than organisms.

## Swarms and collective behaviour

- [Boids](https://github.com/SebLague/Boids) - Reynolds flocking with a readable Unity implementation and a companion video.
- [boids](https://github.com/beneater/boids) - The whole algorithm in about a hundred lines of JavaScript, annotated. The best possible introduction.
- [Ecosystem-2](https://github.com/SebLague/Ecosystem-2) - Foxes, rabbits and grass, plus every unintended equilibrium that follows.

## Run it in a browser

No install, no build step.

- [Evolution](https://github.com/keiwando/evolution) - Build a creature from bones and muscles, then watch evolution teach it to walk. Also on the web and mobile.
- [FlappyLearning](https://github.com/xviniette/FlappyLearning) - Neuroevolution learning Flappy Bird in a single HTML file. Still one of the clearest demos ever made.
- [evolution-simulator](https://github.com/minutelabsio/evolution-simulator) - Minute Labs' creature simulator from their video on natural selection.
- [evolutionSimulator](https://github.com/adityathebe/evolutionSimulator) - Box2D creatures evolving locomotion in the browser.
- [Koi Farm](https://github.com/jobtalle/Koi) - Breeding game with a real genetics model underneath the pretty fish.

## Biology-grade simulation

Where artificial life meets actual wet biology.

- [OpenWorm](https://github.com/openworm/OpenWorm) - Ongoing effort to simulate C. elegans, all 302 neurons and the body they drive, from the bottom up.
- [dm_control](https://github.com/google-deepmind/dm_control) - DeepMind's physics-based continuous control stack. The standard substrate for evolved and learned bodies.

## Papers

- Conway's Game of Life, popularised by Martin Gardner, Scientific American (1970) - the origin of the whole field's intuition.
- Reynolds, [Flocks, Herds, and Schools: A Distributed Behavioral Model](https://www.red3d.com/cwr/papers/1987/boids.html) (1987) - three rules, one flock.
- Langton, *Artificial Life* (1989) - the proceedings that named the field.
- Ray, *An Approach to the Synthesis of Life* (1991) - Tierra, self-replicating code that evolved parasites nobody designed.
- Sims, [Evolving Virtual Creatures](https://www.karlsims.com/papers/siggraph94.pdf) (1994) - morphology and control evolved together. Thirty years on it is still the reference everyone reaches for.
- Bedau et al., *Open Problems in Artificial Life* (2000) - the field's own list of what it cannot yet do.
- Stanley and Miikkulainen, [Evolving Neural Networks through Augmenting Topologies](https://nn.cs.utexas.edu/downloads/papers/stanley.ec02.pdf) (2002) - the NEAT paper.
- Ofria and Wilke, *Avida: A Software Platform for Research in Computational Evolutionary Biology* (2004).
- Stanley, *Compositional Pattern Producing Networks* (2007) - encoding structure as a function of geometry.
- Stanley, D'Ambrosio and Gauci, *A Hypercube-Based Encoding for Evolving Large-Scale Neural Networks* (2009) - HyperNEAT.
- Lehman and Stanley, [Abandoning Objectives: Evolution Through the Search for Novelty Alone](https://www.cs.swarthmore.edu/~meeden/DevelopmentalRobotics/lehman_ecj11.pdf) (2011) - the paper that made "no fitness function" a serious position.
- Mouret and Clune, [Illuminating Search Spaces by Mapping Elites](https://arxiv.org/abs/1504.04909) (2015) - MAP-Elites.
- Wang et al., [POET](https://arxiv.org/abs/1901.01753) (2019) - endlessly generating new environments and their solutions.
- Chan, [Lenia: Biology of Artificial Life](https://arxiv.org/abs/1812.05433) (2019).
- Mordvintsev et al., [Growing Neural Cellular Automata](https://distill.pub/2020/growing-ca/) (2020) - interactive, and the best-explained paper on this list.

## Books

- Steven Levy, *Artificial Life: A Report from the Frontier Where Computers Meet Biology* (1992) - the field as it felt when it was new.
- Gary William Flake, *The Computational Beauty of Nature* (1998) - fractals, chaos, CA and adaptation, with code.
- Melanie Mitchell, *Complexity: A Guided Tour* (2009) - the clearest account of why simple rules produce hard-to-predict systems.
- Kenneth Stanley and Joel Lehman, *Why Greatness Cannot Be Planned* (2015) - novelty search argued as a general principle rather than an algorithm.

## Communities and events

- [ISAL](https://alife.org) - International Society for Artificial Life, which runs the annual ALIFE conference.
- [Artificial Life](https://direct.mit.edu/artl) - the MIT Press journal, the field's journal of record.
- [r/alife](https://www.reddit.com/r/alife/) - small, active, and consistently higher signal than its size suggests.
- [Complexity Explorer](https://www.complexityexplorer.org/) - free Santa Fe Institute courses on complex systems, CA and evolution.

## Related lists

- [awesome-deep-neuroevolution](https://github.com/Alro10/awesome-deep-neuroevolution) - deep learning flavoured neuroevolution, more papers than software.

## Contributing

Pull requests welcome. One rule: open it, run it if it runs, and write the line
that tells a reader why it is worth their evening. See [CONTRIBUTING.md](CONTRIBUTING.md).
