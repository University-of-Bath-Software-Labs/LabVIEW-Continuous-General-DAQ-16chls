
# LabVIEW General DAQ Program - 16 Channels

This is a general-purpose **LabVIEW 2021 data acquisition (DAQ)** program designed to read analog voltage data, display it on a real-time graph, and record the acquired data to a file.

---

## How to Use the Program

### 1. Open the LabVIEW Project
Open the **DAQ Project** (`*.lvproj`).  
> **Important:** The program must be run from the LabVIEW Project to function correctly.

<img alt=" File explorer view image" src="https://github.com/user-attachments/assets/2f70746a-35a8-49a1-b52e-617b8843cdb4" />

### 2. Open the Main VI
In the Project Explorer, double-click **Main.vi**.

<img alt="Project explorer image" src="https://github.com/user-attachments/assets/6469a2ba-6399-4098-ac28-2698d362c6b2" />

### 3. Run the Program
Click the **Run** arrow at the top of the LabVIEW window.

<img alt="LabVIEW run arrow image" src="https://github.com/user-attachments/assets/df8db058-3318-43c9-87cf-9c2e3a11a1ed" />

When prompted, enter a **file name** for saving your recorded data.  
- If left blank, a default name will be used:  
  **Experiment Result – [date and time]**

All saved result files are stored in the **Result Files** folder.

<img alt="Results files image" src="https://github.com/user-attachments/assets/96e2accf-b3f8-4c54-859f-8ac59ec3d410" />

---

## 4. Configure Device and Settings
- Select your **Device Name**  
- Enter the **Sample Rate**  
- If you want recording to stop automatically after a fixed duration, enter a value in **Record Time (s)** and enable **Use Record Time**

<img alt="Device settings image" src="https://github.com/user-attachments/assets/699a277b-19d4-4c26-9c64-411aea971b7a" />

Click **INITIALISE VOLTAGE CHANNELS**.  
A configuration window will appear.

### Channel Configuration
For each channel:
- Enter **Description**
- Enter **Scale**
- Enter **Offset**
- Tick **Select Ch** to enable the channel

Click **UPDATE** when finished.

<img alt="Channel dialog image" src="https://github.com/user-attachments/assets/62395fac-ee49-40e8-bee6-a2c7060e35b0" />

---

## 5. Start Data Acquisition
Click **Start** to begin acquiring data.

### Recording Data
You may start or stop recording data at any time during a run using the **Record** checkbox.

#### Recording behaviour
- When **Record** is **unchecked**, the program continues acquiring and displaying data, but data is **not** written to file.
- When **Record** is **checked**, the program begins recording data to file.

Two recording modes are available depending on whether **Use Record Time** is enabled:

---

### A. Continuous Recording
If **Use Record Time** is **unchecked**, checking **Record** starts recording and recording continues until:
- **Record** is unchecked manually, or
- the program is stopped

<img alt="Record time unticked image" src="https://github.com/user-attachments/assets/a2205d90-976e-4360-af96-bf4a38e5dbb1" />

---

### B. Timed Recording
If **Use Record Time** is **checked**, checking **Record** starts recording immediately and the program records for the duration entered in **Record Time (s)**.

For example:
- if **Record Time (s)** is set to **10**
- and **Use Record Time** is enabled
- checking **Record** will record for **10 seconds from that moment**

At the end of the timed interval:
- recording stops automatically
- the **Record** checkbox is reset automatically

The timed recording feature can be used **multiple times during the same run**.  
For example, if **Record Time (s)** remains set to **10**, you can check **Record** later in the run to record for **another 10 seconds**.

<img alt="Record time ticked image" src="https://github.com/user-attachments/assets/2b46a6f0-306d-4b70-a6ac-5083877b69ba" />

---

## 6. Stopping the Program
- Press **Stop** to stop data acquisition
- You can repeat recording during a run as required
- When you are completely finished, close the window  
  **Always press Stop first** before closing to ensure your data file is saved correctly

<img alt="Stopping image" src="https://github.com/user-attachments/assets/8c89559b-d58d-4c3b-80e4-32495abaaf7e" />

---

## Notes
- The program must be run from the **LabVIEW Project** (`*.lvproj`)
- Result files are saved in the **Result Files** folder
- **Use Record Time** is optional
- When **Use Record Time** is enabled, the value in **Record Time (s)** is treated as the recording duration from the moment **Record** is checked
- Timed recording can be repeated multiple times during a single acquisition run

---

If you need help or wish to modify the program for your application, please contact the **Electronics & Software Labs**.
