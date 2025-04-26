#  T3RRA   
### _Android Triage Rapid Retrieval Analysis_

---

##  What is T3RRA?

**T3RRA** is a battle-tested Android triage tool for forensic professionals, cyber operators, and those who **don't have time to play nice**.  
It connects, extracts, and packages Android data at **warp speed** — designed for real-world field ops, triage missions, and on-the-spot investigations.

You want data?  
T3RRA **pulls it straight from the guts of the device** — **Bluetooth**, **Wi-Fi configs**, **Location history**, **App data**, **Photos**, **SMS databases**, and much more.

It even **fakes a UFED extraction** by generating `.ufdx` packages recognizable by Cellebrite.  


---

## ⚙️ Features

-  **Lightning-fast Android acquisition** (rootless, ADB mode)
-  **Extracts**:
  - Device Info (IMEI, Model, Android Version)
  - Bluetooth & Wi-Fi configs
  - Geolocation dumps
  - Browser data
  - Media (Photos, Videos, Music, Movies)
  - SMS databases
  - Messaging apps installed (WhatsApp, Telegram, Signal, etc.)
-  **Manual App Selection** (Pick what you want to extract!)
-  **Pre-Built Profiles** for rapid one-click extraction
-  **Dark-themed GUI** (because light mode is for cowards)
-  **UFD.xml generation** for fake UFED compatibility
-  **Automatic UFDX package creation** (`*.ufdx`) – Cellebrite will eat it up!
-  **Ready for ALEAPP parsing** if needed.
-  **Built with Python 3.8+**, tkinter, and raw **command-line ADB**.

---

##  How it Works

1.  Connect Android device via USB
2.  Enable _Developer Options_ and _USB Debugging_ on the phone
3.  Launch **T3RRA**
4.  Detect device, select acquisition method
5.  Sit back while T3RRA rips the data out
6.  Find your results + `.ufdx` archive ready for Cellebrite or analysis

---

##  Requirements

- Python 3.8+
- `adb` must be installed and in PATH
- `Pillow` Python library (`pip install pillow`)

Optional:
- ALEAPP (to parse app data later)
- Cellebrite Physical Analyzer (to load `.ufdx`)

---



> "When the mission clock is ticking and there's no second chance...  
> You don't **hope** for data.  
> You **TAKE** it."

---

##  How to Run

```bash
python3 t3rra.py
