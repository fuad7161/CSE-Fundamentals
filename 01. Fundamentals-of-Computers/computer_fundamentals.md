# Computer Fundamentals — Study Notes

## Table of Contents
1. [Introduction to Computers](#1-introduction-to-computers)
2. [Computer Organisation and Architecture](#2-computer-organisation-and-architecture)
3. [Memory and Storage Systems](#3-memory-and-storage-systems)
4. [Input and Output Devices](#4-input-and-output-devices)
5. [Computer Codes](#5-computer-codes)
6. [Computer Arithmetic](#6-computer-arithmetic)
7. [Boolean Algebra](#7-boolean-algebra)
8. [Logic Gates and Digital Circuits](#8-logic-gates-and-digital-circuits)
9. [Computer Software](#9-computer-software)
10. [Operating Systems](#10-operating-systems)
11. [Programming Languages](#11-programming-languages)
12. [Data Communications and Networks](#12-data-communications-and-networks)
13. [Internet and World Wide Web](#13-internet-and-world-wide-web)

---

## 1. INTRODUCTION TO COMPUTERS

### What is a Computer?
A computer is an electronic machine that:
- Takes input from the user
- Processes the given input
- Generates output in the form of useful information

### Computer Components
| Component | Description |
|---|---|
| CPU | "Brain" of computer - controls and executes instructions |
| Monitor | Displays information visually |
| Keyboard/Mouse | Input devices |

### Characteristics of Computers
| Characteristic | Explanation |
|---|---|
| Speed | Solves complex problems in seconds |
| Storage | Huge data storage capacity |
| Accuracy | High precision calculations |
| Reliability | Consistent error-free results |
| Versatility | Performs many different tasks |
| Diligence | Repeats calculations without fatigue |

### Evolution of Computers

**Manual Computing Devices**

| Device | Inventor | Year | Purpose |
|---|---|---|---|
| Abacus | - | ~5000 years ago | Counting frame with beads on wires |
| Napier Bones | John Napier | 1614 | Multiplication and division |
| Slide Rule | Edmund Gunter | 1620 | Logarithms and trigonometry |
| Pascaline | Blaise Pascal | 1642 | Addition/subtraction (toothed wheels) |
| Stepped Reckoner | Gottfried Leibniz | - | Multiplication, division, square roots |

**Automated Computing Devices**

| Device | Inventor | Year | Key Features |
|---|---|---|---|
| Difference Engine | Charles Babbage | 1822 | First automatic mechanical computer |
| Analytical Engine | Charles Babbage | 1833 | First general-purpose programmable digital computer |
| MARK I | Howard Aiken | 1944 | Multiplication in 6 seconds |
| Colossus | Alan Turing | 1944 | First pure electronic digital computer |
| ENIAC | Eckert & Mauchly | 1946 | 17,468 vacuum tubes, 1000x faster than MARK I |
| EDVAC | Eckert & Mauchly | 1949 | First stored-program computer |
| EDSAC | Maurice Wilkes | 1949 | Used mercury delay lines for memory |
| UNIVAC | Eckert & Mauchly | 1951 | First commercial computer |

**Generations of Computers**

| Generation | Period | Technology Used | Key Features |
|---|---|---|---|
| 1st | 1940-1956 | Vacuum tubes | Machine language, bulky, heat issues |
| 2nd | 1956-1963 | Transistors | Smaller, faster, assembly language |
| 3rd | 1964-1975 | Integrated Circuits (ICs) | Smaller, high-level languages |
| 4th | 1975-1989 | LSI/VLSI, Microprocessors | Personal computers, GUI, LAN |
| 5th | 1989-present | ULSI technology | Laptops, PDAs, Internet, parallel processing |

### Classification of Computers

**Based on Operating Principles**

| Type | Description | Example |
|---|---|---|
| Analog | Continuous electrical signals | Operational amplifiers |
| Digital | Processes data in 0s and 1s | Desktop computers |
| Hybrid | Combines analog and digital | Hospital heartbeat monitors |

**Based on Size and Capability**

| Type | Description | Examples |
|---|---|---|
| Microcomputer | Small, personal use | Desktop, Laptop, PDA |
| Mini Computer | Mid-range, 4-200 users | PDP 11, IBM 8000 series |
| Mainframe | Large, enterprise use | IBM 3000, VAX 8000 |
| Super Computer | Fastest, complex operations | CRAY 3, PARAM |

### Practice Questions

**Fill in the Blanks**
1. A ______ is an electronic machine that processes data.
2. The "brain" of the computer is the ______.
3. ______ is considered the father of modern digital computers.
4. The first generation computers used ______ technology.
5. ______ computers use continuous electrical signals.

**Multiple Choice Questions**
1. Which component is known as the brain of computer?
   A) Monitor B) CPU C) Memory D) Keyboard
2. Who is known as the father of modern digital computers?
   A) Alan Turing B) Charles Babbage C) John Mauchly D) Howard Aiken
3. Which generation used transistors?
   A) First B) Second C) Third D) Fourth
4. Laptop computers belong to which category?
   A) Microcomputer B) Minicomputer C) Mainframe D) Supercomputer

**Discussion Questions**
- Explain the characteristics of modern digital computers.
- Differentiate between analog and digital computers.
- Describe the five generations of computers.

---

## 2. COMPUTER ORGANISATION AND ARCHITECTURE

### Key Definitions
- **Computer Architecture:** Definition of basic attributes of hardware components and their interconnections
- **Computer Organisation:** Design and physical arrangement of hardware units

### Central Processing Unit (CPU)

**CPU Components**

| Component | Function |
|---|---|
| Arithmetic Unit (AU) | Performs arithmetic operations (+,-,×,÷) |
| Logic Unit (LU) | Performs logical operations (>,<,=,AND,OR) |
| Control Unit (CU) | Controls flow of data and information |
| Main Memory | RAM - temporary storage |
| Cache Memory | Fast memory for frequently accessed data |
| Registers | High-speed temporary storage |

