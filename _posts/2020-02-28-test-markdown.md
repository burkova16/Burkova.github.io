---
layout: post
title: Sample blog post
subtitle: Each post also has a subtitle
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

**Sowftware design, Algorithm and Data Structures, Database**


In here we will view 3 main artifacts and enhancements for this project.


## 1. Sowftware design

By utilizing a variety of elements, coding structure, and analysis, this CS 350 project showcases my software engineering and design skills. Currently, the program can set the temperature and activating/deactivating the heating system. However, the goal is to expand the project's capabilities by integrating it with Wi-Fi and incorporating an IoT device to collect and transfer data via a hub or IoT gateway for further analysis and action through either a user interface or backend system. 


  The addition of Wi-Fi functionality to the thermostat allows for remote control and monitoring of the temperature settings, even when the user is not physically present. This feature adds convenience and flexibility to the user's experience, as they can adjust the temperature settings from their mobile device or computer, without having to be near the thermostat. Additionally, the ability to connect to Wi-Fi opens opportunities for the device to interact with other smart home systems, such as voice assistants, and provides the potential for more sophisticated automation and energy-saving features. This enhancement serves to highlight my proficiency in software design and demonstrate to potential employers my experience working with IoT technology. To enhance this project, my plan is to add more functions, including connecting the device to Wi-Fi. The IoT device will collect data, which will be transferred to the hub or IoT gateway for collation and analysis. Further actions will be taken through the user interface or back-end systems. This enhancement will demonstrate my software design skills and showcase my experience working with IoT to future employers.


  Wi-Fi functionality should be added to the thermostat in a modular way, allowing for easy modification or removal of the feature in the future if necessary. This can be achieved by separating the Wi-Fi code into its own module or class that can be easily included or excluded from the main codebase. The addition of Wi-Fi functionality requires changes to the overall code structure to accommodate the new feature. This may involve refactoring the existing code to improve code readability and maintainability, such as creating separate functions or classes for different tasks.
  
    
  Adding Wi-Fi to a thermostat can improve the user experience by enabling remote control and monitoring of the device through a mobile app or web portal. This can provide users with greater flexibility and convenience in controlling their home's temperature and energy usage. The addition of Wi-Fi functionality may require changes to the hardware and software architecture of the thermostat, as well as new testing and validation procedures. Outcome-coverage in this area would focus on ensuring that the Wi-Fi feature is reliable, secure, and performs as expected. the outcome-coverage for adding Wi-Fi to a thermostat can be quite broad and multifaceted, encompassing factors such as user experience, energy efficiency, technical performance, market competitiveness, and regulatory compliance.
  
  
  I faced some challenges during this process. Adding Wi-Fi functionality to a thermostat requires the use of external hardware components, such as a Wi-Fi module or chip, and appropriate software libraries that support wireless communication. C++ code can be used to interface with these hardware components and implement the necessary protocols for sending and receiving data over Wi-Fi.



~~~
Start

Check if thermostat is connected to power and WiFi

If not connected, connect to power and WiFi

Initialize thermostat settings and connect to cloud service

Read temperature and humidity from thermostat sensor

Upload sensor data to cloud service

Wait for predetermined time interval

Check if thermostat settings have been changed remotely

If settings have been changed, update thermostat settings and save to memory

Repeat from Read temperature and humidity step

End
~~~

And here is the enchanced code:

```c++
// Initialize variables
    total_energy_saved = 0
    current_energy_consumption = get_current_energy_consumption()
    target_energy_consumption = get_target_energy_consumption()
    // Loop until target energy consumption is reached
    while current_energy_consumption > target_energy_consumption:
        // Check if any devices can be turned off
        device_to_turn_off = find_device_to_turn_off()
        if device_to_turn_off is not None:
            turn_off_device(device_to_turn_off)
            energy_saved = get_energy_saved(device_to_turn_off)
            total_energy_saved += energy_saved
            current_energy_consumption -= energy_saved
        else:
            // No devices can be turned off, so reduce their power consumption
            reduce_device_power_consumption()
            current_energy_consumption = get_current_energy_consumption()
    
    // Print energy saved and return
    print("Total energy saved: ", total_energy_saved)
    return

```

Breaking down the code:


1.	Initialize variables:
•	This block initializes the variables total_energy_saved, current_energy_consumption, and target_energy_consumption to their initial values.


2.	Loop until target energy consumption is reached:
•	This block starts a loop that will continue until the current energy consumption is less than or equal to the target energy consumption. This means that the loop will keep running until the desired energy savings have been achieved.


3.	Check if any devices can be turned off:
•	This block checks to see if there are any devices that can be turned off to save energy. If there are devices that can be turned off, the code will execute the turn_off_device function, which will turn off the device and update the variables total_energy_saved and current_energy_consumption accordingly.


4.	No devices can be turned off:
•	If there are no devices that can be turned off, the code will execute the reduce_device_power_consumption function, which will reduce the power consumption of the devices in some other way. For example, it could reduce the brightness of lights or the power of a fan. After reducing the power consumption, the code updates the current_energy_consumption variable.


5.	Print energy saved and return:
•	This block prints the total amount of energy saved and then returns from the function. The total energy saved is stored in the total_energy_saved variable.



##  2. Algorithm and Data Structures
##  3. Database



## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
