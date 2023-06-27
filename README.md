# Bosch_BMI088_new_data_interrupt_setup

This Arduino sketch configures the BMI088 sensor's registry, specifically targeting interrupts 1 and 3, and assigns them as new data interrupts for the accelerometer and gyroscope. It uses the Wire library to communicate with the sensor over I2C.

The code starts by including the Wire library and defining the I2C addresses for the accelerometer and gyroscope of the BMI088 sensor. It also defines the interrupt mapping registers for each.

In the setup() function, the I2C interface is initialized and the clock speed is set to 400kHz. The writeRegister function is then used to set interrupt 1 as a new data interrupt for the accelerometer, and interrupt 3 as a new data interrupt for the gyroscope.

The writeRegister function takes three arguments - the device address, the register address, and the data to write to the register. It begins an I2C transmission with the specified device, writes the register address and data, and then ends the transmission.

By using this Arduino code in your sketch, you can quickly set up your BMI088 sensor and start gathering accelerometer and gyroscope data in no time.
