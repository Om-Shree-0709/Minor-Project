## **🧠 Dementia Anomaly Detection using Isolation Forest**  

### **📌 Overview**  
This project uses **Isolation Forest** to detect **behavioral anomalies** in dementia patients based on **sensor data** from a smart home environment. The model helps identify **irregular movement patterns, abnormal sensor activations, and potential dementia symptoms**.  

### **📊 Dataset Description (WE HAVE USED 2 Months Data For Current Work**  
The dataset consists of **sensor activity logs** with the following columns:  
- **Timestamp** → Date & Time of sensor activation  
- **Sensor** → Unique sensor ID  
- **Message** → Sensor status (`ON`, `OFF`, `OPEN`, `CLOSE`)  
- **SensorType** → Category of sensor (`Motion`, `Door`, `Appliance`, etc.)  

### **🛠️ Project Workflow**  
1️⃣ **Data Preprocessing**  
   - Convert categorical values (`SensorType`, `Message`) into numerical format.  
   - Extract **time-based features** (`Hour`, `Minute`, `Second`).  

2️⃣ **Anomaly Detection using Isolation Forest**  
   - Trained on features: `Hour`, `SensorType`, `Message`.  
   - **5% contamination rate** assumed for anomaly detection.  
   - Flags **irregular sensor activity** as **potential dementia-related behavior**.  

3️⃣ **Decision Boundary Visualization**  
   - **2D & 3D plots** to separate **normal vs. anomalous behavior**.  
   - Uses **meshgrid & contour plots** for decision boundary.  

4️⃣ **Behavioral Clustering**  
   - **K-Means applied** to group similar anomalies.  
   - Helps **categorize patterns** (e.g., frequent night movements, excessive door activity).  

### **📈 Results & Insights**  
- Anomalies detected during **late-night movements** indicate **wandering behavior**.  
- Unusual **door openings at odd hours** suggest **repetitive behavior or confusion**.  
- **Clustered anomalies** help categorize different types of abnormal behavior patterns.  

### **📌 Next Steps**  
- 🔹 **Fine-tune Isolation Forest parameters** for better accuracy.  
- 🔹 **Integrate real-time monitoring** using IoT devices.  
- 🔹 **Use deep learning models** (e.g., LSTMs) for improved anomaly prediction.  

