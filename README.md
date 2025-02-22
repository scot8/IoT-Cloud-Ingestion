Below is a detailed `README.md` file for your IoT-Cloud-Ingestion project:

---

# **IoT-Cloud-Ingestion.**

This repository contains the setup and configuration details for ingesting real-time data from IoT devices monitoring cattle temperature in a smart farm. The solution uses **Azure IoT Hub** to handle data ingestion for four IoT devices representing the cows in the farm.

---

## **Azure IoT Hub Overview**

The Azure IoT Hub service was set up to enable seamless communication between IoT devices and the cloud.

---

## **Connection Strings for IoT Devices**

Each IoT device was registered in the Azure IoT Hub with a unique identifier corresponding to the cows being monitored. Below are the connection strings for each device:

- **Cow1 Connection String**: `HostName=hubCow.azure-devices.net;DeviceId=cow1;SharedAccessKey=3lz2L1sa32nGr+YP6QUSndszlpIjCLkxa3ExhtkRamw=`
- **Cow2 Connection String**: `HostName=hubCow.azure-devices.net;DeviceId=cow2;SharedAccessKey=jAaVDOEMqildKAgAIUmniz9N3wJ7yEFVHTDMEp8G0yg=`
- **Cow3 Connection String**: `HostName=hubCow.azure-devices.net;DeviceId=cow3;SharedAccessKey=IMTM8GCoKxvSRkmTuSnXRIwv2nQ13EVJAJE3+iw5fps=`
- **Cow4 Connection String**: `HostName=hubCow.azure-devices.net;DeviceId=cow4;SharedAccessKey=V369W5uDKYWXMdr9jU8gpFaCXo4A/dv8FczIIvl7BIo=`

---

## **Setup Process**

### **Step 1: Login to Azure**
1. Navigate to the [Azure Portal](https://portal.azure.com).
2. Log in using your Azure account credentials.

### **Step 2: Create Azure IoT Hub**
1. Search for **IoT Hub** in the Azure search bar and click **Create**.
2. Fill in the following details:
   - **Subscription**: Use your active subscription.
   - **Resource Group**: Create a new resource group (e.g., `xam`) or use an existing one.
   - **Region**: Choose the region closest to your location (e.g., `Canada Central`).
   - **IoT Hub Name**: Enter a unique name for the IoT Hub (e.g., `hubCow`).
3. Review the settings and click **Create**.

### **Step 3: Configure IoT Devices**
1. Once the IoT Hub is deployed, navigate to it from the Azure dashboard.
2. Select **IoT Devices** under the settings.
3. Click **+ New Device** and configure the devices as follows:
   - **Device IDs**: `Cow1`, `Cow2`, `Cow3`, `Cow4`.
   - **Authentication Type**: Symmetric Key.
4. Save each device, and Azure will generate connection strings for them.

### **Step 4: Retrieve Connection Strings**
1. Go to each device's details under **IoT Devices** in the IoT Hub.
2. Copy the **Primary Connection String** for each device and note them for later use.

### **Step 5: Capture Screenshots**
1. Capture a screenshot of the IoT Hub Overview page.
2. ![image](https://github.com/user-attachments/assets/b2a11792-cd72-49a9-8a28-1c8558467705)
   
4. Capture screenshots of the device registration details (optional).
5. ![image](https://github.com/user-attachments/assets/f1c6e06c-1839-49c6-9268-2abb2fecac17)
   


---

## **Repository Structure**

```plaintext
IoT-Cloud-Ingestion/
├── README.md              # Detailed setup instructions and project information
├── screenshots/           # Folder containing all screenshots
│   ├── iot-hub-overview.png
│   ├── device-cow1.png
│   ├── device-cow2.png
│   ├── device-cow3.png
│   └── device-cow4.png
```

---

## **Instructions for Access**

1. Clone this repository:
   ```bash
   git clone https://github.com/scot8/IoT-Cloud-Ingestion.git
   ```
2. Review the README and screenshots for setup details.
3. Access connection strings as needed for device configuration.

---

### **GitHub Repository Link**
[IoT-Cloud-Ingestion Repository](https://github.com/scot8/IoT-Cloud-Ingestion)
