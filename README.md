# AI Search & Inference Algorithms 🤖

> Artificial Intelligence coursework implementations in R - Uppsala University

## 📖 About

Two classic AI algorithm implementations developed for the Artificial Intelligence course at Uppsala University (HT2023). The projects demonstrate pathfinding optimization and probabilistic reasoning using real-world simulation environments.

## 🎯 Projects

### 1. Delivery Man - A* Pathfinding
**File:** `delivery_man_a_star.r`

Implementation of the A* search algorithm for optimal package delivery routing in a city grid with variable traffic conditions.

**Features:**
- A* pathfinding with Manhattan distance heuristic
- Dynamic goal selection (pickup vs delivery)
- Traffic-aware cost calculation
- Optimal route planning in 10x10 grid environment

**How it works:**
- Finds nearest undelivered package using Manhattan distance
- Calculates optimal path considering traffic on vertical and horizontal roads
- Uses priority queue (frontier) to explore lowest-cost paths first
- Returns next move direction for the delivery car

**Package:** Uses the `DeliveryMan` simulation environment

---

### 2. Where's Croc - Hidden Markov Model
**File:** `croc.r`

Bayesian inference implementation using Hidden Markov Models to track and capture a crocodile based on noisy sensor readings.

**Features:**
- Hidden Markov Model for state estimation
- Sensor fusion (salinity, phosphate, nitrogen readings)
- Transition matrix for croc movement prediction
- Breadth-first search for navigation

**How it works:**
- Builds transition matrix modeling crocodile movement between waterholes
- Uses Gaussian emissions from three sensors to estimate croc location
- Applies Bayes' rule to update probability distribution
- Searches for optimal path to most likely location

**Package:** Uses the `WheresCroc` game environment

## 🛠️ Technologies

- **Language:** R
- **Algorithms:** A* Search, Hidden Markov Models, Breadth-First Search
- **Concepts:** Heuristic search, probabilistic inference, pathfinding

## 💻 Usage

### Prerequisites
```r
install.packages("DeliveryMan")
install.packages("WheresCroc")
```

### Running A* Delivery Man
```r
source("delivery_man_a_star.r")
# Use myFunction with DeliveryMan package
```

### Running Where's Croc
```r
source("croc.r")
# Use myFunction with WheresCroc package
```

## 🔑 Key Concepts

- **A* Algorithm:** Informed search using g(n) + h(n) cost function
- **Manhattan Distance:** Heuristic for grid-based pathfinding
- **Hidden Markov Models:** Statistical model for sequential data with hidden states
- **Bayesian Inference:** Updating beliefs based on evidence
- **State Space Search:** Exploring possible states to reach goals

## 🎓 Academic Context

**Institution:** Uppsala University  
**Course:** Artificial Intelligence (HT2023)  
**Authors:** Gabrielle Fidelis de Castilho, Hemavathi Hanasoge Siddaiah, Kim Kuruvilla Mathews
**Topics:** Search algorithms, probabilistic reasoning, game AI
