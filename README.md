Creality Ender 3 S1 Pro Thumbnail Generator Fix for OrcaSlicer

Original files and sources:

* [Printables model page](https://www.printables.com/model/854118-orca-ender-3-s1-thumbnail-generator/files?utm_source=chatgpt.com)
* [Ultimaker community discussion](https://community.ultimaker.com/topic/44667-no-thumbnail-on-creality-3-vs2/?utm_source=chatgpt.com#comment-330593)

This is a fixed version of the OrcaSlicer post-processing script for generating compatible thumbnails for the Creality Ender 3 S1 Pro.

The original script generated thumbnails in **200×200** resolution, which does not work correctly on the Ender 3 S1 Pro.
This version changes the thumbnail resolution to **300×300**, which works properly on the printer LCD screen.

---

# Installation Guide

## 1. Download the Script

Download the fixed script from the GitHub release page:

[GitHub Releases](https://github.com/moto31924/Thumbnail-fixed-generator-for-Creality-Ender-3-S1-Pro-OrcaSlicer/releases/tag/Thumbnail?utm_source=chatgpt.com)

---

## 2. Install Python

Download and install Python from the official website:

[Python Official Website](https://www.python.org/downloads/?utm_source=chatgpt.com)

---

## 3. Install Pillow

Install the Pillow library using pip:

```bash
pip install pillow
```

---

## 4. Copy the Script

Place the script file into:

```text
C:\Users\[your_name]\AppData\Roaming\OrcaSlicer
```

---

## 5. Configure Post-Processing in OrcaSlicer

In OrcaSlicer, configure post-processing and set the paths to:

* `python.exe`
* `thumbnailgen.py`

<img width="404" height="213" alt="image" src="https://github.com/user-attachments/assets/10e97ca3-935e-41a4-8b13-46c862fd9ebd" />

---

## 6. Configure Printer Settings

Use the following printer settings:

<img width="679" height="173" alt="image" src="https://github.com/user-attachments/assets/a0d1ca91-317b-41dc-95d3-ae91b91c2029" />

### Required Settings

* **G-code Flavor:** `Marlin 2`
  *(Works only with Marlin 2 firmware)*

* **Thumbnail Format:** `300×300 / JPG`

---

## 7. Start Slicing

Save all settings and start slicing your model.

The generated G-code will automatically contain a compatible thumbnail that will be displayed on the printer LCD screen, including:

* Print time
* Filament usage
* Number of layers

The thumbnail is generated automatically every time you export G-code.

---

# Tested Configuration

* **OrcaSlicer Version:** `2.3.1`

* **Firmware:**
  [Creality Firmware Downloads](https://www.crealitycloud.com/downloads/firmware/ender-series/ender-3-s1-pro?utm_source=chatgpt.com)

* **Tested Firmware Version:**
  `Ender-3 S1_Pro_HWv24S1_301_SWV2.0.8.28F4_F401_FDM_LASER`

* **Motherboard:** `F4`

---

# Disclaimer

**USE AT YOUR OWN RISK**

