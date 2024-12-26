# Pandemic Control System

This project is a simulation of a pandemic control system using various algorithms and data structures. It helps in managing the spread of infection, allocating medical resources, and visualizing the state of the pandemic.

## Features

- **Infection Rate Calculation**: Calculate the infection rate for a given state.
- **Medical City Services**: Find the nearest medical city and service cities within a state.
- **Graph Algorithms**: Identify bridges and articulation points in the network of cities.
- **Resource Management**: Allocate supplies to states and evacuate cities.
- **Visualization**: Visualize the network of cities and the spread of infection.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/pandemic-control-system.git
    ```
2. Navigate to the project directory:
    ```sh
    cd pandemic-control-system
    ```
3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Run the main script:
    ```sh
    python pandemicControl.py
    ```
2. Provide input through the  file. The file should contain commands in the following format:
    ```plaintext
    nearest_medical_city CityA1
    infection_rate StateA
    find_bridges
    find_articulation_points
    service_city StateA
    get_max_state
    generate_report StateA
    evacuate_city CityA2
    supply_state 5000 StateA
    reach_all_cities StateA
    visualisation
    ```

## File Structure

- : Main script containing the logic for the pandemic control system.
- : Sample input file with commands to be executed.
- `requirements.txt`: List of dependencies required for the project.

## Classes and Methods

### 

Represents a state node with the following attributes:
- : Name of the state.
- : Population of the state.
- : Number of infected individuals.
- : List for heap representation.
- : List for graph representation of the cities in a state.
- : List of medical cities.
- : Edge list representation of the neighboring states.
- : Most infected city in the state.
- : Available supplies in the state.

### Methods

- `nearest_medical_city(city)`: Finds the nearest medical city to the given city.
- `infection_rate(state)`: Calculates the infection rate for the given state.
- `find_bridges()`: Identifies bridges in the network of cities.
- `find_articulation_points()`: Identifies articulation points in the network of cities.
- `service_city(state)`: Services the cities within the given state.
- `get_max_state()`: Gets the state with the maximum infection rate.
- `generate_report(state)`: Generates a report for the given state.
- `evacuate_city(city)`: Evacuates the given city.
- `supply_state(amount, state)`: Supplies the given amount to the state.
- `reach_all_cities(state)`: Ensures all cities in the state are reachable.
- `visualisation()`: Visualizes the network of cities and the spread of infection.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
