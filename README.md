# Smart-Medibox
![SMART MEDIBOX](https://github.com/Shathira-Lakdilu/Smart-Medibox/assets/127112210/4fbc4f7f-0759-4643-ad55-3a0be6399715)
The Smart Medibox is a revolutionary device designed to help you manage your medications effectively and efficiently. It goes beyond your traditional pill organizer by incorporating intelligent features that remind you to take your medication on time and alert you when the surrounding environment is not optimal for its storage.

### Time to Take Your Medicine!

Forget the days of missed doses or scrambling to remember what medication you need to take next. The Smart Medibox features a built-in timer that can be programmed to remind you when it's time to take your medication.

## Hardware components

- ESP32 Development Board
- DHT11 Temperature & Humidity Sensor
- OLED 64x128 Display Module
- Buzzer
- Pushbutton switch 
- Resistor 1 kohm
- Resistor 330 ohm

 **Smart Medibox:** Your Reliable Medication Reminder and Environment Guardian

Say goodbye to missed doses and worries about medication spoilage with the Smart Medibox! This innovative device acts as your personal medication assistant, reminding you to take your medication on time and ensuring optimal storage conditions.

### Key functionalities:
-   **Timely medication reminders:** Set alarms for each medication and receive clear audio notifications when it's time to take your dosage.
-   **Environmental monitoring:** Built-in sensors monitor temperature and humidity levels within the Medibox, alerting you with an alarm if they fall outside the recommended range for your medication.
-   **Informative display:** A clear and concise display showcases the current time, date, and upcoming alarm information, ensuring you stay on track.
-   **Simple setup:** Easily set the date and time upon initial use and enjoy the benefits of your Smart Medibox

**Smart Medibox Operation Flow Chart:** Navigating Efficient Medication Management

The Smart Medibox's operation flow chart provides a clear and concise overview of the device's intelligent functionality. This visual guide details the step-by-step process, illustrating how the Smart Medibox ensures timely medication reminders and optimal storage conditions for your medications.

![Screenshot 2023-11-27 225838](https://github.com/Shathira-Lakdilu/Smart-Medibox/assets/127112210/f5810caa-c3a4-437d-8723-68780df07c4c)

## Function Descriptions for Smart Medibox Project

**1. void print_line(String message):**

This function prints the provided `String` message as a single line on the OLED display. This allows for displaying information such as medication reminders, time updates, and warning messages.

**2. void print_time_now():**

This function retrieves the current time and displays it on the OLED display in the format of "Days, Hours, Minutes, Seconds". This provides users with a clear and concise overview of the time.

**3. void update_time():**

This function utilizes the Arduino `millis()` function to continuously update the internal clock of the Smart Medibox. This ensures that the displayed time and alarm triggers are accurate.

**4. void update_time_with_check_alarm():**

This function combines the functionalities of `print_time_now()` and alarm checking. It displays the current time and also checks if the current time matches the set time for any medication. If a medication reminder is due, it triggers the `ring_alarm` function.

**5. void ring_alarm():**

This function activates the alarm when a medication reminder triggers. It performs three actions:

-   Prints a message on the OLED display reminding the user to take medication.
-   Activates the buzzer to create an audible alert.
-   Lights up an LED for a visual indication of the alarm.

**6. int wait_for_button_press():**

This function monitors the user's interaction with the push buttons. It continuously checks if any button is pressed and returns an integer value representing the specific button that was pressed. This allows for user interaction with the device and navigation through different menus.

**7. void go_to_menu():**

This function analyzes the button pressed, identified by the `wait_for_button_press()` function, and switches the Smart Medibox to the appropriate mode. This enables users to access different functionalities such as setting alarms, viewing medication schedules, and monitoring environmental conditions.

**8. void run_mode():**

This function executes the code specific to the currently selected mode. Depending on the user's input, it might handle medication reminders, display settings, or environmental monitoring tasks.

**9. void check_temp():**

This function utilizes the DHT22 sensor to measure the temperature and humidity within the Medibox. It then compares these values to the pre-configured optimal range.

## Schematic Design
![schametic](https://github.com/Shathira-Lakdilu/Smart-Medibox/assets/127112210/23a7e37f-f73f-4b3b-a19d-eb8731b10c8d)

## PCB Design
![PCB](https://github.com/Shathira-Lakdilu/Smart-Medibox/assets/127112210/e9ee38d6-f2cb-46ad-b106-abe445b0bb70)
![Screenshot_20221223_032322](https://github.com/Shathira-Lakdilu/Smart-Medibox/assets/127112210/afdd79af-faef-4477-9959-998ec7e6dfbd)

## Additional Resources:
**Simulation on Wokwi:**  This interactive simulation allows you to experience 
![medibox wokwi](https://github.com/Shathira-Lakdilu/Smart-Medibox/assets/127112210/e85d6681-5624-4e87-9544-d817fd7cbf44)
the Smart Medibox's functionality firsthand.


