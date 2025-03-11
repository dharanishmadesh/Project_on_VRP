
# 🚗 Genetic Algorithm for Vehicle Routing Problem (VRP)

This project uses a **Genetic Algorithm (GA)** to solve the **Vehicle Routing Problem (VRP)**. The goal is to optimize the routes for multiple vehicles to visit a set of locations with minimal total distance and balance the load between vehicles.

## 📊 Overview

The project utilizes a Genetic Algorithm to:
- **Optimize vehicle routes**: Find the most efficient way for vehicles to visit a set of locations.
- **Balance the load**: Minimize the imbalance between the total distances traveled by each vehicle.

## 🚀 How to Run

### 1. **Clone this Repository**

To start, clone this repository using the command below:

```bash
git clone https://github.com/your-username/vehicle-routing-genetic-algorithm.git
cd vehicle-routing-genetic-algorithm
```

### 2. **Install Required Libraries**

Make sure you have the required libraries installed. Run the following command:

```bash
pip install matplotlib deap
```

### 3. **Run the Script**

You can run the `main.py` script to execute the Genetic Algorithm and optimize the vehicle routes:

```bash
python main.py
```

The script will:
- Generate random locations for the vehicles to visit.
- Use a genetic algorithm to optimize the total distance and balance the load among the vehicles.
- Visualize the optimal routes for each vehicle after the optimization.

## 🛠️ Features

- **Genetic Algorithm**: A GA with crossover, mutation, and selection operators.
- **Route Optimization**: Minimize the total distance traveled by the vehicles.
- **Balance Penalty**: Optimize the load between vehicles using a penalty based on the standard deviation of distances.

## 📈 Visualization

The script generates a plot showing:
- The locations (as blue dots).
- The depot (as a red square).
- The optimized routes for each vehicle.

## 📝 Example Output

After running the genetic algorithm, you will get a visualization of the optimal routes, similar to this:

- **Locations** will be plotted as blue dots.
- **Depot** will be plotted as a red square.
- **Routes** will be drawn for each vehicle.

## 🔧 Algorithm Details

The algorithm is based on a **Genetic Algorithm**:
- **Crossover**: Uses partially matched crossover (PMX) for permutation-based representations.
- **Mutation**: Shuffles the indices of locations with a probability of 5% for each index.
- **Selection**: Tournament selection with a tournament size of 3.

The goal of the genetic algorithm is to minimize:
1. **Total Distance**: The total distance traveled by all vehicles.
2. **Balance Penalty**: The imbalance between the total distance traveled by each vehicle (standard deviation).

## 📊 Plotting

The **plot_routes** function visualizes the best solution after the genetic algorithm has finished running. It plots the depot and locations, then draws the optimal route for each vehicle.

## 💡 Example Code Flow

### Task 1 - Setup Locations and Vehicles
- Randomly generate locations (coordinates) and set the depot at a fixed point.

### Task 2 - Genetic Algorithm Setup
- Use DEAP to define a genetic algorithm for optimizing routes.

### Task 3 - Fitness Evaluation
- Fitness is evaluated based on the total distance and the balance between vehicle routes.

### Task 4 - Visualize the Solution
- After running the algorithm, the best route is displayed using `matplotlib`.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Author

- **Your Name**  
  GitHub: [@your-username](https://github.com/your-username)
```

### Key Sections in the README:
1. **Project Overview** with the goal of solving the VRP.
2. **How to Clone and Run** the repository.
3. **Installation Instructions** for dependencies.
4. **Features** of the Genetic Algorithm and the Vehicle Routing Problem.
5. **Visualization Details** about plotting the optimal routes.
6. **Algorithm Details** explaining the genetic algorithm setup.
7. **License and Author** sections.

Feel free to modify and personalize the content based on your specific details, including your GitHub username and any additional project information!
