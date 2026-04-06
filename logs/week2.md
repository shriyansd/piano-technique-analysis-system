# Week 2 — Build V1 prototype

## Monday - Day 1
- Researching components to purchase for the glove prototype

### Microcontroller Selection

#### Option 1: [Arduino Nano V3.0 (CH340)](https://www.amazon.com/LAFVIN-Board-ATmega328P-Micro-Controller-Arduino/dp/B07G99NNXL/ref=sr_1_2?crid=3L0N2GRXETV9Q&dib=eyJ2IjoiMSJ9.0uv9j0wmlzOzbkEwda-bJ3Y4Wh9T6H5-V8lbsAVGpk4aWFfD_z6dyBKOcacM0i_NfxYfHuLqqGjZ3dZ_1HPW0UaI9nAEEcJwjo7ZVk00v8IbW1nUWKsMCAjDA_ufg3cggjWwQFRhIG0_nTjc7xzeRaOLw9FCxtk0NMfTtONl-tXmnNMC_sTWlXy8a-BOlIQN8_kO_t-0VLhGM6DjMcLkxAWNWt-4oB3iEavbbzex_Ro.50usVLM4L9TUChc-SZFysLw-6jW7xXDGy-m0DuYBQL0&dib_tag=se&keywords=arduino+nano+v3.0+ch340&qid=1775513056&sprefix=arduino+nano+v3.0+ch340%2Caps%2C236&sr=8-2)
  - Pros:
      - 8 analog input pins - sufficient for multiple sensors (FSR, flex, mic)
      - Simple and beginner-friendly - ideal for rapid prototyping  
      - 5V logic - directly compatible with most sensors (no level shifting required)  
      - Low cost - allows for experimentation, replacement, and iteration  
      - Stable and predictable - no background wireless processes interfering with timing  
  - Cons:
      - No built-in Wi-Fi or Bluetooth (limits wireless communication)  
      - Limited processing power and memory - not suitable for advanced real-time processing  
      - Requires wired connection to laptop for data transfer 

#### Option 2: [Arduino Nano ESP32](https://www.amazon.com/Arduino-ABX00083-Bluetooth-MicroPython-Compatible/dp/B0C947BHK5/ref=sr_1_1_sspa?crid=S9DJAC6PA4CV&dib=eyJ2IjoiMSJ9.QmNYvO8VeEYJRoPLV8e0zXTVa4f1jG2BDdr1cCnXe_OQPxll2p4MRtEvcdyAjUzwsmYcBqV7VpP9HKNBOMKQQg3XW9ebQyHS8mk-s2wtHu4p0E4pNznY9hmcluU_dihlxDkAuGATYmuPyojAIAWTYYe5l510tamQi6-mrmNp_W8y3TrCawjxOSKm4fDRZ1-JHrEIyFbAVd-8vva1Y-MXEcJYSngBD3bA1_cxP2qB_ZA.q6huMYtKsXLQ11GgsgKt1kUeKT21MzwCJUtiEzoXrPU&dib_tag=se&keywords=arduino%2Bnano&qid=1775511316&sprefix=arduino%2Bnan%2Caps%2C186&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1) (future upgrade)
  - Pros:
    - Built-in Wi-Fi and Bluetooth - enables wireless data transfer and mobile app integration   
    - Significantly higher processing power - supports more complex analysis and future ML features  
    - More memory - allows scaling of software and data handling  

  - Cons:
    - Increased complexity - harder to debug, especially in early stages  
    - 3.3V logic - may require additional circuitry for some sensors  
    - Wireless communication introduces latency and connection issues  
    - Overkill for initial prototype focused on basic sensor validation

### Sensor Selection

#### FSR Sensor: [FSR402 Force Sensor](https://www.amazon.com/FSR402-Pressure-Sensitive-Resistor-Arduino-Raspberry/dp/B0DHGPGBBJ/ref=sr_1_2?crid=2K3QVROTP9Z3Z&dib=eyJ2IjoiMSJ9.VeHQmOAn3OWwQTRbXl8YVHb7P3_E-R8kOP0-v-nrsZaQADNj2epnSpctO6Jz3E21nrOD9tFWHPlyfJ25YcMYIUH1J5jmTH6kJRG6MMBm2xZwuhR5P_dyHYBDkUe4LZjhUpoF5Gw1Bwl1K3luL8LR0xLnLJ3GB9_k10pdru3mecFoXumiQVmwob_H4o5DmQQYf7HUzRBwC-KUJRvK9Ur3WMHJ7s4m4y8Kt1X_iQY_smQ.YYuz_OJ4hQXnImBCaSAfRKUI5qply6jajUI8xX2cP3M&dib_tag=se&keywords=fsr%2Bsensor%2Barduino&qid=1775513250&sprefix=fsr%2Bsensor%2Barduino%2Caps%2C257&sr=8-2&th=1)  
  - Need 10k resistors
  - Jumper wires for extension
