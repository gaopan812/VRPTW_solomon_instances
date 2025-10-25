# VRPTW Solomon Instances

Standard VRPTW benchmark datasets from [Solomon (1987)](https://neo.lcc.uma.es/vrp/vrp-instances/capacitated-vrp-with-time-windows-instances/) in JSON format.

## 📂 Dataset Structure

- `solomon_25/`, `solomon_50/`, `solomon_100/`: Number of customers.
- Each JSON file contains:
  - `vehicle.number`: Available vehicles
  - `vehicle.capacity`: Vehicle capacity
  - `customers[]`: List of nodes (0 = depot)
    - `id`, `x`, `y`: Node ID and coordinates
    - `demand`: Cargo demand
    - `ready_time`, `due_time`: Time window [a, b]
    - `service_time`: Service duration

## 🧩 Instance Types

- **C-type**: Clustered customers (urban-like)
- **R-type**: Randomly distributed (rural-like)
- **RC-type**: Mixed distribution


## 📚 Source
Original data: [Solomon Benchmark Problems](https://neo.lcc.uma.es/vrp/vrp-instances/capacitated-vrp-with-time-windows-instances/)

> This project is a format conversion. The data belongs to M.M. Solomon (1987).