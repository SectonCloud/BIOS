# CloudVM BIOS
This repository contains the code for the **minimal BIOS firmware** used to boot up the selected virtual machine. **CloudVM BIOS** is based on [SeaBIOS](https://github.com/coreboot/seabios).

## Building image
To build for **QEMU** *(CloudVM uses QEMU by default)*, follow the steps below:

1. Clone the BIOS repository:
```bash
git clone https://github.com/SectonCloud/BIOS
```

2. Install **`build-essential`** & **`git`**:
```bash
sudo apt-get install build-essential git -y
```

3. Build firmware image:
```bash
make
```

The resulting file *"out/bios.bin"* contains the processed BIOS image.

## Troubleshooting
### scripts/xxx.sh: Permission denied
`chmod +x scripts/xxx.sh`
### python: not found
Make sure that `python3` and `python-is-python3` are installed.