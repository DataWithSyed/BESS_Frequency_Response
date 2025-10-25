# ⚡ Battery Energy Storage System (BESS) Frequency Response Modeling

This repository demonstrates the **modeling and simulation of a Battery Energy Storage System (BESS)** for **frequency response applications**.
The notebook analyzes how BESS can be used to stabilize grid frequency by responding dynamically to load variations or renewable generation fluctuations.

This project combines **data-driven analysis**, **control logic**, and **energy systems modeling**, providing a foundational approach for researchers and engineers working in grid stability and renewable integration.

---

## 📘 Project Overview

Modern power systems face increasing challenges in maintaining frequency stability due to the integration of variable renewable energy sources such as wind and solar.
Battery Energy Storage Systems (BESS) offer a fast and flexible means of providing **Frequency Containment Reserve (FCR)** and **Frequency Restoration Reserve (FRR)** services.

This notebook simulates a simplified BESS control strategy that:

* Monitors frequency deviations in real-time,
* Adjusts charge/discharge behavior accordingly,
* Evaluates the impact on grid stability and system performance.

---

## ⚙️ Objectives

* Model a **BESS frequency response control system**.
* Simulate the **real-time charge/discharge behavior** under frequency deviation scenarios.
* Analyze **energy capacity utilization** and **response efficiency**.
* Demonstrate how BESS can support **frequency regulation** in modern power grids.

---

## 🧠 Methodology

1. **Input Data**

   * Frequency deviation signal (time-series data)
   * System parameters such as power rating, energy capacity, and efficiency.

2. **Control Logic**

   * The BESS reacts to frequency deviations:

     * **Discharges** when frequency < nominal (to support the grid).
     * **Charges** when frequency > nominal (to absorb excess power).
   * Incorporates constraints like charge limits and state-of-charge (SoC) boundaries.

3. **Simulation**

   * Uses a Python-based iterative time-step approach.
   * Tracks state-of-charge (SoC), power flow, and cumulative energy throughput.

4. **Performance Evaluation**

   * Visualizes power response, SoC trends, and cumulative frequency regulation contribution.

---

## 🧮 Key Components

| Component                 | Description                                                                               |
| ------------------------- | ----------------------------------------------------------------------------------------- |
| **Frequency Signal**      | Time-series input data representing frequency deviation from nominal (e.g., 50 or 60 Hz). |
| **BESS Control**          | Algorithm to determine charge/discharge power based on deviation magnitude.               |
| **State-of-Charge (SoC)** | Updated iteratively with efficiency factors and power flow limits.                        |
| **Response Efficiency**   | Evaluated based on energy throughput and time to stabilize deviations.                    |

---

## 📊 Example Outputs

* **Frequency vs. Power Response Graph**
* **State-of-Charge Over Time**
* **Cumulative Energy Dispatched**
* **Performance Metrics (Efficiency, Utilization, Responsiveness)**

> 📈 These visualizations help understand how BESS dynamically compensates for frequency fluctuations and stabilizes grid operation.

---

## 🧰 Technologies Used

* **Python 3.10+**
* **Pandas** – Data handling
* **Matplotlib** – Visualization
* **NumPy** – Numerical computation
* **Jupyter Notebook** – Interactive development environment

---

## 🚀 How to Run

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/BESS-Frequency-Response.git
   cd BESS-Frequency-Response
   ```

2. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Notebook**

   ```bash
   jupyter notebook "BESS_Freq_Response.ipynb"
   ```

---

## 🔒 Data Notice

> ⚠️ **Note:**
> The original dataset used for this project is **not publicly available** due to confidentiality restrictions.
> The repository includes **only the code and modeling framework**, which can be applied to your own dataset.

---

## 💡 Future Enhancements

* Integration with **real-world frequency datasets** from power system operators.
* Implementation of **adaptive control logic** using reinforcement learning.
* Addition of **battery degradation modeling** to evaluate lifecycle performance.
* Real-time simulation using **SimPy** or **OpenModelica** integration.

---