### CPU Cycle (Machine Cycle)
```
Fetch → Decode → Execute → Store
```

| Phase | Description |
|---|---|
| Fetch | Retrieves instruction from memory |
| Decode | Breaks instruction into opcode and operands |
| Execute | ALU performs the operation |
| Store | Results stored back in memory |

### Cache Memory Types
| Type | Location | Speed | Size |
|---|---|---|---|
| L1 Cache (Primary) | Inside CPU | Fastest | Smallest |
| L2 Cache (Secondary) | On Motherboard | Slower | Larger |

### Registers
| Register | Purpose |
|---|---|
| Program Counter (PC) | Tracks next instruction |
| Instruction Register (IR) | Holds instruction to be decoded |
| Memory Address Register (MAR) | Holds memory address |
| Memory Buffer Register (MBR) | Stores data from/to CPU |
| Memory Data Register (MDR) | Stores operands and data |
| Accumulator (ACC) | Stores ALU results |

### Processor Communication

**Memory Read Operation**
1. Processor loads address into MAR
2. Issues READ control signal
3. Memory loads data into MDR
4. Data transferred to processor

**Memory Write Operation**
1. Processor loads address into MAR
2. Processor loads data into MDR
3. Issues WRITE control signal
4. Memory stores data

### The Bus System
| Bus Type | Direction | Purpose |
|---|---|---|
| Data Bus | Bidirectional | Transfers data |
| Address Bus | Unidirectional | Transfers addresses |
| Control Bus | Bidirectional | Transfers control signals |

### Instruction Sets
| Feature | CISC | RISC |
|---|---|---|
| Instructions | 100-250 complex | 0-100 simple |
| Format | Variable length | Fixed 32-bit |
| Speed | Slower | Faster (single clock cycle) |
| Design | Complex hardware | Simple hardware |
| Memory Access | Frequent | Minimal (register-based) |

### Practice Questions

**Fill in the Blanks**
1. The CPU is popularly known as the ______ of the computer.
2. The ______ unit performs arithmetic operations.
3. The ______ register keeps track of the next instruction.
4. ______ memory is faster than main memory.
5. RISC stands for ______.

**Multiple Choice Questions**
1. Which is not an internal component of CPU?
   A) Arithmetic Unit B) Logic Unit C) Interface Unit D) Control Unit
2. Which cache is known as internal cache?
   A) L1 B) L2 C) L3 D) L4
3. The machine cycle consists of:
   A) Fetch-Execute B) Fetch-Decode-Execute-Store C) Store-Fetch-Decode D) None of these

**Discussion Questions**
- Draw and explain the block diagram of a computer system.
- Explain the concept of cache memory.
- Differentiate between CISC and RISC processors.

---

## 3. MEMORY AND STORAGE SYSTEMS

### Memory Types

**Primary Memory (Volatile)**

| Type | Description | Characteristics |
|---|---|---|
| RAM | Random Access Memory | Volatile, Read/Write |
| ROM | Read Only Memory | Non-volatile, Read-only |

**Secondary Memory (Non-volatile)**

| Type | Examples |
|---|---|
| Magnetic | Hard disks, Floppy disks, Magnetic tapes |
| Optical | CD, DVD, Blu-ray |
| Solid State | USB drives, Memory cards |

### Memory Representation
- **Bit:** Smallest unit (0 or 1)
- **Byte:** 8 bits (smallest addressable unit)
- **Word:** 2 or 4 bytes
- **Kilobyte (KB):** 1,024 bytes
- **Megabyte (MB):** 1,048,576 bytes
- **Gigabyte (GB):** 1,073,741,824 bytes

### RAM Types
| Type | Memory Cell | Needs Refresh | Speed | Cost |
|---|---|---|---|---|
| SRAM | Transistors | No | Fast | Expensive |
| DRAM | Transistor + Capacitor | Yes | Slower | Cheaper |

### ROM Types
| Type | Erasable | Method |
|---|---|---|
| PROM | No | - |
| EPROM | Yes | UV Light |
| EEPROM | Yes | Electric Charge |
| Flash ROM | Yes | Electric Charge (block by block) |

### Magnetic Storage Systems

**Magnetic Tapes**
- Sequential access
- Used for backup
- Low cost, large capacity

**Magnetic Disks**
- Random access
- Tracks: Concentric circles
- Sectors: Broken up units of tracks
- Types: Hard disks, Floppy disks

### Optical Storage Systems
| Type | Read/Write | Examples |
|---|---|---|
| Read-only | Read only | CD-ROM, DVD-ROM |
| WORM | Write once, read many | CD-R, DVD-R |
| Rewritable | Read/Write multiple times | CD-RW, DVD-RW |

### Solid-State Storage Devices (SSD)
| Feature | Advantage | Disadvantage |
|---|---|---|
| Speed | Faster than hard drives | - |
| Power | Low power consumption | - |
| Reliability | No moving parts | - |
| Cost | - | More expensive |
| Capacity | - | Lower capacity |
| Writing Speed | - | Slower than hard drives |

### Storage Evaluation Criteria
- **Access Mode:** Random, Sequential, Direct
- **Access Time:** Time to retrieve data
- **Storage Capacity:** Size available
- **Storage Type:** Volatile/Non-volatile
- **Cost:** Cost per bit of storage

### Practice Questions

**Fill in the Blanks**
1. ______ memory is volatile while ______ memory is non-volatile.
2. The smallest addressable unit of memory is ______.
3. ______ and ______ are the two main types of RAM.
4. A magnetic disk surface contains ______ and ______.
5. SSD stands for ______.

**Multiple Choice Questions**
1. Which memory is volatile?
   A) ROM B) RAM C) Hard Disk D) CD-ROM
