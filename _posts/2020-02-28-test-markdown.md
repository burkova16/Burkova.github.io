---
layout: post
title: Explanation of the code
subtitle: Here I will discuss end explain the code
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, explanation, follow]
tags: [code, C++]
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


##  2. Algorithm and Data Structures


  The current thermostat project makes use of algorithms and data structures. The program currently uses a temperature control algorithm, as a thermostat needs to maintain the temperature of a room within a specified range. An algorithm can be used to control the heating and cooling systems to achieve this goal. The algorithm might use a simple proportional-integral-derivative (PID) controller or a more sophisticated model-predictive control (MPC) algorithm, depending on the specific requirements of the application. 
  
  
  The plan for enhancing the project is to include energy-saving algorithms that can reduce energy usage by adjusting the temperature based on room occupancy. For example, an algorithm may adjust the temperature to a more energy-efficient level when the room is unoccupied. I will need to ensure that the algorithms are safe for the user to use in energy-saving mode. I can enhance the energy-saving mode simply by adding another button to the code and enabling the function. This enhancement will showcase my knowledge of implementing algorithms in the application.
  
  
  Enhancing the project to include energy-saving algorithms that can reduce energy usage by adjusting the temperature based on room occupancy is a good choice for this project. By adjusting the temperature based on room occupancy, energy-saving algorithms can significantly reduce energy consumption. When rooms are unoccupied, the thermostat can adjust the temperature to a more energy-efficient level, which can help save on energy costs. For example, an algorithm might adjust the temperature to a more energy-efficient level when the room is unoccupied. This enhancement will demonstrate my knowledge of algorithm implementation in the application. The components of this artifact will showcase my skills in initialization, looping, device management, and energy consumption.
  
  
  I have met the course objectives that were my goal. The updates for the outcome-coverage plans are testing and optimization, integration with smart home systems, and use of advanced algorithms. After implementing the energy-saving algorithms, it will be important to test and optimize their performance. This can be done by measuring energy consumption before and after implementing the algorithms and making adjustments as needed to ensure optimal energy savings. The project could be further enhanced by integrating it with smart home systems such as Google Home or Amazon Alexa. This would allow users to control the thermostat remotely and receive alerts when rooms are unoccupied or when energy consumption exceeds a certain threshold. While the current algorithms are effective, more advanced algorithms such as machine learning-based algorithms could be used to further improve energy savings. These algorithms could learn from user behavior patterns and adjust temperature settings accordingly.
  
  
  I have learned that pseudocode is very helpful for this project. Pseudocode can be written in plain English or any other natural language, making it easy to read and understand for people without technical programming knowledge. This can help ensure that the program's logic and functionality are clear to all stakeholders involved in the development process. One of the challenges I faced was testing. Since I only have one thermostat and no special rooms to switch temperatures, it was not convenient to keep testing in the same room.

~~~
pseudocode for the energy-saving algorithm
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
~~~


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


##  3. Database


The thermostat has memory, but it does not include a database. The plan is to enhance the project by adding a MySQL database. The original design does not include many libraries, so additional libraries will be required to save data to the database. The temperature and humidity readings from the thermostat can be stored in a structured way in a MySQL database, with columns for the timestamp, temperature, and humidity readings. This data can be used for various purposes, such as generating charts and reports, detecting anomalies, and analyzing trends over time. This enhancement will improve data management, increase functionality, and improve the user experience.


Adding SQL database to this project will showcase my skills in data management, integration, scalability, and reliability. By adding a MySQL database, I am showcasing the ability to manage data in a structured and efficient way. I will be showing that I can create tables, insert data, and retrieve data from a database using SQL statements. Integrating a MySQL database into a project requires knowledge of various technologies, such as database management systems, APIs, and programming languages. This demonstrates the ability to work with different technologies and integrate them seamlessly into a project. A database will allow to store large amounts of data and scale the application as it grows. I will be showing an ability to design and develop applications that can handle large amounts of data and scale as needed. One of the ways to improve the enhancement is adding security level to it. This involves implementing user authentication, access control, and encryption. This helps to protect the data from unauthorized access and ensure data privacy and confidentiality.


