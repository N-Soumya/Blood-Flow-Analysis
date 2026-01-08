# Quantum-Enhanced Blood Flow Analysis using CFD 🩸💻

**Author**: Soumya Nagendra  
**Institution**: School of Computer Science and Engineering, KLE Technological University

## 🎯 Abstract
This research compares the efficiency of **Quantum Machine Learning (QML)** circuits and classical **Machine Learning (ML)** models in predicting hemodynamic parameters derived from **Computational Fluid Dynamics (CFD)** simulations of a 3D human aorta model.

## 🏗️ System Architecture
The project follows a five-step methodology:
1. **Aorta 3D Modeling**: Created using anatomical data of healthy adults (Ages 25-30).
2. **CFD Simulations**: Conducted on **Ansys Workbench 2023** to understand blood flow behavior.
3. **Data Extraction**: Extracted flow parameters (velocity magnitude, pressure, wall-shear) from ~217,000 nodes.
4. **Model Training**: Comparison between Random Forest/Decision Tree and Pennylane-based QML circuits.
5. **Comparative Analysis**: Evaluation of MSE and R-squared errors.

## 🧪 Experimental Setup
### CFD Framework
- **Software**: Ansys Student 2023 R2.
- **Rheological Model**: **Carreau Model** used to simulate non-Newtonian blood behavior.
- **Algorithm**: **PIMPLE algorithm** (combining PISO and SIMPLE) for pressure-velocity coupling.

### Quantum Infrastructure
- **Simulators**: Amazon Braket 34-qubit **SV1** (State Vector Simulator).
- **Hardware**: **IonQ Aria 1** (25-qubit universal gate-model ion-trap QPU).
- **Circuit Design**: Single-qubit X and Y rotations followed by **CNOT entanglement** in a ring pattern.

## 📊 Key Results
| Algorithm | ML MSE | Quantum ML MSE |
| :--- | :--- | :--- |
| Random Forest Regressor | 0.0105 | 6.5084 |
| Decision Tree | 0.02317 | 6.5085 |

*Finding: While classical models currently outperform simple quantum circuits, the QML results show promise for complex data structures as quantum hardware evolves and I need to re-do it with a complex quantum circuit.*
