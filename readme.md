<p align="center">
  <img src="https://github.com/FNBUBBLES420-ORG/Assistive-AimGuide/blob/main/banner/Assitive-AimGuide.png" alt="Assistive-AimGuide" width="350">
</p>

<p align="center">
  <img src="https://github.com/FNBUBBLES420-ORG/Assistive-AimGuide/blob/main/banner/fnbubbles420.png" alt="Fnbubbles420 Logo" width="80" align="left">
  <img src="https://github.com/FNBUBBLES420-ORG/Assistive-AimGuide/blob/main/banner/fnbubbles420.png" alt="Fnbubbles420 Logo" width="80" align="right">
  <br><br><br>
  <h1 align="center">FNBubbles420 Org - Assistive Aim-Guide</h1>
</p>



# 🎯 Assistive AimGuide Configuration GUI - AMD GPU

A sleek, user-friendly configuration tool built with `Tkinter` for customizing and launching the Assistive AimGuide, designed to help disabled gamers and streamers optimize their aim-assist tool powered by AI models. Perfect for users with physical or cognitive challenges who need support while gaming.

> 💙 Built with accessibility in mind by the FNBUBBLES420 Organization.

---

## 📦 Features

- Dynamic GUI to update and reload configurations
- Visual toggles for features like masking, visuals, and headshot targeting
- Optimized support for ONNX models on AMD/Intel GPUs via DirectML
- Live launching of the assistive detection tool
- Full support for `DirectML` and device targeting

---

## 🐍 Install Python 3.11.9 Without Admin Access (Super Easy!)

1. In the extracted folder, **look for** the file:  

```
python3119.bat
```

2. **Double-click** this `.bat` file.
3. It will automatically:
- Download Python 3.11.9
- Install it locally (no admin required)
- Add it to your PATH
- Close when complete

> 💡 Now you’re ready to install packages and run the app — without needing admin access!

## 🛠️ Requirements

Ensure you have the following installed before running the GUI:

```bash
pip install -r requirements.txt
```

### **Sample dependencies include**:

- `torch`, `torchvision`, `torchaudio`
- `onnx`, `onnxruntime-directml`, `pyautogui`, `pywin32`
- `tkinter` (usually comes with Python)

Your model placed in `pt_models/` (ONNX format only, e.g., `.onnx`)

## 🚀 How to Run the GUI

Make sure you're in the project root directory. Then, launch the GUI with:

```
python gui.py
```

## 🧠 How It Works

- Modify detection and model settings in the GUI.
- Press 💾 Update Config to save changes.
- Press 🚀 Run App to launch the AI detection engine in the background.
- Use 🔁 Reload Config to reset the GUI to match the saved JSON configuration.
- Close safely with ❌ Close App.

---

## 📂 Default Configuration File

Configuration is stored in `user_config.json`. The GUI reads and writes to this file automatically using `get_config()` and `set_config()` from `config.py`.

### ✅ Sample config for AMD (DirectML):

```json
{
  "screenShotHeight": 320,
  "screenShotWidth": 320,
  "useMask": true,
  "maskSide": "left",
  "maskWidth": 80,
  "maskHeight": 200,
  "aaMovementAmp": 0.4,
  "confidence": 0.4,
  "aaActivateKey": "CapsLock",
  "aaQuitKey": "8",
  "headshot_mode": true,
  "cpsDisplay": true,
  "visuals": false,
  "centerOfScreen": true,
  "model_path": "pt_models/v5_model.onnx",
  "model_type": "onnx",
  "enable_cuda": false,
  "device_type": "directml",
  "Close App": false
}
```

---

## 📢 Notes

- Ensure your model file (.onnx) exists at the given path.
- CUDA options are disabled for AMD GPU support.
- All runtime config changes are persisted in `user_config.json`.

---

# 🙌 Made With ❤️ by Bubbles The Dev & FNBubbles420 Org
### This app is part of the mission of [FNBUBBLES420 ORG](https://fnbubbles420.org) – helping gamers with disabilities break limits and play freely.

### 💌 Questions or Support?
- Join our Discord community.
- [Click To Join Discord](https://discord.fnbubbles420.org/invite)
---