2. Which is the fastest type of memory?
   A) Cache B) RAM C) Secondary memory D) ROM
3. A group of 8 bits is called:
   A) Word B) Byte C) Nibble D) Kilobyte

**Discussion Questions**
- Explain the memory hierarchy with a diagram.
- Differentiate between SRAM and DRAM.
- Explain the various types of ROM.
- Compare magnetic, optical, and solid-state storage.

---

## 4. INPUT AND OUTPUT DEVICES

### Input Devices

**Keyboard**
- Alphanumeric keys: Letters and numbers
- Function keys: F1-F12 for specific tasks
- Central keys: Arrow keys, SHIFT, ALT, CTRL
- Numeric keypad: Calculator-like keys
- Special purpose keys: Escape, Insert, Delete, etc.

**Pointing Devices**

| Device | Description | Use |
|---|---|---|
| Mouse | Hand-held pointing device | GUI operations |
| Mechanical Mouse | Ball and rollers | Cursor movement |
| Optical Mouse | LED and optical sensor | More accurate cursor |
| Trackball | Rolling ball in socket | CAD, portable computers |
| Light Pen | Light-sensitive pen | Drawing on screen |
| Joystick | Stick and buttons | Games, CAD |
| Touchscreen | Direct touch interface | ATMs, PDAs, phones |

**Scanning Devices**

| Scanner Type | Characteristics |
|---|---|
| Hand-held | Small, scans up to 5 inches |
| Flatbed | Standard size, glass pane, CCD technology |
| Drum | High resolution, PMT technology |
| Slide | Scans slides and film negatives |

**Optical Recognition Devices**

| Device | Application |
|---|---|
| OCR | Converts printed text to editable form |
| OMR | Multiple choice answer sheets |
| MICR | Bank cheques processing |
| Bar Code Reader | Supermarket items, library books |

**Other Input Devices**

| Device | Purpose |
|---|---|
| Digital Camera | Captures images electronically |
| Voice Recognition | Converts speech to machine code |
| Data Acquisition Sensors | Detects physical quantities |
| Microphone | Converts sound to electrical signals |
| Webcam | Records video/images |
| Graphics Tablet | Enters pictorial information |

### Output Devices

**Display Monitors**

| Type | Technology | Pros | Cons |
|---|---|---|---|
| CRT | Cathode Ray Tube | High contrast, colour depth | Bulky, high power |
| LCD | Liquid Crystal Display | Slim, low power | Fixed resolution |
| TFT | Thin Film Transistor | Better quality than LCD | More expensive |

**Printers**

| Printer Type | Speed | Quality | Cost | Noise |
|---|---|---|---|---|
| Dot Matrix | Slow | Low | Cheap | Loud |
| Daisy Wheel | Very Slow | Good | Moderate | Loud |
| Drum Printer | High | Low | Moderate | Loud |
| Ink-jet | Moderate | High | Moderate | Quiet |
| Laser | High | Excellent | Expensive | Quiet |

**Plotters**

| Type | How it Works |
|---|---|
| Drum Plotter | Pen moves vertically, paper moves horizontally |
| Flat-bed Plotter | Pen moves in X/Y direction, paper fixed |
| Ink-jet Plotter | Sprays ink droplets |
| Electrostatic Plotter | Uses electrostatic charges |

**Voice Output Systems**
- Reproduction: Uses recorded human voice
- Speech Synthesis: Converts written text to speech

**Projectors**

| Type | Use |
|---|---|
| Ultralight | Portable presentations |
| Conference Room | Large venues, business meetings |
| Fixed Installation | Permanent installations |

**Terminals**

| Type | Processing Power |
|---|---|
| Intelligent | Full processing power |
| Smart | Limited processing |
| Dumb | No processing power |

### Practice Questions

**Fill in the Blanks**
1. ______ devices are used for moving the cursor on the screen.
2. An ______ mouse uses LEDs and optical sensors.
3. ______ scanners use Photo Multiplier Tubes technology.
4. MICR stands for ______.
5. CRT stands for ______.

**Multiple Choice Questions**
1. Which is not an input device?
   A) Scanner B) Plotter C) Keyboard D) Mouse
2. Which printer is an impact printer?
   A) Ink-jet B) Laser C) Dot Matrix D) Thermal
3. What does OCR stand for?
   A) Optical Character Recognition B) Optical Code Reader C) Output Character Recognition D) Optional Code Reader

**Discussion Questions**
- Explain the different types of pointing devices.
- Differentiate between impact and non-impact printers.
- Compare CRT, LCD, and TFT monitors.
- Explain the working of MICR devices.

---

## 5. COMPUTER CODES

### Positional Number Systems
| System | Base | Digits/Symbols |
|---|---|---|
| Decimal | 10 | 0-9 |
| Binary | 2 | 0, 1 |
| Hexadecimal | 16 | 0-9, A-F |
| Octal | 8 | 0-7 |

### Binary System
- **Bit:** Binary digit (0 or 1)
- **Nibble:** 4 bits
- **Byte:** 8 bits
- **Word:** 16 bits
- **Double Word:** 32 bits

### 4-Bit BCD Systems

**Weighted 8421 Code**

| Decimal | 8421 Code |
|---|---|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |

**Excess-3 Code**
Add 3 to each digit before converting to binary

### 8-Bit BCD Systems (Alphanumeric Codes)
| Code | Developer | Bits | Use |
|---|---|---|---|
| EBCDIC | IBM | 8 | IBM systems |
| ASCII | Multiple | 7/8 | Widely used |
| Gray Code | - | 8 | Contiguous digits differ by 1 bit |

### 16-Bit Unicode
- International character set
- Supports 65,536 characters
- Handles all major languages

### Number System Conversions

