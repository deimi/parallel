# parallel

This repository is dedicated to fast parallel communications on Raspberry Pi.  The speed is essential when communicating with large liquid crystal displays, as a lot of data has to be transferred for a single full screen picture.

## Main library

### parallel.c

General purpose C library for parallel communications on Raspberry Pi
   - supports 6800 and 8080 protocols, both 4 bits and 8 bits
   - supports arbitrary GPIO pins from 0 to 27
   - supports writing and reading, reading is optional
   - supports objective oriented programming, initialisation returns the pointer to chip instance
   - all RPi data lines by default in read mode in order to avoid possible conflict and destruction of GPIO pins

### parallel.so

C library compiled for use with Python

## Examples of use

### RA6963.py

Python library for RA6963 controller chip (requires parallel.so)

### RA6963_test.py

Python test file for the Python Library (reqires RA6963.py)

The result: https://youtu.be/7CxnJM1tHzU

Note: If you don't want to control backlight from the program, set bl=-1.  If you are not interested in backlight PWM, set pwm=False.  If there are problems, try to make waiting times longer.
