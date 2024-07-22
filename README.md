# CloudVM BIOS
This repository contains the code for the **minimal BIOS firmware** used to boot up the selected virtual machine. **CloudVM BIOS** is based on [SeaBIOS](https://github.com/coreboot/seabios).

## Building image
To build for **QEMU** *(CloudVM uses QEMU by default)*, follow the steps below:

1. Clone the BIOS repository:
```bash
git clone https://github.com/SectonCloud/BIOS
```

2. Install **`build-essentials`** & **`git`**:
```bash
sudo apt-get install build-essential git -y
```

3. Build firmware image:
```bash
make
```

The resulting file *"out/bios.bin"* contains the processed BIOS image.