**Binary to Decimal**
```
10101101₂ = 1×2⁷ + 0×2⁶ + 1×2⁵ + 0×2⁴ + 1×2³ + 1×2² + 0×2¹ + 1×2⁰
           = 128 + 0 + 32 + 0 + 8 + 4 + 0 + 1 = 173₁₀
```

**Decimal to Binary**
```
30₁₀ → 30÷2=15 rem 0
      15÷2=7 rem 1
      7÷2=3 rem 1
      3÷2=1 rem 1
      1÷2=0 rem 1
Result: 11110₂
```

**Octal to Hexadecimal**
```
365₈ → 011 110 101 (binary)
     → 0000 1111 0101 (4-bit grouping)
     → 0F5₁₆
```

### Practice Questions

**Fill in the Blanks**
1. The decimal system uses base ______.
2. A combination of 8 bits is called a ______.
3. The hexadecimal system uses ______ symbols.
4. BCD stands for ______.
5. ASCII stands for ______.

**Multiple Choice Questions**
1. Which is not a positional number system?
   A) Binary B) Octal C) Decimal D) Roman
2. The binary equivalent of decimal 6 is:
   A) 0110 B) 1000 C) 0010 D) 0111
3. Which code is an 8-bit alphanumeric code?
   A) Gray Code B) BCD C) ASCII D) Excess-3

**Discussion Questions**
- Explain the various positional number systems.
- Convert the following: (1101)₂ to decimal; (25)₁₀ to binary; (A3)₁₆ to decimal
- Describe the Gray code and its applications.

---

## 6. COMPUTER ARITHMETIC

### Binary Addition Rules
| A | B | Sum | Carry |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

### Binary Multiplication
- Same as decimal multiplication
- Only 0 and 1 results
- Can be performed as repeated addition

### Binary Subtraction
| A | B | Difference | Borrow |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 0 |

### Binary Division
- Same as decimal division
- Uses binary subtraction
- Dividend must be greater than divisor

### Signed/Unsigned Numbers
- **Unsigned:** Positive numbers only
- **Signed:** Can be positive or negative
- **Sign bit:** 0 for positive, 1 for negative

### Complements

**One's Complement**
- Flip all bits (0→1, 1→0)
- Two representations of zero

**Two's Complement**
- One's complement + 1
- Widely used for negative numbers
- Single representation for zero

| Integer | One's Complement | Two's Complement |
|---|---|---|
| +7 | 0111 | 0111 |
| -7 | 1000 | 1001 |
| +0 | 0000 | 0000 |
| -0 | 1111 | (no representation) |

### Integer Representations
| Representation | Range | Uses |
|---|---|---|
| Unsigned Magnitude | 0 to (2^n - 1) | Positive integers |
| Signed Magnitude | -(2^n-1) to +(2^n-1) | Positive and negative |
| One's Complement | -(2^n-1) to +(2^n-1) | Negative integers |
| Two's Complement | -2^(n-1) to +(2^(n-1)-1) | Most common |

### Floating-Point Representation
```
Number = Mantissa × Base^Exponent
Example: 325.123 = 3.25123 × 10²
```

**IEEE 754 Format (32-bit)**

| Component | Bits | Description |
|---|---|---|
| Sign | 1 | 0=positive, 1=negative |
| Exponent | 8 | Excess-127 notation |
| Mantissa | 23 | Normalized fraction |

### Integer Arithmetic (Signed-Magnitude System)
- Same sign: Add magnitudes, keep sign
- Opposite signs: Subtract smaller from larger
- Multiplication: Multiply magnitudes, XOR signs

### Floating-Point Arithmetic
- Addition: Make exponents equal, add mantissas
- Subtraction: Make exponents equal, subtract mantissas
- Multiplication: Multiply mantissas, add exponents
- Division: Divide mantissas, subtract exponents

### Arithmetic Errors
| Error Type | Description |
|---|---|
| Overflow | Number too large to handle |
| Underflow | Number too small to handle |
| Truncation | Loss of low-order bits |
| Sign Error | Unsigned↔Signed conversion |

### Laws of Arithmetic
| Law | Multiplication | Addition |
|---|---|---|
| Identity | a×1 = a | a+0 = a |
| Commutative | a×b = b×a | a+b = b+a |
| Associative | a×(b×c) = (a×b)×c | a+(b+c) = (a+b)+c |
| Distributive | a×(b+c) = a×b + a×c | - |

### Practice Questions

**Fill in the Blanks**
1. Binary addition follows ______ rules.
2. The ______ bit indicates the sign of a number.
3. Two's complement of a number = ______ + 1.
4. ______ error occurs when a number is too large.
5. The exponent part in floating-point uses ______ notation.

**Multiple Choice Questions**
1. Binary multiplication is repeated:
   A) Addition B) Subtraction C) Division D) Multiplication
2. The sign bit for negative numbers is:
   A) 0 B) 1 C) -1 D) Not defined
3. Which is not a valid binary addition rule?
   A) 0+0=0 B) 1+1=0 with carry 1 C) 1+0=1 D) 1+1=0 with no carry

**Discussion Questions**
- Explain binary addition, subtraction, multiplication, and division.
- What is the purpose of two's complement representation?
- Explain floating-point representation with an example.
- Describe the different types of arithmetic errors.

---

## 7. BOOLEAN ALGEBRA

### Introduction
- Developed by George Boole in 1854
- Applied to switching circuits by Claude Shannon in 1938
- Also called Switching Algebra
- Values: 0 (FALSE) and 1 (TRUE)

### Boolean Variables and Operators
| Operator | Symbol | Type |
|---|---|---|
| Logical Addition (OR) | + | Binary |
| Logical Multiplication (AND) | · | Binary |
| Logical Complement (NOT) | ¬ | Unary |

### Boolean Operations

**AND Operation** — A·B = 1 only when A=1 AND B=1

| A | B | A·B |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

**OR Operation** — A+B = 1 when A=1 OR B=1

| A | B | A+B |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

