# MDLR Tools

MDLR Tools is a PyQt5-based GUI application designed for managing Payment Request Forms (PRF) and FSI Data Entry Forms. The application provides a tabbed interface for easy navigation between different forms and tools.

## Features

- **Payment Request Form (PRF)**: Manage and process payment requests
- **FSI Data Entry Form**: Handle FSI (Financial Services Industry?) data entry operations
- Single instance enforcement: Prevents multiple instances of the application from running simultaneously

---

## For End Users: Standalone Executable (No Installation Required)

 Users can download and run MDLR Tools without installing Python or any dependencies.

### Download

Get the latest release from the `releases/` folder:
- `mdlr_tools_v1.0.0.zip` (approx. 192 MB)

### Installation

1. Extract the ZIP file to any folder on your computer
2. Navigate into the extracted `mdlr_tools` folder
3. Double-click `mdlr_tools.exe` to launch the application

That's it — no Python, no pip, no setup required.

### Notes

- The application is portable — you can run it from a USB drive or network location
- Keep the entire `mdlr_tools` folder intact; do not move the `.exe` out of the folder
- If you see a Windows SmartScreen or antivirus warning, click "Run anyway" (the app is safe)

---

## For Developers: Running from Source

### Requirements

- Python 3.x
- PyQt5
- ReportLab
- pdfplumber

### Installation

1. Clone or download the repository
2. Install required dependencies:
   ```
   pip install PyQt5 reportlab pdfplumber
   ```
3. Run the application:
   ```
   python mdlr_tools.py
   ```

### Building a Standalone Executable

To create your own standalone `.exe` for distribution:

1. Install PyInstaller:
   ```
   pip install pyinstaller
   ```
2. Build the executable:
   ```
   pyinstaller mdlr_tools.spec
   ```
3. The bundled application will be created in the `dist/mdlr_tools/` folder

---

## Contributing

Contributions are welcome. Please ensure that any changes maintain the application's single-instance behavior and follow the existing code structure.

## License

This project is licensed under the MIT License - see the LICENSE file for details.