# NFC Hacker Card 💳⚡

A custom NFC-enabled business card PCB featuring a sleek design with an embedded NFC chip, LED indicator, and unique lightbulb artwork.

![Black PCB Design](https://img.shields.io/badge/PCB-Black-000000?style=flat-square)
![NFC](https://img.shields.io/badge/NFC-13.56MHz-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-success?style=flat-square)

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

## 🛠️ Assembly Options

### Option 1: JLCPCB Assembly Service (Recommended)
- **Difficulty**: None (fully assembled)
- **Cost**: ~$15-30 for 2-5 boards with assembly
- **Time**: 5-7 days
- **Pros**: Professional assembly, tested, ready to use

### Option 2: DIY Hand Assembly
- **Difficulty**: ⚠️ **Advanced** (SMD soldering required)
- **Cost**: ~$3-10 (PCB + components)
- **Time**: 1-2 hours per board
- **Required Skills**: 
  - Experience with 0603/0805 SMD components
  - Hot air station or reflow oven recommended
  - Magnification/microscope highly recommended

#### DIY Assembly Requirements:
- Soldering iron with fine tip (temperature controlled)
- Hot air station or reflow oven
- Tweezers (ESD-safe, fine point)
- Flux paste
- Solder paste (recommended) or fine solder wire
- Magnifying glass or microscope
- Steady hands!

## 🛒 Where to Buy Components

### Primary Source: LCSC.com (Recommended)
```
C1:   LCSC Part C21120  (220nF capacitor)
LED1: LCSC Part C2296   (Yellow LED)
R1:   LCSC Part C23182  (47Ω resistor)  
U1:   LCSC Part C710403 (NFC chip)
```
**Advantages**: Cheap, same warehouse as JLCPCB, exact part numbers

### Alternative Sources:
- **Mouser**: Search by manufacturer part numbers
- **DigiKey**: Excellent for North America
- **AliExpress**: Budget option (2-4 week shipping)

## 📐 PCB Specifications

- **Dimensions**: 88.9mm × 50.8mm (2 layer)
- **Thickness**: 1.6mm
- **Color**: Black solder mask
- **Silkscreen**: White
- **Finish**: HASL (with lead) or LeadFree HASL
- **Min Track/Space**: Standard 6mil/6mil

## 🚀 Ordering Instructions

### Ordering PCBs Only (DIY Assembly)

1. **Download Gerber files**: `Gerber_PCB_2025-12-07.zip`
2. **Upload to JLCPCB**: https://jlcpcb.com/
3. **Settings**:
   - PCB Qty: 5 (minimum)
   - PCB Color: **Black**
   - Silkscreen: **White**  
   - PCB Thickness: 1.6mm
   - Surface Finish: HASL
4. **Cost**: ~$3-5 for 5 PCBs + shipping

### Ordering with Assembly

1. Upload Gerber files to JLCPCB
2. Enable **PCB Assembly** toggle
3. Select:
   - PCBA Type: **Economic**
   - Assembly Side: **Top Side**
   - PCBA Qty: 2 (minimum)
   - Tooling holes: **Added by JLCPCB**
4. Upload BOM: `BOM_Board1_PCB_2025-12-07.xlsx`
5. Upload CPL (Component Placement) file if required
6. Review and confirm
7. **Cost**: ~$15-30 total (PCB + assembly + components)

## 💡 Programming the NFC Chip

### Required:
- NFC-enabled smartphone (Android/iPhone)
- NFC Tools app (iOS/Android) or similar

### Steps:
1. Power the card (tap to NFC-enabled phone or use external power)
2. Open NFC Tools app
3. Select "Write"
4. Add records:
   - URL (website, social media)
   - vCard (contact info)
   - Text
   - Custom data
5. Tap card to phone to write data

### Use Cases:
- Business card with instant contact sharing
- Portfolio website link
- Social media profiles
- WiFi credentials
- Custom hacker/demo projects

## ⚡ Power Options

The NFC chip harvests power from the NFC reader (phone), so:
- **No battery required!**
- LED lights up when powered by NFC field
- Works with any NFC-enabled smartphone

## 🔧 Troubleshooting

### LED doesn't light up:
- Check R1 and LED1 orientation (polarity)
- Verify R1 resistance (47Ω)
- Check solder joints on U1 NFC chip

### NFC not detected:
- Ensure U2 antenna traces are not damaged
- Check U1 chip orientation and soldering
- Test with multiple NFC devices
- Verify C1 capacitor is properly soldered

### Read range is poor:
- Check antenna coil continuity
- Ensure no shorts on antenna traces
- Capacitor C1 must be correct value (220nF)

## 📁 Files in This Repository

- `BOM_Board1_PCB_2025-12-07.xlsx` - Bill of Materials for ordering
- `Gerber_PCB_2025-12-07.zip` - PCB manufacturing files
- `JOURNAL.md` - Project development notes
- `README.md` - This file

## 🎨 Design Notes

- Artwork features a minimalist lightbulb design representing innovation
- White silkscreen on black creates high contrast
- NFC tap icon indicates where to tap phones
- Antenna coil is visible on the PCB as decorative element

## 📄 License

Open source hardware - feel free to modify and use for your projects!

## 🤝 Contributing

Pull requests welcome! Ideas for improvements:
- Add RGB LED support
- Alternative antenna designs
- Different form factors
- Enhanced power harvesting

## 👤 Author

**Shaurya Gupta**  
🌐 shauryag.com  

---

**Happy Hacking! 🚀💻**