**NOT Operation** — ¬A = 1 when A=0

| A | ¬A |
|---|---|
| 0 | 1 |
| 1 | 0 |

### Basic Rules
| Rule | Expression |
|---|---|
| 1 | A + 0 = A |
| 2 | A + 1 = 1 |
| 3 | A·0 = 0 |
| 4 | A·1 = A |
| 5 | A + A = A |
| 6 | A + ¬A = 1 |
| 7 | A·A = A |
| 8 | A·¬A = 0 |
| 9 | ¬(¬A) = A |
| 10 | A + AB = A |

### Principle of Duality
- Swap 0↔1 and +↔· in any true statement
- The dual statement is also true

### DeMorgan's Theorems
```
¬(A + B) = ¬A · ¬B
¬(A·B) = ¬A + ¬B
```

### Boolean Expressions

**Sum-of-Products (SOP)**
```
F(A,B,C) = ABC + ¬BC + ¬AB
```
- Product terms are called minterms
- Canonical SOP: Each term contains all variables

**Product-of-Sums (POS)**
```
F(A,B,C) = (A+B)(¬B+C)(A+¬C)
```
- Sum terms are called maxterms
- Canonical POS: Each term contains all variables

### Venn Diagrams
- Used to illustrate Boolean operations
- Each circle represents a Boolean variable
- Overlapped areas represent AND operation
- Combined areas represent OR operation

### Practice Questions

**Fill in the Blanks**
1. Boolean algebra was developed by ______.
2. The AND operation is also called ______.
3. DeMorgan's theorem: ¬(A+B) = ______.
4. SOP stands for ______.
5. The principle of duality swaps ______ and ______.

**Multiple Choice Questions**
1. Which is the identity element for OR operation?
   A) 0 B) 1 C) A D) ¬A
2. The output of A + ¬A is:
   A) 0 B) 1 C) A D) ¬A
3. Which expression represents DeMorgan's law?
   A) ¬(A+B) = ¬A + ¬B B) ¬(A·B) = ¬A · ¬B C) ¬(A+B) = ¬A · ¬B D) ¬(A·B) = ¬A + B

**Discussion Questions**
- Explain the basic Boolean operations with truth tables.
- State and prove DeMorgan's theorems.
- What is the principle of duality?
- Differentiate between SOP and POS forms.

---

## 8. LOGIC GATES AND DIGITAL CIRCUITS

### Basic Logic Gates
| Gate | Expression | Truth Table |
|---|---|---|
| AND | Y = A·B | 1 only when A=1,B=1 |
| OR | Y = A+B | 0 only when A=0,B=0 |
| NOT | Y = ¬A | Inverts input |

### Derived Logic Gates
| Gate | Expression | Output |
|---|---|---|
| NAND | Y = ¬(A·B) | 0 when both inputs are 1 |
| NOR | Y = ¬(A+B) | 1 when both inputs are 0 |
| XOR | Y = A⊕B | 1 when inputs are different |
| XNOR | Y = ¬(A⊕B) | 1 when inputs are same |

### Logic Families
| Family | Components |
|---|---|
| DL (Diode Logic) | Diodes, Resistors |
| DTL (Diode-Transistor Logic) | Diodes, Transistors, Resistors |
| TTL (Transistor-Transistor Logic) | Transistors |

### K-Map (Karnaugh Map)
- Graphical method to simplify Boolean expressions
- Groups of 2, 4, or 8 adjacent 1s
- Each group eliminates changing variables

### Adder Circuits

**Half Adder**
- Adds 2 bits
- Sum = XOR(A,B)
- Carry = AND(A,B)

| A | B | Sum | Carry |
|---|---|---|---|
| 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 0 | 1 | 0 |
| 1 | 1 | 0 | 1 |

**Full Adder**
- Adds 3 bits
- Uses two half adders and an OR gate

**4-Bit Adder**
- Four full adders cascaded
- Performs addition of two 4-bit numbers

### Flip-Flops
| Type | Description | Characteristic |
|---|---|---|
| SR | Set-Reset | Undefined for S=R=1 |
| D | Data/ Delay | Q = D |
| JK | Improved SR | Toggles for J=K=1 |
| T | Toggle | Toggles when T=1 |

### Applications of Flip-Flops

**Counters**
- Up Counter: Counts ascending
- Down Counter: Counts descending
- Synchronous: All flip-flops get clock simultaneously
- Asynchronous (Ripple): Each gets clock from previous

**Registers**
- Group of flip-flops for storing binary data
- Each flip-flop stores 1 bit
- Uses D-type flip-flops

### Practice Questions

**Fill in the Blanks**
1. The output of NAND gate is ______ only when both inputs are 1.
2. A ______ adds two binary numbers.
3. A ______ adds three binary numbers.
4. ______ is a sequential electronic circuit.
5. A register uses ______ type flip-flop.

**Multiple Choice Questions**
1. Which is a basic logic gate?
   A) NAND B) NOR C) XOR D) AND
2. The output of XOR gate is 1 when:
   A) Both inputs are 0 B) Both inputs are 1 C) Inputs are different D) Inputs are same
3. Which flip-flop eliminates the race condition?
   A) SR B) D C) JK D) T

**Discussion Questions**
- Explain the working of a half adder and full adder.
- Describe the different types of flip-flops.
- What is the difference between synchronous and asynchronous counters?
- Explain K-map simplification with an example.

---

## 9. COMPUTER SOFTWARE

### System Software

**System Management Programs**

| Program | Function |
|---|---|
| Operating System | Manages resources, user interface |
| Utility Programs | Disk defragmenter, virus scanner, backup |
| Device Drivers | Translates between OS and hardware |

**System Development Programs**

| Program | Function |
|---|---|
| Language Translators | Compiler, Interpreter, Assembler |
| Linkers | Combines object modules |
| Debuggers | Finds errors in programs |
| Editors | Text, audio, graphics editing |

