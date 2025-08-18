# Augment Cleaner v2.0 - Enhanced Privacy Protection

A C# Windows Forms application specifically designed for newer Augment versions (0.492.2+) that scans for and removes personal data, system fingerprints, and usage tracking.

**🎯 100% Feature-Equivalent to Python Version** - This C# version provides identical functionality to the original Python script with the added benefit of a modern, professional GUI interface.

## 🎨 Modern Design Features

- **Professional Dark Header** with gradient background
- **Card-based Layout** with subtle shadows and modern styling
- **Color-coded Status Indicators** with emoji icons
- **Modern Button Design** with hover effects and descriptions
- **Enhanced Typography** using Segoe UI font family
- **Responsive Layout** that adapts to window resizing
- **Rich Text Logging** with improved readability

## Features

🔍 **Comprehensive Scanning**
- Detects Augment extensions across multiple IDEs (VSCode, VSCode Insiders, Cursor)
- Deep scans databases for personal data collection
- Identifies system fingerprinting attempts
- Finds cloud synchronization traces
- Detects AI/ML training data collection
- Scans Windows Registry for Augment entries
- Checks network traces and hosts file modifications

🧹 **Safe Cleaning**
- Creates automatic backups before any removal
- Removes extensions and associated data
- Cleans personal data from databases
- Removes system fingerprint files
- Clears cloud activity logs
- Removes AI training data files
- Provides registry entry warnings

🛡️ **Privacy Protection**
- Specifically targets newer Augment versions with enhanced data collection
- Identifies and removes personal information like usernames and system details
- Protects against hardware fingerprinting
- Removes usage tracking data

## Requirements

- Windows 10/11
- .NET 9.0 Runtime
- Administrator privileges (recommended for full system scan)

## Usage

1. **Launch the application**
   ```bash
   dotnet run
   ```

2. **Scan for Augment data**
   - Click "🔍 Scan for Augment Data"
   - Wait for the comprehensive scan to complete
   - Review the findings in the log window

3. **Clean found data**
   - If Augment data is found, click "🧹 Clean Found Data"
   - Confirm the cleaning operation
   - Backups will be automatically created

## What Gets Scanned

### Extensions
- VSCode extensions directory
- VSCode Insiders extensions
- Cursor IDE extensions
- Version detection for enhanced data collection

### Databases
- VSCode state databases
- Personal data entries
- Username and system information
- Configuration data

### System Files
- Hardware fingerprint files
- System identification data
- Machine-specific information

### Cloud Data
- Synchronization logs
- Upload activity traces
- Remote server connections

### AI Training Data
- Machine learning model files
- Training data collections
- Neural network data

### Registry Entries
- Windows Registry keys
- Installation records
- Configuration entries

## Backup Location

All removed data is backed up to:
```
%USERPROFILE%\Documents\augment_backup_YYYYMMDD_HHMMSS\
```

## Building from Source

1. **Clone or download the source code**
2. **Install dependencies**
   ```bash
   dotnet restore
   ```
3. **Build the application**
   ```bash
   dotnet build
   ```
4. **Run the application**
   ```bash
   dotnet run
   ```

## Dependencies

- System.Data.SQLite - For database operations
- Microsoft.Win32.Registry - For registry access
- System.Windows.Forms - For GUI interface

## Security Notes

- This tool requires file system access to scan for Augment data
- Administrator privileges may be needed for complete system scanning
- All operations create backups for safety
- Registry cleaning requires manual confirmation

## Disclaimer

This tool is designed to help protect user privacy by removing data collection from Augment extensions. Use at your own risk and always review the backup files before permanent deletion.

## Version History

- **v2.0** - C# Windows Forms implementation with enhanced GUI
- **v1.0** - Original Python console version

## License

This software is provided as-is for privacy protection purposes.
