# Software Layers in Embedded Systems

## Software Layers
- Logical separation of embedded software
- Each layer has specific responsibility
- Interacts only with adjacent layers

---

## Purpose
- Hardware isolation
- Code reuse
- Portability
- Maintainability

---

## Typical Embedded Software Stack


---

## Layer Summary
- **Application** → System logic
- **Middleware** → Reusable services
- **OS (optional)** → Scheduling, memory
- **Drivers / HAL** → Hardware interface
- **Hardware** → Physical components

---

## HAL (Quick)
- Abstracts hardware
- Portable interface
- No direct register access by application

---

## Bootloader (Intro)
- Runs before application
- Initializes system
- Loads firmware

---

# Software Components in Embedded Systems

## Software Components
- Modular functional units
- Interface-based communication

---

## Types
- Control Libraries
- Peripheral Libraries (SPI, UART, GPIO)
- Firmware Components
- Hardware Drivers

---

## Component Architecture

<img width="1761" height="849" alt="image" src="https://github.com/user-attachments/assets/f1cd61bf-da26-49d9-ac8c-a79c41d78a1a" />


---

## Diagram Keywords
- Library-based design
- Interface stability
- Hardware abstraction
- Replaceable components

---

## Reusability & Versioning
- New component → same interface
- Old component → legacy
- Lower layers unchanged

---

## Hardware Mapping
- GPIO → RGB LED
- SPI → nRF24L01+
- UART → Off-board device

---


