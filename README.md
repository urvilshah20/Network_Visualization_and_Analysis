# AI Adoption Network Analysis in Investment Banking

### **Project Background**

While artificial intelligence technologies offer transformative potential across industries, many organizations face significant challenges in translating AI initiatives from concept to reality. The implementation gap in AI adoption stems from several key factors:

- Operational Disruption: Integration of AI systems often requires substantial changes to existing workflows
- Talent Gap: Limited availability of specialists with AI expertise
- Compliance Challenges: Complex regulatory requirements and ethical considerations
- Professional Resistance: Particularly in knowledge-intensive sectors, where experts may view AI as a potential threat

In the investment banking sector, understanding how traders perceive and interact with AI technologies is crucial for successful implementation. This project specifically examines these dynamics within trading floor networks.

### **Project Overview**

This project analyzes network dynamics and node behavior patterns within an investment banking trading floor network, focusing on AI tool adoption and trader interactions. The analysis aims to understand and promote the adoption of AI tools for securities evaluation among traders.

### **Objective**

The primary goal is to assist a large investment bank in promoting AI tool adoption by:

- Understanding and addressing traders' concerns about AI
- Analyzing network structures and interaction patterns
- Identifying influential nodes and community structures
- Developing strategies for AI integration

### **Dataset**

The analysis is based on a comprehensive survey conducted at a major trading floor in Canary Wharf. The dataset (`trading_floor.xml`) encompasses responses from 192 traders and includes:

**Data Components:**

**1) Knowledge Exchange Network**

- the undirected network of knowledge exchange between traders (traders A and B are connected when A says he/she shares technical and industry knowledge with B and vice versa)
- Edge creation based on mutual technical and industry knowledge sharing
- Represents organic information flow within the trading floor


**2) AI Impact Assessment**

- Individual trader's opinion about AI's contribution to their work and effectiveness in evaluating securities
- Scale: 1 (minimal impact) to 10 (significant impact)
- Stored as node attribute 'ai'


**3) Spatial Information**

- Trading floor divided into six zones
- Each zone contains 32 traders (16 per side)
- Trader positions mapped using x-pos and y-pos coordinates
- Enables spatial analysis of AI adoption patterns

### **Features**

- Network structure analysis
- Community detection using Louvain algorithm
- Centrality measures calculation
- Opinion distribution visualization
- Comparative network analysis
- Spatial pattern analysis

### **Technologies Used**

- Python 3.8+
- NetworkX for graph analysis
- Pandas for data manipulation
- Matplotlib/Seaborn for visualization
- Community detection algorithms
- Statistical analysis libraries


### **Getting Started**

**Project Structure:**
The repository contains the following key files:

- `NetworkAnalysisCode.ipynb`: Main Jupyter notebook containing all analysis code
- `trading_floor.xml`: Dataset file containing trader network information
- `AI_Adoption_NetworkAnalysis.pdf`: Detailed analysis and findings report

**Prerequisites:**
Required Python libraries:
```
networkx
pandas
matplotlib
seaborn
jupyter
```

**Installation & Setup:**

1) Clone the repository or download the files
2) Install required dependencies:

```
pip install networkx pandas matplotlib seaborn jupyter
```

**Usage:**

1) Place both `NetworkAnalysisCode.ipynb` and `trading_floor.xml` in the same directory
2) Open the directory in VSCode or your preferred IDE
3) Run the Jupyter notebook to perform the analysis
4) Refer to `AI_Adoption_NetworkAnalysis.pdf` for detailed analysis and findings

**Note:**

Ensure the dataset file (`trading_floor.xml`) is in the same folder as the notebook for the code to run properly.

### **Contributing**

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss the proposed changes.
