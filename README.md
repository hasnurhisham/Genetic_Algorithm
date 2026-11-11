Genetic Algorithm Web Application (Streamlit)

A web-based interactive application built with Streamlit and Python to visualize and analyze the execution of Genetic Algorithms (GA) on binary bitstrings and continuous real-valued benchmark functions.

Developed as part of the assessment for BSD3513: Introduction to Artificial Intelligence at Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA).

🔗 Project Links

Live Streamlit App: https://ga-lab2-hasnur.streamlit.app

GitHub Repository: https://github.com/hasnurhisham/Genetic-Algorithm

📌 Problem Overview (Lab 2 Requirements)

This project satisfies the custom optimization constraints of Lab Report 2 (Question 2):

Population Size: $N = 300$ individuals.

Chromosome Length: 80 bits.

Generations: 50 generations.

Target Objective: Custom fitness function reaching its global maximum score of 80.0 when the number of ones in the chromosome is equal to 50.

Mathematically, the custom OneMax fitness assignment is expressed as:

$$f(x) = 80 - \vert{}\text{count\_ones}(x) - 50\vert{}$$

✨ Features

Custom Fitness Function: Targets exact binary pattern constraints ($50 \text{ ones} \rightarrow \text{Fitness} = 80.0$).

Real-Time Live Charting: Tracks Best, Average, and Worst population fitness across generations.

Support for Multiple Benchmark Functions: Includes binary OneMax as well as real-valued continuous functions (Sphere and Rastrigin).

Configurable GA Parameters: Easily tune population size, generations, crossover rate, mutation rate, tournament selection size, and elitism directly from the sidebar.

Population Snapshot: Allows users to inspect the final population table and individual fitness scores.

🛠️ Project Structure

├── GA_streamlit.py       # Main Streamlit application and GA logic
├── requirements.txt      # Required dependencies for Streamlit Community Cloud
└── README.md             # Project documentation


🚀 Local Setup & Installation

Follow these steps to run the application locally on your machine:

1. Clone the Repository

git clone https://github.com/hasnurhisham/Genetic-Algorithm.git
cd Genetic-Algorithm


2. Set Up Virtual Environment (Optional but Recommended)

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate


3. Install Dependencies

pip install -r requirements.txt


4. Run the Streamlit App

streamlit run GA_streamlit.py


📦 Dependencies (requirements.txt)

Ensure your repository contains a requirements.txt file with the following packages:

streamlit>=1.30.0
numpy>=1.24.0
pandas>=2.0.0


📊 Experimental Results

When executed with the lab parameter configuration (80 bits, 300 population, 50 generations):

Target Fitness Achieved: 80.000000

Optimal Chromosome: Contains exactly 50 ones and 30 zeros ($\sum_{i=1}^{80} x_i = 50$).

Convergence Behavior:

Best Fitness maintains the optimal solution via elitism.

Average Fitness rapidly converges from ~70.0 to ~78.5 due to tournament selection and crossover.

Worst Fitness demonstrates continuous variance due to bit mutation, preventing premature stagnation.

