# 📱 CLI QR Code Generator

> *Generate QR codes instantly from the command line! Simple, fast, and effective.*

## 🌟 Highlights

- **Simple CLI interface** - Just run and enter your URL
- **Instant generation** - Creates QR codes in seconds ⚡
- **PNG output** - Saves as a standard image file
- **Minimal dependencies** - Only requires the qrcode library
- **Pure Python** - Clean, readable code with standard library

## ℹ️ Overview

**CLI QR Code Generator** is a straightforward command-line tool that generates QR codes from any URL or text input. Built with Python and the qrcode library, it provides a quick way to create scannable QR codes without needing online generators or complex software.

Perfect for developers, marketers, or anyone who needs to generate QR codes quickly and locally.

### ✍️ Author

Built by **SwagBoy3000** ([@SwagBoy3000](https://github.com/SwagBoy3000)), a CS student at USTHB. This project demonstrates clean Python scripting and practical CLI tool development.

## 🚀 Quick Start

```bash
# Run the generator
python main.py

# Enter your URL when prompted
Enter the URL: https://github.com/SwagBoy3000

# QR code saved as QR.png!
QR code generated!!
```

## ⬇️ Installation

### Requirements
- Python 3.8 or higher
- `qrcode` library with PIL support

### Quick Install
```bash
# Clone the repository
git clone https://github.com/SwagBoy3000/CLI_QRgen.git
cd CLI_QRgen

# Install dependencies
pip install qrcode[pil]

# Run the generator
python main.py
```

## ✨ Features

- 📱 **URL to QR** - Convert any URL into a scannable QR code
- 💾 **PNG Export** - Automatically saves as QR.png
- 🎯 **Simple Interface** - Just input and generate
- ⚡ **Fast Generation** - Creates codes in milliseconds
- 🔧 **Extensible** - Easy to modify for custom use cases

## 🛠️ Usage

### Basic Usage
```bash
python main.py
```

### Example Session
```
Enter the URL: https://swagboy3000.github.io
QR code generated!!
```

The QR code will be saved as `QR.png` in the current directory.

### Use Cases
- Share website links
- Create event check-in codes
- Generate WiFi connection QR codes
- Product URLs for marketing
- Contact information sharing

## 🧩 How It Works

```python
import qrcode

# Get user input
url = input("Enter the URL").strip()

# Create QR code object
qr = qrcode.QRCode()
qr.add_data(url)

# Generate and save image
img = qr.make_image()
img.save("QR.png")
```

Simple, effective, and easy to understand!

## 🔧 Built With

- **Python 3** - Core language
- **qrcode** - QR code generation library
- **PIL (Pillow)** - Image processing

## 📈 Future Enhancements

- [ ] Custom output filename option
- [ ] QR code size customization
- [ ] Color customization (foreground/background)
- [ ] Batch generation from file
- [ ] Error correction level options
- [ ] Add logo/image in center of QR code
- [ ] Support for vCard, WiFi, and other formats

## 💭 Contributing

Found a bug or have a feature idea? Open an [issue](https://github.com/SwagBoy3000/CLI_QRgen/issues) or submit a pull request!

---

**Built with 💜 by SwagBoy3000**