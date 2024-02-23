/*
 * Please find this basic code below for the BME680. Unfortunately, the BME680's internal AQI only works with the FireBeetle ESP8266 IoT Microcontroller.
 * After exploring forums and datasheets for the sensor's resistance levels and outputs, as well as developing an algorithm, I've created a solution that should work with:
 * - ESP32 Dev Kit
 * - ESP S3 32S
 * - Arduino UNO
 * - Arduino Mega
 * Adjust header files and other supporting libraries to suit your needs, as this is an I2C device.
 * The BME680 library is required, and typically, you don't need to manually include the math library using #include <math.h> or #include <cmath>,
 * as it is included by default in the standard Arduino environment.
 * However, if you're working in a different environment or with plain C/C++ files, you might need to include it explicitly.
 */

/* You can use an accurate altitude to calibrate sea level air pressure. 
 * And then use this calibrated sea level pressure as a reference to obtain the calibrated altitude.
 * In this case, 33.0m is my locations accurate altitude.
 */
