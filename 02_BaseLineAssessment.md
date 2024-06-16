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
Its main advantage is the ability to estimate energy consumption in devices with an AMD processor. However, PowerTOP use cases go beyond simple energy consumption measurements. For example, it provides an interactive mode that allows users to fine-tune power management settings in their Linux system. 

**Features:**
- Monitors system-wide and per-application energy consumption
- Provides recommendations for reducing energy usage
- Useful for optimizing power settings and configurations

**Installation:**
- Install PowerTOP using your Linux package manager:
```sudo apt-get install powertop```  # For Debian/Ubuntu
```sudo yum install powertop```     # For CentOS/RHEL
```sudo powertop --csv=output.csv -t 20```

**Usage:**
Run PowerTOP with root privileges
sudo powertop

**Observe energy usage data for various processes**
____________________________________________________________________
 *  *  *   Overview of Software Power Consumers   *  *  *

Usage;Wakeups/s;GPU ops/s;Disk IO/s;GFX Wakeups/s;Category;Description;PW Estimate
172.9 us/s; 24.9;;;;Timer;tick_sched_timer; 98.5 mW
296.0 us/s; 22.9;;;;Process;[PID 313728] /usr/bin/containerd ; 90.8 mW
 96.5 us/s; 16.2;;;;Process;[PID 11] [rcu_sched]; 64.2 mW
225.5 us/s; 14.1;;;;Process;[PID 313736] /usr/bin/containerd ; 56.0 mW
409.9 us/s; 12.3;;;;Process;[PID 361909] /usr/bin/vmtoolsd ; 49.4 mW
232.0 us/s; 12.1;;;;Process;[PID 313737] /usr/bin/containerd ; 48.3 mW
 24.5 us/s;  4.9;;;;kWork;fb_flashcursor; 19.4 mW
 21.4 us/s;  4.8;;;;kWork;vmw_fence_work_func; 19.0 mW
156.0 us/s;  3.9;;;;kWork;psi_avgs_work; 15.8 mW
309.8 us/s;  3.4;;;;kWork;vmw_fb_dirty_flush; 13.9 mW
 29.4 us/s;  3.3;;;;kWork;gc_worker; 13.1 mW
311.6 us/s;  1.7;;;;Timer;hrtimer_wakeup; 7.19 mW
 23.8 us/s;  1.2;;;;Interrupt;[17] ioc0; 4.97 mW
 39.7 us/s;  1.0;;;;Process;[PID 811] /usr/sbin/ntpd -p /var/run/ntpd.pid -g -u 113:117 ; 4.20 mW
 15.5 us/s;  1.0;;;;Timer;watchdog_timer_fn; 3.97 mW
  4.4 us/s;  1.0;;;;kWork;vmballoon_work; 3.95 mW
  6.0 us/s;  0.9;;;;kWork;mpt_fault_reset_work; 3.76 mW
 15.8 us/s;  0.8;;;;kWork;vmstat_shepherd; 3.38 mW
  1.1 ms/s; 0.15;;;;Process;[PID 377852] powertop --csv=output.csv -t 20 ; 2.33 mW
[...]

In the file, under the table entitled Overview of Software Power Consumers, there is a line with the following:
```The system baseline power is estimated at:  5.43  W;```

**Calculate power consumption**
This means that, on average, our processor and main memory leveraged 5.43W of power during the 20 seconds of execution. As mentioned before, this is not the energy consumption (yet!). The total energy consumption in this measurement is computed by multiplying the average power by the duration of the measurement:

E=P.Δt=5.43W×20s=108.6J

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


