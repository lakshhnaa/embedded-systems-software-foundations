# Hardware Abstraction Layer (HAL) and Bare-Metal Systems

## Hardware Abstraction Layer (HAL)
- Software layer between application and hardware
- Hides hardware-specific details
- Provides uniform API for peripherals

---

## Purpose of HAL
- Hardware abstraction
- Portability
- Code reuse
- Easier maintenance

---

## HAL Conceptual Stack
- Application Layer  
- HAL API  
- Device Drivers  
- Hardware Registers  
- Hardware  

Application does not access hardware registers directly.

---

## Benefits of HAL
- Platform independent
- Clean application code
- Easier hardware migration
- Reduced hardware-related bugs

---

## Bare-Metal Programming
- Runs directly on hardware
- No operating system
- Full hardware control

---

## Bare-Metal Characteristics
- No OS
- Single main program
- Deterministic execution
- Minimal memory usage

---

## Typical Bare-Metal Execution Flow
- Reset Handler  
- Hardware Initialization  
- Main Application  
- Infinite Loop  

---

## HAL vs Bare-Metal

| Feature | HAL | Bare-Metal |
|------|----|----|
| Hardware access | Abstracted | Direct |
| Portability | High | Low |
| Performance | Slight overhead | Maximum |
| Code size | Larger | Smaller |
| Complexity | Moderate | Low |

---

## When to Use HAL
- Portability required
- Faster development
- Complex peripherals
- Hardware may change

---

## When to Use Bare-Metal
- Simple systems
- Maximum performance
- Very low memory
- Strict timing constraints

---

# Software Block Diagrams

## Example: HAL-Based Software Block Diagram
<img width="527" height="405" alt="image" src="https://github.com/user-attachments/assets/528b4952-2b21-49e1-925b-ccff40aefa13" />


### Keywords Explanation
- Application Layer → High-level logic
- HAL → Hardware abstraction
- SPI Driver (`spi.c`) → Communication handling
- GPIO Hardware → Physical pin control
- Function calls flow downward
