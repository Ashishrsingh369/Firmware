# Firmware
Firmware Testing and AI/ML integration on edge.
import serial

ser = serial.Serial('COM3', 9600)  # Adjust port and baud rate
ser.write(b"START\n")
response = ser.readline()
print(f"Response: {response.decode()}")
ser.close()