I have achieved the course objectives that were my goal. The updates to the outcome-coverage plans include data storage management, analytics and reporting, and integration with other systems. Since the thermostat generates a large amount of data, such as temperature and humidity readings, it is necessary to store and manage that data in a database. A database can provide a structured and organized way to store and retrieve data, making it easier to manage and analyze. With the addition of a database, complex queries and analytics can now be performed on the data, allowing for insights to be gained from it.


One of the main things I have learned is the use of libraries for MySQL. The MySQL C++ library provides a high-level interface for connecting to the database, executing queries, and retrieving data. One difficulty that I have encountered is that storing sensitive data, such as temperature and humidity readings, in a database can raise security concerns. It is important to implement appropriate security measures, such as user authentication and access control, to ensure that the data is protected. I have learned that pseudocode is very helpful for this project. Pseudocode can be written in plain English or any other natural language, making it easy to read and understand for people without technical programming knowledge. This can help ensure that the program's logic and functionality are clear to all stakeholders involved in the development process. One of the challenges I faced was testing. Since I only have one thermostat and no special rooms to switch temperatures, it was not convenient to keep testing in the same room.

~~~
Pseudocode:
The first step is to include the necessary libraries for the project, including MySQL Connector/C++, which will allow the program to interact with the database.
Next, the program will establish a connection to the MySQL database using a username and password.
After establishing a connection, the program will create a table in the database to store temperature and humidity readings, along with a timestamp for each reading.
Then, the program will retrieve temperature and humidity readings from the thermostat and insert them into the MySQL database table.
Finally, the program will close the database connection.
Overall, this pseudocode outlines the basic steps needed to add a MySQL database to the thermostat project for better data management and analysis.
~~~



Here is an example of enchanced code in the .c file

```
void *mainThread(void *arg0)
{

    // Initialize variables
    double total_energy_saved = 0;
    double current_energy_consumption = get_current_energy_consumption();
    double target_energy_consumption = get_target_energy_consumption();

    // Loop until target energy consumption is reached
    while (current_energy_consumption > target_energy_consumption) {
        // Check if any devices can be turned off
        string device_to_turn_off = find_device_to_turn_off();
        if (device_to_turn_off != "") {
            turn_off_device(device_to_turn_off);
            double energy_saved = get_energy_saved(device_to_turn_off);
            total_energy_saved += energy_saved;
            current_energy_consumption -= energy_saved;
        }
        else {
            // No devices can be turned off, so reduce their power consumption
            reduce_device_power_consumption();
            current_energy_consumption = get_current_energy_consumption();
        }
    }

    // Print energy saved and return
    cout << "Total energy saved: " << total_energy_saved << endl;
    return 0;
    /* Call driver init functions */
    GPIO_init();

    /* Configure the LED and button pins */
    GPIO_setConfig(CONFIG_GPIO_LED_0, GPIO_CFG_OUT_STD | GPIO_CFG_OUT_LOW);
    GPIO_setConfig(CONFIG_GPIO_LED_1, GPIO_CFG_OUT_STD | GPIO_CFG_OUT_LOW);
    GPIO_setConfig(CONFIG_GPIO_BUTTON_0, GPIO_CFG_IN_PU | GPIO_CFG_IN_INT_FALLING);

    /* Turn on user LED */
    GPIO_write(CONFIG_GPIO_LED_0, CONFIG_GPIO_LED_ON);

    /* Install Button callback */
    GPIO_setCallback(CONFIG_GPIO_BUTTON_0, gpioButtonFxn0);

    /* Enable interrupts */
    GPIO_enableInt(CONFIG_GPIO_BUTTON_0);

    /*
     *  If more than one input pin is available for your device, interrupts
     *  will be enabled on CONFIG_GPIO_BUTTON1.
     */
    if (CONFIG_GPIO_BUTTON_0 != CONFIG_GPIO_BUTTON_1) {
        /* Configure BUTTON1 pin */
        GPIO_setConfig(CONFIG_GPIO_BUTTON_1, GPIO_CFG_IN_PU | GPIO_CFG_IN_INT_FALLING);

        /* Install Button callback */
        GPIO_setCallback(CONFIG_GPIO_BUTTON_1, gpioButtonFxn1);
        GPIO_enableInt(CONFIG_GPIO_BUTTON_1);
    }

    return (NULL);
}

```



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
