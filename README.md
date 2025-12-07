# NFC Hacker Card 💳⚡

A custom NFC-enabled business card PCB featuring a sleek design with an embedded NFC chip, LED indicator, and unique lightbulb artwork.

## ✨ Features

- **NFC Technology**: NT3H2111W0FHKH chip for seamless contactless data sharing
- **Visual Feedback**: Yellow LED indicator for successful NFC interactions
- **Unique Design**: Custom lightbulb silkscreen artwork on black PCB
- **Compact Size**: Business card dimensions (88.9mm × 50.8mm)
- **Premium Finish**: Black solder mask with white silkscreen

## 📋 Bill of Materials (BOM)

| Designator | Component | Package | Value | LCSC Part # | Manufacturer Part # | Qty |
|------------|-----------|---------|-------|-------------|---------------------|-----|
| **C1** | Capacitor | 0603 | 220nF | C21120 | CL10B224KA8NNNC | 1 |
| **LED1** | LED (Yellow) | 0805 | - | C2296 | KT-0805Y | 1 |
| **R1** | Resistor | 0603 | 47Ω | C23182 | 0603WAF470JT5E | 1 |
| **U1** | NFC Chip | XQFN-8 | 13.56MHz | C710403 | NT3H2111W0FHKH | 1 |
| **U2** | NFC Antenna | PCB Trace | 25×48mm | - | (Integrated) | 1 |

### Component Details

#### U1 - NFC Chip (NT3H2111W0FHKH)
- **Frequency**: 13.56 MHz (ISO 14443 Type A)
- **Memory**: 106Kbit/s I2C interface
- **Package**: XQFN-8 (1.6mm × 1.6mm)
- **Manufacturer**: NXP Semiconductors
- **Features**: Energy harvesting, I2C interface, field detection

#### U2 - NFC Antenna
- **Type**: PCB coil antenna (copper traces)
- **Dimensions**: 25mm × 48mm
- **No external component required** - integrated into PCB design

**Shaurya Gupta**  
🌐 shauryag.com  

