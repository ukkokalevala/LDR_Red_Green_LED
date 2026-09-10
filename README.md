Pin Definitions:

    ldrPin is defined as the analog pin A0 where the LDR is connected.
    greenPin is defined as the digital pin D1 where the green LED is connected.
    redPin is defined as the digital pin D2 where the red LED is connected.

Setup Function:

    pinMode(greenPin, OUTPUT); sets the green LED pin as an output.
    pinMode(redPin, OUTPUT); sets the red LED pin as an output.
    Serial.begin(115200); initializes serial communication at 115200 baud rate.

Loop Function:

    int ldrValue = analogRead(ldrPin); reads the analog value from the LDR.
    Serial.println(ldrValue); prints the LDR value to the serial monitor.
    The if statement checks if the LDR value is below or equal to 300 (you can adjust this threshold value based on your specific requirements).
        If the condition is true, it turns on the red LED and turns off the green LED.
        If the condition is false, it turns off the red LED and turns on the green LED.
    delay(500); pauses the loop for 500 milliseconds before repeating.
This program will turn on the red LED when the LDR value is below or equal to the threshold and will turn on the green LED when the LDR value is above the threshold.
