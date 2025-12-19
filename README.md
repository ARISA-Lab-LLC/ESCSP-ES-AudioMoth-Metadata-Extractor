# ESCSP-ES-AudioMoth-Metadata-Extractor (ES AME)

## Description
ES AudioMoth Metadata Extractor (ES AME) is a Python-based utility developed by the Eclipse Soundscapes team to extract and organize metadata from AudioMoth field recorders. It retrieves device-level information stored on the SD card, including:
* 📎 Serial number of the AudioMoth device
* ⚙️ Firmware version
* 📁 Number and size of audio files
* ⏱️ Start and end timestamps for each recording
* 🌡️ Temperature metadata (if available)


AME supports batch processing, making it ideal for large-scale deployments across many sites. The structured metadata it generates can be used for quality control, recorder validation, and streamlined dataset documentation—especially in preparation for open publication via tools like AZUS.

## Key Features
* Extract AudioMoth serial number from metadata.
*  Retrieve firmware version of each recording device.
* Count number of audio files and calculate file sizes.
* Parse start and end timestamps for each recording.
*  Capture temperature metadata if available.
*  Batch process multiple SD cards or folders.
*  Generate structured output for downstream use (e.g., with AZUS).
  
## Example Use Case
Researchers collecting data using dozens of AudioMoth recorders can use AME to validate devices, track firmware versions, and confirm timestamp alignment across datasets. This ensures data transparency and consistency when preparing large volumes of sound data for public release or scientific analysis.

## Installation
```bash
git clone [https://github.com/EclipseSoundscapes/ame.git](https://github.com/ARISA-Lab-LLC/ESCSP-ES-AudioMoth-Metadata-Extractor.git
cd ESCSP-ES-AudioMoth-Metadata-Extractor
pip install -r requirements.txt
```

## Usage
Basic usage: (In develeopment. Not Correct)
ame/

*See `examples/` and `docs/` for more options.*

## Project Structure (In develeopment. Not Correct)
ame/
├── ame.py
├── parser/
│   ├── metadata_reader.py
│   └── utils.py
├── examples/
├── docs/
└── README.md

## License
BSD 3-Clause License. See LICENSE file for details.

## Copyrights, Acknowledgements, and Atrributions

Eclipse Soundscapes is an enterprise of ARISA Lab, LLC and is supported by NASA award No. 80NSSC21M0008. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Aeronautics and Space Administration.

## About

AME is one of five open tools shared by Eclipse Soundscapes:
1. AZUS – Automated Zenodo Upload Software
2. Eclipse Look-Up Tool – Public web tool for eclipse timing by ZIP code
3. Eclipse Phase Timing Tool – Backend processor for latitude/longitude eclipse phase times
4. WAVES – Audio extraction and time-window matching for multi-day .wav files
5. AME – AudioMoth Metadata Extractor
