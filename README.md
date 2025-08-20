# Document Reader - Releases

This repository contains compiled binaries and release artifacts for Document Reader.

## Current Release: v1.0.0

### Downloads

- [document-reader-v1.0.0-macos.tar.gz](https://github.com/shyamalschandra/document-reader-releases/releases/download/v1.0.0/document-reader-v1.0.0-macos.tar.gz)
  - **SHA256**: `a398a5106e5e09bf7fd98e3f686268696e02a38b35552ffea3d9cdbdf73ad3ee`
  - **Platform**: macOS 13.0+
  - **Architecture**: Universal (Intel + Apple Silicon)

### What's Included

- `document-reader`: Command-line interface
- `DocumentReaderGUI`: SwiftUI graphical application

### Installation

#### Option 1: Homebrew (Recommended)
```bash
brew tap shyamalschandra/document-reader
brew install document-reader
```

#### Option 2: Manual Installation
```bash
# Download and extract
curl -L https://github.com/shyamalschandra/document-reader-releases/releases/download/v1.0.0/document-reader-v1.0.0-macos.tar.gz | tar -xz

# Install CLI
sudo cp document-reader /usr/local/bin/

# Install GUI (create app bundle)
mkdir -p DocumentReader.app/Contents/MacOS
cp DocumentReaderGUI DocumentReader.app/Contents/MacOS/DocumentReader
cp DocumentReader.app /Applications/
```

### System Requirements

- macOS 13.0 or later
- VLC media player
- 50MB free disk space

### Usage

```bash
# CLI
document-reader document.pdf --output /path/to/output --play

# GUI
open /Applications/DocumentReader.app
```

### Verification

Verify the download integrity using SHA256:
```bash
shasum -a 256 document-reader-v1.0.0-macos.tar.gz
# Should match: a398a5106e5e09bf7fd98e3f686268696e02a38b35552ffea3d9cdbdf73ad3ee
```

### Support

- [Main Repository](https://github.com/shyamalschandra/Document-Reader-I)
- [Homebrew Tap](https://github.com/shyamalschandra/homebrew-document-reader)

### License

Copyright (C) 2025, Shyamal Suhana Chandra

### Release Notes

#### v1.0.0 (Initial Release)
- PDF text extraction and processing
- Text-to-speech audio generation
- M3U playlist creation for VLC
- Command-line interface with full argument parsing
- Modern SwiftUI graphical interface
- Homebrew installation support
- Comprehensive test suite
- Documentation and usage examples
