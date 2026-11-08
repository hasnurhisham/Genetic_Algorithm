# 🧬 Genetic Algorithm – Bit Pattern Optimisation

**Artificial Intelligence | Lab Report 2 – Search Algorithms**

## Project Overview

This project demonstrates the implementation of a Genetic Algorithm (GA) to optimise binary bit patterns using evolutionary computation. Inspired by natural selection, the algorithm evolves a population of candidate solutions through selection, crossover, and mutation to search for an optimal chromosome.

The main objective is to generate an 80-bit chromosome containing exactly 50 ones, which corresponds to the maximum fitness value of 80.

## Problem Definition

The Genetic Algorithm is configured according to the following assignment requirements:

| Parameter | Value |
|---|---|
| Population size | 300 |
| Chromosome length | 80 bits |
| Target number of ones | 50 |
| Maximum fitness value | 80 |
| Number of generations | 50 |
| Chromosome representation | Binary (0 and 1) |

The optimisation aims to identify a chromosome that satisfies the target number of ones while maximising its fitness score.

## Genetic Algorithm Methodology

The Genetic Algorithm follows an evolutionary optimisation process:

1. **Population Initialisation:** Generate an initial population of 300 binary chromosomes, each containing 80 bits.
2. **Fitness Evaluation:** Calculate the fitness of each chromosome according to its number of ones. The highest possible fitness is 80 when exactly 50 ones are present.
3. **Selection:** Select chromosomes for reproduction based on their fitness.
4. **Crossover:** Combine genetic information from selected parent chromosomes to produce offspring.
5. **Mutation:** Introduce random changes to selected bits to maintain genetic diversity.
6. **Replacement:** Form the next generation using the offspring and the replacement strategy.
7. **Termination:** Repeat the evolutionary process for up to 50 generations and report the best solution obtained.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Genetic Algorithm implementation |
| Streamlit | Interactive web application |
| GitHub | Source code hosting and version control |
| VS Code | Development environment |

## Installation and Setup

### Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

### Install Dependencies

```bash
python3 -m pip install -r requirements.txt
```

### Run the Application

```bash
python3 -m streamlit run app.py
```

The application will typically open at `http://localhost:8501`.

## Results and Output

The application is intended to demonstrate the evolutionary optimisation process by displaying the resulting bit pattern and its fitness value.

The main outputs to document are:

- Best chromosome obtained.
- Number of ones in the best chromosome.
- Best fitness value.
- Generation at which the best solution was identified.
- Fitness progression across generations, if implemented.

A successful optimal solution contains exactly 50 ones and achieves a fitness score of 80.

## Application Screenshots

Include screenshots demonstrating the actual application and results.

Suggested screenshots:

- Genetic Algorithm configuration.
- Best chromosome and fitness score.
- Fitness progression graph, if available.

## Deployment

**Live Application:** [Insert your deployed Streamlit URL]

**GitHub Repository:** [Insert your repository URL]

## Limitations

Genetic Algorithms are stochastic optimisation methods, meaning their results may vary between runs. Their performance depends on the fitness function, selection mechanism, crossover and mutation settings, and number of generations. Therefore, the algorithm is not guaranteed to identify the optimal solution in every run.

## Project Information

**Course:** BSD3513 Artificial Intelligence  
**Assessment:** Lab Report 2 – Search Algorithms  
**Topic:** Genetic Algorithm  
**Developer:** [Your name]  
**Institution:** Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA)
