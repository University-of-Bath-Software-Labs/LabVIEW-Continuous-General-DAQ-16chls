
# LabVIEW Genral DAQ Program - 16 Channels

This is a general-purpose **LabVIEW 2021 data acquisition (DAQ)** program designed to read analog voltage data, display it on a real‑time graph, and record the acquired data to a file.

---

## How to Use the Program

### 1. Open the LabVIEW Project
Open the **DAQ Project** (`*.lvproj`).  
> **Important:** The program must be run from the LabVIEW Project to function correctly.

<img width="970" height="463" alt="image" src="https://github.com/user-attachments/assets/d0725066-2f61-4aae-ac26-6cd635a44e2b" />

### 2. Open the Main VI
In the Project Explorer, double‑click **Main.vi**.

<img width="594" height="433" alt="image" src="https://github.com/user-attachments/assets/02863c3b-b27c-4bda-aae9-9651e76974bf" />

### 3. Run the Program
Click the **Run** arrow at the top of the LabVIEW window.

<img width="947" height="382" alt="image" src="https://github.com/user-attachments/assets/60179c00-5ec0-4bff-b0b5-ca82848f2f30" />

When prompted, enter a **file name** for saving your recorded data.  
- If left blank, a default name will be used:  
  **Experiment Result – [date and time]**

All saved result files are stored in the **Result Files** folder.

<img width="766" height="203" alt="image" src="https://github.com/user-attachments/assets/738ac0c7-175d-43d5-ba8a-83259f0e1944" />

---

## 4. Configure Device and Settings
- Select your **Device Name**.  
- Enter the **Sample Rate**.  
- If you want to record for a fixed duration, enable **Use Record Time**.

  <img width="266" height="283" alt="image" src="https://github.com/user-attachments/assets/72fd9036-07bb-4d75-830b-e329bd8bf0ca" />

Click **INITIALISE VOLTAGE CHANNELS**.  
A configuration window will appear.

### Channel Configuration
For each channel:
- Enter **Description**, **Scale**, and **Offset**.  
- Tick **Select Ch** to enable the channel.

Click **UPDATE** when finished.

<img width="802" height="531" alt="image" src="https://github.com/user-attachments/assets/98ebcc8c-8f5c-4e3f-900d-7e0775a3363d" />

---

## 5. Start Data Acquisition
Click **Start** to begin acquiring data.

### Recording Data
You may record data at any time using the **Record** button.

Two options exist depending on program configuration:

- **Case A:** Records continuously until you press **Stop**

<img width="191" height="261" alt="image" src="https://github.com/user-attachments/assets/2e84c9b0-fd26-498b-aa08-2f136dca1882" />

- **Case B:** Automatically records for **10 seconds**

<img width="184" height="261" alt="image" src="https://github.com/user-attachments/assets/729d1aac-0ae6-4390-bae7-b0b4644d0579" />

---

## 6. Stopping the Program
- Press **Stop** to stop data acquisition.  
  You can repeat Step 5 to begin another acquisition cycle.
- When you are completely finished, close the window.  
  **Always press Stop first** before closing to ensure your data file is saved correctly.

<img width="1090" height="577" alt="image" src="https://github.com/user-attachments/assets/6cfd566c-e76b-4de3-90fe-3c6aaab7cdca" />

---

If you need help or wish to modify the program for your application, please contact the **Electronics & Software Labs**.

