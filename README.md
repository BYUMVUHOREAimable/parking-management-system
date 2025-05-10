# Smart Parking Management System

A comprehensive parking management solution that combines RFID technology, license plate recognition, and automated payment processing.

## 🚀 Features

- **RFID-based Vehicle Identification**
  - Secure vehicle tracking using RFID cards
  - Automatic balance management
  - Real-time payment processing

- **License Plate Recognition**
  - Automated plate detection and reading
  - Integration with RFID system
  - Support for multiple vehicle types

- **Payment Processing**
  - Automated fee calculation
  - Real-time balance updates
  - Secure transaction handling

## 🛠️ Hardware Requirements

- Arduino Uno/Nano
- MFRC522 RFID Reader
- Webcam for license plate detection
- LED indicators
- Buzzer for alerts

## 💻 Software Requirements

- Python 3.8+
- Arduino IDE
- Required Python packages (see requirements.txt)
- Required Arduino libraries:
  - MFRC522
  - SPI

## 📁 Project Structure

```
parking-management-system/
├── hardware/
│   ├── payment/
│   │   └── process_payment.ino    # Payment processing on Arduino
│   ├── writing_on_rfid/
│   │   └── top_up.ino            # RFID card initialization
│   └── process_payment.py         # PC-side payment logic
├── model/
│   ├── dataset/                   # Training data
│   ├── scripts/                   # Model training scripts
│   └── runs/                      # Training logs
└── hardware/
    ├── car_entry.py              # Entry management
    ├── car_exit.py               # Exit management
    └── webcam_detect.py          # License plate detection
```

## 🚀 Getting Started

1. **Hardware Setup**
   - Connect RFID reader to Arduino
   - Connect webcam to PC
   - Power up the system

2. **Software Setup**
   ```bash
   # Install Python dependencies
   pip install -r requirements.txt
   
   # Upload Arduino code
   # Open Arduino IDE and upload process_payment.ino and top_up.ino
   ```

3. **System Initialization**
   - Run the main system:
   ```bash
   python hardware/main.py
   ```

## 🔄 Workflow

1. **Vehicle Entry**
   - License plate is captured and recognized
   - RFID card is initialized with plate number and balance
   - Entry time is recorded

2. **Vehicle Exit**
   - License plate is verified
   - RFID card is read
   - Parking fee is calculated
   - Balance is updated
   - Exit is processed

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- Your Name - Initial work

## 🙏 Acknowledgments

- Thanks to all contributors
- Inspired by modern parking management needs 