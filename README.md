English:

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
or
https://pypi.org/project/pillow/
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

Česky:

# Oprava generátoru náhledů pro Creality Ender 3 S1 Pro v OrcaSliceru

Původní soubory a zdroje:

* [Printables stránka modelu](https://www.printables.com/model/854118-orca-ender-3-s1-thumbnail-generator/files?utm_source=chatgpt.com)
* [Diskuze na Ultimaker Community](https://community.ultimaker.com/topic/44667-no-thumbnail-on-creality-3-vs2/?utm_source=chatgpt.com#comment-330593)

Toto je upravená verze post-processing skriptu pro OrcaSlicer, která generuje kompatibilní náhledy pro tiskárnu Creality Ender 3 S1 Pro.

Původní skript generoval náhledy v rozlišení **200×200**, které na Ender 3 S1 Pro nefunguje správně.
Tato upravená verze mění rozlišení náhledu na **300×300**, které již správně funguje na LCD displeji tiskárny.

---

# Návod k instalaci

## 1. Stažení skriptu

Stáhněte opravený skript z GitHub Releases:

[GitHub Releases](https://github.com/moto31924/Thumbnail-fixed-generator-for-Creality-Ender-3-S1-Pro-OrcaSlicer/releases/tag/Thumbnail?utm_source=chatgpt.com)

---

## 2. Instalace Pythonu

Stáhněte a nainstalujte Python z oficiálních stránek:

[Oficiální stránky Pythonu](https://www.python.org/downloads/?utm_source=chatgpt.com)

---

## 3. Instalace Pillow

Nainstalujte knihovnu Pillow pomocí příkazu:

```bash id="iv71yi"
pip install pillow
```

nebo:

[Pillow na PyPI](https://pypi.org/project/pillow/?utm_source=chatgpt.com)

---

## 4. Zkopírování skriptu

Umístěte soubor skriptu do složky:

```text id="jjuhz3"
C:\Users\[vaše_jméno]\AppData\Roaming\OrcaSlicer
```
<img width="404" height="213" alt="image" src="https://github.com/user-attachments/assets/10e97ca3-935e-41a4-8b13-46c862fd9ebd" />

---

## 5. Nastavení Post-Processing v OrcaSliceru

V OrcaSliceru nastavte post-processing a zadejte cesty k:

* `python.exe`
* `thumbnailgen.py`

---

## 6. Nastavení tiskárny

Použijte následující nastavení tiskárny:

### Požadované nastavení

* **G-code Flavor:** `Marlin 2`
  *(Funguje pouze s firmwarem Marlin 2)*

* **Thumbnail Format:** `300×300 / JPG`
<img width="679" height="173" alt="image" src="https://github.com/user-attachments/assets/a0d1ca91-317b-41dc-95d3-ae91b91c2029" />

---

## 7. Spuštění slicování

Uložte všechna nastavení a začněte slicovat model.

Vygenerovaný G-code bude automaticky obsahovat kompatibilní náhled, který se zobrazí na LCD displeji tiskárny, včetně:

* času tisku
* spotřeby filamentu
* počtu vrstev

Náhled se generuje automaticky při každém exportu G-code.

---

# Testovaná konfigurace

* **Verze OrcaSliceru:** `2.3.1`

* **Firmware:**
  [Stažení firmware Creality](https://www.crealitycloud.com/downloads/firmware/ender-series/ender-3-s1-pro?utm_source=chatgpt.com)

* **Testovaná verze firmware:**
  `Ender-3 S1_Pro_HWv24S1_301_SWV2.0.8.28F4_F401_FDM_LASER`

* **Základní deska:** `F4`

---

# Upozornění

**Používáte na vlastní riziko.**