### Application Software

**Standard Applications**

| Type | Purpose | Example |
|---|---|---|
| Word Processor | Document creation | MS Word |
| Spreadsheet | Calculations, data | MS Excel |
| DBMS | Database management | MS Access, MySQL |
| DTP | Publishing | MS Publisher |
| Web Browser | Internet access | Chrome, Firefox |

**Unique Applications**
- Inventory Management System
- Pay-roll System
- Examination Results Processing
- Airline Reservation Systems

### Data Models in DBMS
| Model | Structure | Example |
|---|---|---|
| Hierarchical | Tree structure | IMS |
| Network | Graph structure | IDMS |
| Relational | Tables | Oracle, MySQL |

### Database Properties (ACID)
| Property | Description |
|---|---|
| Atomicity | Transaction completes fully or not at all |
| Consistency | Database maintains consistency |
| Isolation | Transactions don't interfere |
| Durability | Committed changes are permanent |

### Problem Solving Tools
| Tool | Purpose |
|---|---|
| Hierarchy Chart | Shows top-down structure |
| Algorithm | Step-by-step solution |
| Flowchart | Pictorial representation |
| Pseudocode | Logic description |

### Flowchart Symbols
| Symbol | Shape | Purpose |
|---|---|---|
| Start/End | Oval | Program start/end |
| Input/Output | Parallelogram | Data I/O |
| Process | Rectangle | Calculations |
| Decision | Diamond | Conditions |
| Flow Lines | Arrows | Direction of flow |

### Control Structures
| Structure | Description |
|---|---|
| Sequence | Statements executed in order |
| Selection | If-Then-Else, Case |
| Repetition | Do-While, Repeat-Until |

### Practice Questions

**Fill in the Blanks**
1. Software is classified into ______ and ______.
2. ______ manages the allocation of devices and resources.
3. A device driver acts as a translator between ______ and ______.
4. ______ converts high-level language to low-level language.
5. ______ is a pictorial representation of a process.

**Multiple Choice Questions**
1. Which is not a system software?
   A) Operating System B) Compiler C) MS Word D) Device Driver
2. A device driver acts as interface between:
   A) User and hardware B) OS and hardware C) Application and OS D) User and OS
3. Which is used for document creation?
   A) Spreadsheet B) Word Processor C) DBMS D) DTP

**Discussion Questions**
- Explain the different types of computer software.
- What are the functions of an operating system?
- Describe the components of DBMS.
- Explain the problem-solving process.

---

## 10. OPERATING SYSTEMS

### Process Management

**Process States**
```
New → Ready → Running → Terminated
         ↓          ↓
      Waiting    Blocked
         ↓
      Suspended
```

**Process Control Block (PCB) Contents**
- Process ID
- Process State
- Program Counter
- Register Information
- Scheduling Information
- Memory Information
- I/O Status

**Scheduling Algorithms**
| Algorithm | Description |
|---|---|
| FCFS | First Come First Served |
| SJF | Shortest Job First |
| Priority | Highest priority first |
| Round Robin | Time quantum allocation |

### Memory Management
| Technique | Description |
|---|---|
| Segmentation | Memory divided into variable-sized segments |
| Paging | Memory divided into equal-sized pages |
| Swapping | Moving processes between main and secondary memory |

### File Management

**File Attributes**
- Name, Type, Location, Size
- Date/Time created/modified/accessed
- Read-only, Hidden, Archive

**File Operations**
- Create, Save, Open, Close
- Modify, Rename, Delete

**File Systems**
| System | Characteristics |
|---|---|
| FAT (File Allocation Table) | Simple, for smaller disks |
| NTFS (New Technology) | Robust, for larger disks |

### Types of Operating Systems
| Type | Description | Examples |
|---|---|---|
| Batch Processing | Jobs processed in batches | Early OS |
| Multi-user | Multiple users simultaneously | Unix, Linux |
| Multitasking | Multiple tasks simultaneously | Windows, Unix |
| Real-time | Time-critical applications | MTOS, Lynx |
| Multiprocessor | Multiple CPUs | Windows, Unix |
| Embedded | Dedicated devices | Palm OS, Windows CE |

### User Interfaces
| Interface | Method | Pros | Cons |
|---|---|---|---|
| GUI | Point-and-click | User-friendly | Resource-intensive |
| CLI | Command typing | Efficient, powerful | Steep learning curve |

### Popular Operating Systems

**MS-DOS (1981)**
- Single-user, single-tasking
- Command line interface
- Key files: IO.SYS, MSDOS.SYS, CONFIG.SYS, COMMAND.COM, AUTOEXEC.BAT

**UNIX**
- Multi-user, multitasking
- Components: Kernel, Shell, Files/Processes
- Hierarchical directory structure (root: /)

**Windows**
- GUI-based
- Various versions: 95, 98, 2000, ME, XP, Vista

### Practice Questions

**Fill in the Blanks**
1. ______ manages the processes in a computer system.
2. PCB stands for ______.
3. ______ scheduling allocates a fixed time quantum to each process.
4. ______ is the central part of UNIX.
5. MS-DOS provides a ______ interface.

**Multiple Choice Questions**
1. Which is a function of OS?
   A) Process Management B) Memory Management C) File Management D) All of these
2. Which OS is multi-user?
   A) MS-DOS B) Windows 95 C) Unix D) All of these
3. Which is the simplest scheduling algorithm?
   A) FCFS B) SJF C) Priority D) Round Robin

**Discussion Questions**
- Explain the various functions of an operating system.
- Describe the process states with a diagram.
- Explain the different types of scheduling algorithms.
- Differentiate between GUI and CLI.

---

## 11. PROGRAMMING LANGUAGES

