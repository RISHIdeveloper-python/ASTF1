#ASTF1

A Python-based AST1 binary asset parser and patching tool.

ASTF1 is an experimental Python project focused on safely parsing, validating, and patching AST1 binary assets.

Features

- AST1 header and pointer-table validation
- Structural overlap and duplicate-key detection
- Bounded XZ/LZMA decompression
- RGBA vector patching
- SHA-256 source-change detection
- File locking
- Temporary-file-based replacement
- File and directory synchronization checks
- Fault-injection and subprocess crash testing

Testing

The current test suite contains 15 tests covering:

- Malformed binary structures
- Compression errors and output limits
- Interrupted writes and synchronization failures
- Replacement failures
- Subprocess crash scenarios

Recorded test result: 15 tests passed.

Project Structure

ASTF1/
├── astf1.py
├── README.md
└── LICENSE

Requirements

- Python 3
- Standard-library modules used by the project

Running

Run the test suite:

python astf1.py

Limitations

- ASTF1 currently supports the AST1 format implemented in this project.
- The recorded tests do not establish universal correctness or production readiness.
- Compatibility and durability behavior may vary across operating systems and filesystems.

Project Status

Experimental engineering project. The current version is preserved as a portfolio checkpoint.

Author

RISHI
GitHub: "RISHIdeveloper-python" (https://github.com/RISHIdeveloper-python)
