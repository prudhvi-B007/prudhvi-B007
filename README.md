# **Prudhvi Raj Belide** 👨‍💻 
#### Embedded Systems Engineer

<div align="left">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&duration=3000&pause=1000&color=00FF41&left=true&vCenter=true&width=435&lines=Loading+Firmware...;Initializing+Peripherals...;Setting+up+RTOS...;System+ready!" alt="Typing SVG" />

  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/prudhvibelide10/)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@prudhvi.belide)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:prrbe.0610@gmail.com)


  ```text
  Status Register (PSTAT):
  [x] MS Student @ University of Colorado Boulder
  [x] Embedded Systems & IoT 
  [x] Timeline: 2024-2026
  ```
</div>

## 📟 Memory Map

```ld
/* prudhvi.ld - Linker Script */
MEMORY
{
  SKILLS (rx)      : ORIGIN = 0x00000000, LENGTH = 64K   /* Technical Skills */
  EXPERIENCE (rx)  : ORIGIN = 0x00010000, LENGTH = 32K   /* Work Experience */
  PROJECTS (rx)    : ORIGIN = 0x00020000, LENGTH = 32K   /* Notable Projects */
  RESEARCH (rx)    : ORIGIN = 0x00030000, LENGTH = 16K   /* Publications */
  SOCIAL (rw)      : ORIGIN = 0x00040000, LENGTH = 8K    /* Connect with me */
}
```

## 🔧 Technical Peripherals

<details>
<summary>⚡ Core Modules</summary>

```c
/* system_config.h */
#define MCU_PLATFORMS {
    "ARM Cortex M0/M3/M4",
    "STM32F4xx",
    "MKL16Z32VLH4",
    "ESP32",
    "ZGM130S/230S",
    "8051"
}

#define PROTOCOLS {
    UART_ENABLED   = 1,
    SPI_ENABLED    = 1,
    I2C_ENABLED    = 1,
    ZIGBEE_ENABLED = 1,
    ZWAVE_ENABLED  = 1,
    BLE_ENABLED    = 1
}

typedef struct {
    const char* languages[4];
    const char* frameworks[3];
    const char* tools[7];
} Skills_t;

Skills_t mySkills = {
    .languages = {"C", "Embedded C", "Assembly", "Python"},
    .frameworks = {"FreeRTOS", "Bare-metal", "Embedded Linux"},
    .tools = {"Simplicity Studio", "STM32CubeIDE", "Keil", 
              "VSCode", "Altium", "Oscilloscope", "Logic Analyzer"}
};
```
</details>

## 🔄 Interrupt Vector Table

```asm
; experience_vector.s
.section .vectors
    .word   _stack_top              ; Stack pointer
    .word   hogar_controls_isr      ; 3.5 years as Embedded Firmware Developer
    .word   drdo_research_isr       ; Research Internship
    .word   people_tech_isr         ; Embedded Developer Intern

hogar_controls_isr:
    PUSH    {R0-R3, LR}
    BL      develop_iot_devices     ; IoT Home Automation
    BL      implement_protocols     ; Z-Wave and Zigbee
    POP     {R0-R3, PC}
```

## 📚 Research Cache

1. [Sixth Sense Robot Using Image Processing](https://ieeexplore.ieee.org/document/9770743)
   - Implementation of advanced image processing techniques for robotic control

2. [Heart Defect Monitoring System](https://ieeexplore.ieee.org/document/9770624)
   - Real-time heart monitoring using embedded systems

3. [Smart Transportation System](https://ieeexplore.ieee.org/document/9545525)
   - IoT-based intelligent transportation management


## 💭 Debug Console

```c
#define DEBUG_WISDOM(msg) __asm__ __volatile__("BKPT #0\n\t" : : "r"(msg))

void embedded_thoughts(void) {
    DEBUG_WISDOM("Rule Number 1 : Never disturb the working Code!");
    DEBUG_WISDOM("When your interrupt handler has an interrupt handler, it's time to rethink life choices");
    DEBUG_WISDOM("My code is perfect, must be a hardware issue. My hardware is perfect, must be a code issue");
}
```




<div align="center">
  