### History of Programming Languages
| Period | Language | Characteristics |
|---|---|---|
| 1843 | Analytical Engine | First program by Ada Lovelace |
| 1940s | Machine Language | Binary code, machine-dependent |
| 1950s | Assembly Language | Mnemonics, machine-dependent |
| 1957 | FORTRAN | High-level, scientific |
| 1958 | LISP | Functional, AI |
| 1959 | COBOL | Business-oriented |
| 1964 | BASIC | General-purpose, simple |
| 1970 | PASCAL | Procedural, structured |
| 1972 | C | System software, powerful |
| 1979 | C++ | OOP, enhanced C |
| 1995 | Java | Web, platform-independent |

### Generations of Languages
| Generation | Type | Examples | Features |
|---|---|---|---|
| 1GL | Machine Language | Binary code | Machine-dependent, fast |
| 2GL | Assembly Language | Mnemonics | Machine-dependent |
| 3GL | High-Level Language | FORTRAN, C, COBOL | Machine-independent, easier |
| 4GL | Very High-Level | SQL, PowerBuilder | Database-oriented |
| 5GL | AI Languages | Prolog, Mercury | Constraint programming |

### Language Translators
| Translator | Process | Output |
|---|---|---|
| Compiler | Translates entire program | Machine code |
| Interpreter | Translates line by line | Machine code |
| Assembler | Translates assembly | Machine code |

### Programming Paradigms
| Paradigm | Approach | Languages |
|---|---|---|
| Procedural | Step-by-step procedures | FORTRAN, C, BASIC |
| Logic-oriented | Rules and facts | Prolog |
| Object-oriented | Objects and messages | C++, Java, C# |

### Characteristics of a Good Programming Language
- Simple, clear, concise
- Well-documented function library
- Efficient use of memory/resources
- Integrated Development Environment (IDE)
- Platform independent
- Object-oriented features
- Consistent syntax and semantics

### Practice Questions

**Fill in the Blanks**
1. ______ is considered the first computer programmer.
2. A ______ translates assembly language to machine code.
3. ______ uses 0s and 1s only.
4. The term "opcode" means ______.
5. ______ is developed by Sun Microsystems.

**Multiple Choice Questions**
1. Which is a low-level language?
   A) C B) Java C) Assembly D) FORTRAN
2. A compiler translates:
   A) Machine to assembly B) Assembly to machine C) High-level to machine D) Machine to high-level
3. Who developed C language?
   A) Bjarne Stroustrup B) Dennis Ritchie C) James Gosling D) John Backus

**Discussion Questions**
- Explain the different generations of programming languages.
- What are language translators? Explain compiler and interpreter.
- Describe the program development process.
- Differentiate between procedural and object-oriented programming.

---

## 12. DATA COMMUNICATIONS AND NETWORKS

### Modem
- **Modulator:** Converts digital to analog
- **Demodulator:** Converts analog to digital
- **Internal:** Inside computer
- **External:** Connected to COM port

### Types of Networks
| Type | Area Covered | Speed | Example |
|---|---|---|---|
| LAN | Building/Campus | High | Office network |
| MAN | City | Moderate | Cable TV |
| WAN | Country/Continent | Low | Internet |
| Internet | Global | Variable | Worldwide web |

### Network Architectures
| Architecture | Description | Advantages | Disadvantages |
|---|---|---|---|
| Client-Server | Centralized server | Secure, manageable | Single point of failure |
| Peer-to-Peer | Decentralized | Simple, cheap | Less secure |
| VAN | Value-added services | Extra features | Costly |

### Network Topologies
| Topology | Pros | Cons |
|---|---|---|
| Bus | Less cabling, simple | Single point of failure |
| Star | Easy error detection | Hub failure affects all |
| Ring | Equal access | One failure affects all |
| Mesh | Reliable, multiple paths | Very expensive |
| Tree | Hierarchical organization | Root failure affects all |

### Network Media
| Medium | Type | Use |
|---|---|---|
| Twisted Pair | Wired | LAN |
| Coaxial | Wired | Long distances |
| Optical Fibre | Wired | High speed, secure |
| Microwave | Wireless | Line-of-sight |
| Satellite | Wireless | Global |

### Network Protocols
| Protocol | Full Form | Purpose |
|---|---|---|
| HTTP | Hypertext Transfer Protocol | Web browsing |
| FTP | File Transfer Protocol | File transfer |
| SMTP | Simple Mail Transfer Protocol | Email |
| TCP/IP | Transmission Control/Internet Protocol | Internet communication |
| DNS | Domain Name System | Converts domain to IP |

### Applications of Networks
| Application | Description |
|---|---|
| Data Sharing | Access shared data |
| Resource Sharing | Share printers, storage |
| Personal Communication | Email, video conferencing |
| Remote Access | Access from remote locations |

### Practice Questions

**Fill in the Blanks**
1. ______ converts digital to analog.
2. LAN covers a ______ area.
3. In ______ topology, all nodes connect to a central hub.
4. HTTP stands for ______.
5. ______ translates domain names to IP addresses.

**Multiple Choice Questions**
1. Which network covers a building?
   A) WAN B) MAN C) LAN D) Internet
2. In star topology, the central device is called:
   A) Hub B) Repeater C) Bridge D) Router
3. Which is not a network protocol?
   A) HTTP B) FTP C) NMP D) TCP/IP

**Discussion Questions**
- Explain the different types of network topologies.
- What is the difference between LAN, MAN, and WAN?
- Describe the client-server and peer-to-peer architectures.
- Explain the functions of various network protocols.

---

## 13. INTERNET AND WORLD WIDE WEB

### Internet History Timeline
| Year | Event |
|---|---|
| 1969 | ARPAnet established |
| 1972 | ARPAnet opened to public |
| 1974 | TCP/IP developed |
| 1979 | Usenet created |
| 1982 | Eunet in Europe |
| 1983 | TCP/IP becomes standard |
| 1984 | DNS introduced |
| 1987 | NSFNET established |
| 1990 | Archie (FTP search) |
| 1991 | Gopher and Veronica |
| 1992 | World Wide Web |

