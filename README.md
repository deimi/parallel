# parallel



General purpose C library for parallel communications on Raspberry Pi
   - supports 6800 and 8080 protocols, both 4 bits and 8 bits
   - supports arbitrary GPIO pins from 0 to 27
   - supports writing and reading, reading is optional
   - supports objective oriented programming, initialisation returns the pointer to chip instance
   - all RPi data lines by default in read mode in order to avoid possible conflict and destruction of GPIO pins

