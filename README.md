# 🚀 Compressor_Control_Offline_RL

This repository contains an implementation of **Offline Reinforcement Learning (Offline RL)** to control a compressor system based on historical operational data.

The project is built using Python and Keras, and includes Jupyter notebooks for training the model and simulating the control behavior, along with the necessary data and pre-trained artifacts.

---

## 📁 Repository Structure

```
📦 Compressor_Control_Offline_RL
├── main.ipynb                # Notebook to simulate compressor control using the trained model
├── Offline_Model.ipynb       # Notebook to train the RL model from historical data
├── Compressor_Machine.keras  # Pre-trained RL model saved in Keras format
├── scaler.sav                # Scaler object used for feature normalization
├── Compressor-_1_.xlsx       # Historical dataset used for training and simulation
```

---

## 📌 Key Features

- ✅ Offline RL approach to learn from historical data without real-time interaction
- 📊 Data-driven control for compressor machine operations
- 🧠 Includes feature scaling, training pipeline, and simulation logic
- 💾 Pre-trained model and scaler ready to use
- 🔬 Based on reproducible Jupyter notebooks

---

## 🛠 How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/alexandertiopan1212/Compressor_Control_Offline_RL.git
   cd Compressor_Control_Offline_RL
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   > If `requirements.txt` is not available, make sure to install manually:
   ```bash
   pip install numpy pandas scikit-learn tensorflow openpyxl
   ```

3. Open `Offline_Model.ipynb` to explore how the model was trained using historical compressor data.

4. Open `main.ipynb` to simulate how the trained model controls the compressor under different conditions.

---

## 📈 Dataset

The dataset `Compressor-_1_.xlsx` contains historical records of compressor operations, including:

- Operational states
- Input/output pressures
- Flow rates
- Environmental variables

These are used to build the state-action space for the RL model.

---

## 🤖 Model

The model is saved in `Compressor_Machine.keras` and was trained using a Deep Q-Learning (DQN) approach adapted for offline use.

The model takes the current state of the compressor as input and predicts the best control action.

Normalization of inputs was done using `MinMaxScaler` saved in `scaler.sav`.

---

## 📌 Notes

- This implementation is focused on *offline* training, so the model learns entirely from logged historical data.
- Future improvements can include online fine-tuning or integration with a digital twin for continuous learning.

---

## 📬 Contact

For questions or collaboration, feel free to reach out to:

**Alexander Tiopan**  
[GitHub](https://github.com/alexandertiopan1212) | [LinkedIn](https://www.linkedin.com/in/alexander-tiopan/)  
📧 alexandertiopan1212@gmail.com

---

## 📝 License

This project is licensed under the MIT License — feel free to use and modify with attribution.
