
# LabVIEW Genral DAQ Program - 16 Channels

This is a general-purpose **LabVIEW 2021 data acquisition (DAQ)** program designed to read analog voltage data, display it on a real‑time graph, and record the acquired data to a file.

---

## How to Use the Program

### 1. Open the LabVIEW Project
Open the **DAQ Project** (`*.lvproj`).  
> **Important:** The program must be run from the LabVIEW Project to function correctly.

### 2. Open the Main VI
In the Project Explorer, double‑click **Main.vi**.

### 3. Run the Program
Click the **Run** arrow at the top of the LabVIEW window.

When prompted, enter a **file name** for saving your recorded data.  
- If left blank, a default name will be used:  
  **Experiment Result – [date and time]**

All saved result files are stored in the **Result Files** folder.

---

## 4. Configure Device and Settings
- Select your **Device Name**.  
- Enter the **Sample Rate**.  
- If you want to record for a fixed duration, enable **Use Record Time**.

Click **INITIALISE VOLTAGE CHANNELS**.  
A configuration window will appear.

### Channel Configuration
For each channel:
- Enter **Description**, **Scale**, and **Offset**.  
- Tick **Select Ch** to enable the channel.

Click **OK** when finished.

---

## 5. Start Data Acquisition
Click **Start** to begin acquiring data.

### Recording Data
You may record data at any time using the **Record** button.

Two options exist depending on program configuration:

- **Case A:** Records continuously until you press **Stop**  
- **Case B:** Automatically records for **10 seconds**

---

## 6. Stopping the Program
- Press **Stop** to stop data acquisition.  
  You can repeat Step 5 to begin another acquisition cycle.
- When you are completely finished, close the window.  
  **Always press Stop first** before closing to ensure your data file is saved correctly.

---

If you need help or wish to modify the program for your application, please contact the **Electronics & Software Labs**.

