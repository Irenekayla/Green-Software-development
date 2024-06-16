Step 2 in green software development is understanding the current environmental impact of your software.

# **Overview**

Conducting a baseline assessment is crucial to understanding the current environmental impact of your software. This step involves measuring the energy consumption, carbon footprint, and resource usage of your existing software systems. 

# **2.1 Measuring Current Energy Consumption**
You can't improve something you cannot measure. The energy efficiency of a software program can be computed by measuring the amount of energy that the program consumes while it is running. This can be done using a variety of tools and techniques, such as power meters and energy profilers.

## **2.1.1 Understanding Energy Profiling**

Energy profiling tools help you measure the energy consumption of your software and identify areas for improvement. Below are some recommended tools for conducting a baseline assessment.

## **2.1.2. Tools for Energy Profiling**

Some popular tools used to measure energy consumption are:
Joulemeter
PowerTOP

### **Joulemeter**

**Description:**
Joulemeter is a tool developed by Microsoft that estimates the energy consumption of your computer and the software running on it.

**Features:**
- Monitors power usage of individual applications.
- Estimates energy consumption based on hardware utilization.
- Provides real-time data and historical usage reports.

**Installation:**
- Download Joulemeter from the [Microsoft Research website](https://www.microsoft.com/en-us/research/project/joulemeter/).

**Usage:**
1. Install and launch Joulemeter.
2. Select the application or process you want to monitor.
3. View real-time energy consumption data and export reports for analysis.

**Example:**

Process Name    | CPU Power (W) | Disk Power (W) | Display Power (W) | Total Power (W)
---------------------------------------------------------------------------------------
example.exe     |       15.2    |        3.1     |         4.8       |       23.1


### **PowerTOP**

**Description:**
PowerTOP is a Linux-based tool that helps diagnose issues with power consumption and provides suggestions for improving power efficiency.

**Features:**
- Monitors system-wide and per-application energy consumption
- Provides recommendations for reducing energy usage
- Useful for optimizing power settings and configurations

**Installation:**
- Install PowerTOP using your Linux package manager:
sudo apt-get install powertop  # For Debian/Ubuntu
sudo yum install powertop     # For CentOS/RHEL

**Usage:**
Run PowerTOP with root privileges
sudo powertop

Observe energy usage data for various processes
Follow recommendations to reduce power consumption

## **2.2 Measure Carbon Footprint**

### **2.2.1 Understanding Carbon Footprint**
Carbon footprint measures the total greenhouse gas emissions caused directly and indirectly by an activity. For software, this includes energy consumption, data transfer, and cloud services usage.

### **2.2.2 Tools for measuring carbon footprint**

Some popular tools used to measure energy consumption are:
AWS Carbon Footprint Tool
Google Cloud Carbon Calculator

## **2.3 Evaluate Resource Usage**

### **2.2.1 Understanding Resource Usage**
Resource usage includes the consumption of CPU, memory, and storage. Efficient use of these resources can significantly reduce energy consumption and environmental impact.

### **2.2.2 Tools for measuring resource usage**

Some popular tools used to measure energy consumption are:
Htop
VisualVM

# **2.4 Document the Findings**
## **Baseline Assessment Report**

### **Overview**
This report documents the baseline environmental impact of the current software system.

### **Energy Consumption**
- **Total Energy Use:** 300 kWh
- **High Impact Components:** Data processing, API calls

### **Carbon Footprint**
- **Total Emissions:** 150 kg CO2
- **Major Contributors:** Cloud services, data storage

### **Resource Usage**
- **CPU Usage:** 40% average
- **Memory Usage:** 70% average

### **Recommendations**
- **Optimize Data Processing:** Refactor code to improve efficiency.
- **Reduce Cloud Footprint:** Migrate to more energy-efficient cloud services.


