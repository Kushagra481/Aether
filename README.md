# AETHER  
## AI-Powered Cascading Disaster Prediction and Response System

AETHER is a hybrid disaster intelligence system built to predict how failures spread across regions during complex disaster events. Instead of treating floods, fires, earthquakes, or infrastructure failures as isolated incidents, AETHER models them as connected processes that can trigger one another over time. The system combines interpretable simulation with graph-based learning so it can both explain local propagation and learn larger cascade patterns from data.

## Overview

The main goal of AETHER is to answer three practical questions:

- What area is likely to fail next?
- How will the current disaster spread over time?
- Which regions need attention before the damage escalates?

To do this, AETHER uses a two-layer design. The first layer is an Infrastructure Interaction Model that simulates how disruption spreads between connected zones. The second layer is a Temporal Graph Neural Network that learns recurring cascade behavior from spatiotemporal patterns. Together, these components allow the system to move beyond simple detection and toward early forecasting.

## Key Contributions

- Built a hybrid framework that combines simulation-based reasoning with temporal graph learning
- Designed for multi-hazard settings where one disaster can trigger secondary failures
- Models cascading effects across connected geographic zones
- Supports large-scale graph processing and fast inference
- Includes a fault-tolerant communication layer concept for real-time disaster response settings

## System Pipeline

1. Collect disaster event and regional context data  
2. Construct a graph where nodes represent zones and edges represent interactions  
3. Run the Infrastructure Interaction Model to simulate disruption spread  
4. Convert propagation outputs into node-level temporal features  
5. Feed these features into the Temporal Graph Neural Network  
6. Predict future high-risk regions and cascade progression  

## Architecture Figures

### Figure 1. Overall System Architecture
<!-- Insert Figure 1 here -->
![Figure 1 Placeholder](<img width="1600" height="745" alt="image" src="https://github.com/user-attachments/assets/bd87776a-b536-4766-b8d7-f9b83d64ddfa" />
)

### Figure 2. Model Architecture
<!-- Insert Figure 2 here -->
![Figure 2 Placeholder](<img width="1600" height="445" alt="image" src="https://github.com/user-attachments/assets/8994f6d1-6363-43f6-8710-01e8de4feb87" />
)

### Figure 3. Knowledge Graph Architecture
<!-- Insert Figure 3 here -->
![Figure 3 Placeholder](<img width="930" height="1484" alt="image" src="https://github.com/user-attachments/assets/4ff3fd6a-7536-43c0-b15b-70d0484dbc91" />
)

### Figure 4. Input Output Inoperability Model Architecture
<!-- Insert Figure 4 here -->
![Figure 4 Placeholder](Z<img width="417" height="318" alt="image" src="https://github.com/user-attachments/assets/1750630d-c080-4391-a62a-156c67366392" />
)

### Figure 5. Cascade Heatmap
<!-- Insert Figure 5 here -->
![Figure 5 Placeholder](![Uploading image.png…]()
)

## Core Components

### 1. Knowledge Graph Layer
The knowledge graph captures structured relationships between disaster events, locations, environmental factors, and temporal dependencies. It helps represent how different events are semantically, spatially, and temporally connected. This layer is useful for turning raw disaster records into a graph structure that can support both simulation and learning.

### 2. Infrastructure Interaction Model
The Infrastructure Interaction Model is the interpretable part of AETHER. It simulates how disruption in one zone affects neighboring zones over time. Instead of directly relying on a black-box predictor, this component gives a step-by-step estimate of inoperability spread, making the system easier to inspect and reason about.

### 3. Temporal Graph Neural Network
The Temporal Graph Neural Network learns cascade patterns from evolving graph states. It takes node features, graph connectivity, and time-dependent propagation signals to predict which areas are most likely to be affected next. This layer helps the system move beyond fixed rules and capture more complex multi-step patterns.

### 4. Response and Communication Layer
AETHER is designed with deployment-oriented thinking in mind. The broader system concept includes a mesh-style communication layer for resilient disaster monitoring and response. This supports the idea of decentralized coordination even when parts of the system fail.

## Technical Highlights

- Hybrid modeling using simulation and graph learning
- Temporal reasoning over dynamic disaster graphs
- Supports cascading and compound event analysis
- Designed for scalable node-level inference
- Suitable for research in disaster forecasting, resilience, and AI for real-world safety systems

## Tech Stack

- Python
- PyTorch
- PyTorch Geometric
- NumPy
- Pandas
- Matplotlib
- C++
- Rerun

## Use Cases

- Early warning for cascading disaster scenarios
- Regional risk forecasting
- Infrastructure stress analysis
- Multi-hazard planning and resilience research
- AI-assisted disaster response systems

## Project Motivation

Most disaster prediction systems focus on detecting individual events. AETHER focuses on what happens after the first event. That shift matters because many real-world failures are not isolated. They spread, interact, and create secondary risks. This project was built to study those failure chains in a more structured and practical way.

## Future Improvements

- Integrate live sensor streams for real-time forecasting
- Add uncertainty estimation for safer decision support
- Improve multimodal fusion using satellite and weather data
- Expand the communication layer into a full deployment-ready prototype
- Build a visual dashboard for live risk tracking
