
# MEGAT Physics-Informed Neural Network (PINN) Experiment


## Abstract

Typical industrial plants with reaction units often operate under proprietary technology provided by licensors. These licensors offer technology packages containing specialized catalysts, processes, and kinetic models, encapsulated within a "black box." Unfortunately, the details of the catalysts' behavior and precise kinetic models are treated as trade secrets, leaving plant operators unable to independently perform critical activities such as:

- Process optimization
- Troubleshooting
- Adapting processes to different feedstocks  

Operators must instead rely on the licensor for support, which can be time-consuming and inefficient, particularly for fast optimizations.  

### The Opportunity with Machine Learning  

Operational data offers a unique opportunity to address this issue. By leveraging advancements in machine learning, particularly **Physics-Informed Neural Networks (PINNs)**, it is possible to infer the hidden aspects of reaction kinetics and catalyst behavior. PINNs integrate governing physical laws (e.g., mass and energy balance equations) directly into the neural network architecture. This hybrid approach combines:

1. The **robustness** of data-driven machine learning  
2. The **accuracy** of physics-based modeling  

This enables the network to learn underlying kinetics and catalyst behavior consistent with the physical constraints of the system.

### Experiment Objective  

The goal of this project is to use PINNs to "unlock" the black box, creating a model that captures the essential features of process kinetics and catalyst performance. By training the PINN on operational plant data, the resulting model can be used for:

- Independent process optimization  
- Simulations and predictions  
- Troubleshooting and flexibility enhancement  

---

## Features

- **Data-driven Learning:** Utilizes plant operational data for training.  
- **Physics Integration:** Incorporates mass and energy balance equations directly into the neural network loss function.  
- **Interpretability:** Provides insights into hidden reaction kinetics and catalyst behavior.  
- **Practical Applications:** Empowers plant operators to perform optimizations and troubleshooting independently.  

---

## Repository Contents

- `pinn-trial-1.ipynb`: The core experiment notebook demonstrating the implementation and results of the PINN approach.  
- `data/`: Folder for operational data used for training the PINN (placeholder for dataset details).  
- `src/`: Scripts for model architecture, training pipelines, and custom loss functions.  
- `results/`: Visualization of the PINN predictions, losses, and model performance.  

---

## Installation and Usage

1. Clone this repository:  
   ```bash
   git clone https://github.com/maercaestro/megat-pinn.git
   cd megat-pinn
   ```

2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:  
   Open `pinn-trial-1.ipynb` in your preferred Jupyter Notebook environment and execute the cells step-by-step.

---

## Results

- **Kinetic Modeling:** Successfully inferred hidden reaction kinetics based on operational data.  
- **Physical Consistency:** Ensured model predictions adhered to physical laws through PINN architecture.  
- **Applications:** Demonstrated potential for process optimization and troubleshooting in an industrial setting.

---

## Future Work

- Expanding the model to include multi-feedstock adaptability.  
- Enhancing computational efficiency for large-scale industrial applications.  
- Integrating real-time optimization capabilities.

---

## References
1. [Pinn Orginal Paper](https://arxiv.org/abs/1711.10561)
