# CloneWB

CloneWB is a powerful tool to download websites from the internet to your computer, Developed by LocalSix, the tool provides an interactive command-line interface and options for direct scripting.

![CLONEWB Banner](https://github.com/user-attachments/assets/f7da62db-e9be-4458-9fd6-11c45090d52a)

## Fitur

- Complete website clone with all assets
- Support for setting crawl depth
- Multi-threading for faster retrieval
- Automatic output to ZIP file
- Automatic handling for virtual environments
- Easy-to-use interactive command-line interface

## Rules

- Python 3.6 or later
- The required Python packages will be installed automatically.

## How to use

### The fast way

Just run the file `clonewb.py`:

```bash
python clonewb.py
```

The script will automatically file:
1. Check and create virtual environment if needed
2. Installing all required dependencies
3. Displays an interactive command-line interface

### Interactive Mode

After running the tool, you will see an interactive prompt:

```
CLONEWB >>
```

Available commands:
- `clone [URL]` - Clone website with default settings
- `advanced [URL] [DEPTH] [THREADS]` - Cloning with custom settings
- `clean` - Delete all output files, logs, and archives
- `clear` - Clear the terminal screen
- `version` - Show version information
- `help` - Show command list
- `exit` - Exit the program

Example:
```
CLONEWB >> clone https://example.com
```

### Command Line Mode

You can also use this tool directly from the command line:

```bash
# Clone website with default settings
python clonewb.py -u https://example.com

# Cloning with custom settings
python clonewbl.py -u https://example.com -d 5 -t 10

# Clean output files
python clonewb.py --clean
```

### Opsi Command-Line

- `-u, --url` - URL of the website to be cloned
- `-d, --depth` - Maximum crawling depth (default: 3)
- `-t, --threads` - Number of concurrent threads (default: 5)
- `-o, --output` - Directory output (default: "output")
- `--clean` - Clean up output and log files

## Output Structure

```
output/
├── html/
│   ├── index.html
│   └── ...
├── css/
│   └── ...
├── js/
│   └── ...
├── images/
│   └── ...
└── other/
    └── ...
```

Once cloning is complete, all files will be archived into a ZIP file with a name based on the website domain.

### Erasing Data

Use commands `clean` to delete all output, log, and archive files:

```
CLONEWB >> clean
```

## Lisensi

[MIT License](https://opensource.org/licenses/MIT)

## Developer

Developed by [LocalSix](https://github.com/localsix)

## Contribution

Contributions are always welcome! Please fork the repository and submit a pull request.