### Internet Services
| Service | Description |
|---|---|
| Email | Electronic mail |
| Online Chat | Real-time text communication |
| Online Shopping | E-commerce |
| Usenet | Newsgroups |
| WWW | World Wide Web |

### E-Business Categories
| Category | Description | Example |
|---|---|---|
| B2B | Business to Business | Supplier to manufacturer |
| B2C | Business to Consumer | Online retail |
| C2C | Consumer to Consumer | eBay |
| C2B | Consumer to Business | Google Adsense |

### Web Browsers
| Browser | Year | Features |
|---|---|---|
| Internet Explorer | 1995 | SSL, Windows integration |
| Netscape Navigator | 1990s | Early popular browser |
| Mozilla Firefox | 2004 | Open source, extensible |

### Search Engine Tips
- **Double Quotes:** Search exact phrase — Example: "types of computers"
- **Boolean Operators:** AND, OR, NOT — Example: "track ball OR touch ball"
- **Plus (+):** All words must be present — Example: "features + mouse"
- **Minus (-):** Exclude words

### Email
```
Email Address Format: username@domain.com
Example: shruti_garg@yahoo.com
```

| Field | Purpose |
|---|---|
| To | Primary recipient |
| CC | Carbon Copy recipients |
| Subject | Email topic |
| Body | Message content |

### Internet Protocols

**TCP/IP Model**

| Layer | Protocols |
|---|---|
| Application | HTTP, FTP, SMTP, DNS |
| Transport | TCP, UDP |
| Internet | IP, ICMP, ARP |
| Physical | RS-232C, V.35, IEEE 802.3 |

**OSI Model (7 Layers)**

| Layer | Function |
|---|---|
| 7. Application | User interface |
| 6. Presentation | Data formatting, encryption |
| 5. Session | Session management |
| 4. Transport | End-to-end delivery |
| 3. Network | Routing |
| 2. Data Link | Error detection/correction |
| 1. Physical | Hardware transmission |

### Practice Questions

**Fill in the Blanks**
1. ARPAnet was developed in ______.
2. DNS stands for ______.
3. ______ is the global network of networks.
4. The first protocol used on ARPAnet was ______.
5. ______ converts domain names to IP addresses.

**Multiple Choice Questions**
1. When was ARPAnet developed?
   A) 1945 B) 1967 C) 1969 D) 1974
2. Which e-business category does eBay belong to?
   A) B2B B) B2C C) C2C D) C2B
3. How many layers are in the OSI model?
   A) 4 B) 5 C) 7 D) 8

**Discussion Questions**
- Trace the history of the Internet.
- Explain the different applications of the Internet.
- What are the layers of TCP/IP and OSI models?
- Describe the e-business categories with examples.

---

## Key Terms Quick Reference 📝

| Term | Definition |
|---|---|
| CPU | Brain of the computer, processes instructions |
| RAM | Volatile memory, read/write |
| ROM | Non-volatile memory, read-only |
| Bit | Smallest unit of information (0/1) |
| Byte | 8 bits, smallest addressable unit |
| LAN | Local Area Network |
| WAN | Wide Area Network |
| OS | Operating System |
| GUI | Graphical User Interface |
| CLI | Command Line Interface |
| SOP | Sum of Products (Boolean) |
| POS | Product of Sums (Boolean) |
| PCB | Process Control Block |
| IPC | Interprocess Communication |
| FAT | File Allocation Table |
| NTFS | New Technology File System |
| DNS | Domain Name System |
| TCP/IP | Transmission Control Protocol/Internet Protocol |
| HTTP | Hypertext Transfer Protocol |
| FTP | File Transfer Protocol |
| SMTP | Simple Mail Transfer Protocol |
| URL | Uniform Resource Locator |
| HTML | Hypertext Markup Language |
| WWW | World Wide Web |

---

## Exam Tips 💡

**Remember These Key Points**
- Generations of Computers: Vacuum tubes → Transistors → ICs → Microprocessors → ULSI
- Memory Types:
  - Primary (RAM, ROM) - Volatile/Non-volatile
  - Secondary (Magnetic, Optical, Solid State)
- Boolean Algebra: AND (·), OR (+), NOT (¬)
- Number Systems: Binary (2), Octal (8), Decimal (10), Hexadecimal (16)
- OS Functions: Process, Memory, File, Device, Security Management
- Network Topologies: Bus, Star, Ring, Mesh, Tree, Hybrid
- Internet History: ARPAnet (1969) → TCP/IP (1974) → DNS (1984) → WWW (1992)
- Programming: Machine → Assembly → High-level → Very High-level → AI

**Common Formulas**
- Binary to Decimal: Sum of (bit × 2^position)
- Decimal to Binary: Repeated division by 2
- Number of links in Mesh: n(n-1)/2
- Cache hit: Data found in cache

---

## Practice Questions Summary ✅

**Self-Assessment Checklist**
- [ ] Can you explain the characteristics of a computer?
- [ ] Can you describe the five generations of computers?
- [ ] Can you differentiate between analog, digital, and hybrid computers?
- [ ] Can you explain the CPU cycle?
- [ ] Can you differentiate between SRAM and DRAM?
- [ ] Can you explain the different types of ROM?
- [ ] Can you list and describe various input/output devices?
- [ ] Can you perform number system conversions?
- [ ] Can you simplify Boolean expressions?
- [ ] Can you explain logic gates and their truth tables?
- [ ] Can you differentiate between system and application software?
- [ ] Can you describe the functions of an operating system?
- [ ] Can you explain the generations of programming languages?
- [ ] Can you describe network topologies?
- [ ] Can you explain the history and services of the Internet?

**Good luck with your exam! 🎓**
