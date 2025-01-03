<div align="center">

[![Verilator Simulation](https://github.com/RDSik/verilog-fir-filter/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/RDSik/axis-fir-filter/actions/workflows/main.yml)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/RDSik/axis-fir-filter/blob/master/LICENSE.txt)

</div><br/><br/>

# Usage

## Dependencies 

`python`, `chocolatey`, `winget`

## Installation

### Download python and git:
- [Install Chocolatey on Windows 10](https://gist.github.com/lopezjurip/2a188c90284bf239197b)

### Clone repository:
```bash
git clone https://github.com/RDSik/axis-fir-filter.git
cd axis-fir-filter
```

### Download packages:
```bash
pip install six
pip install hdlmake
```

### Download make (add to PATH system variable the Make bin folder: C:\Program Files (x86)\GnuWin32\bin):
```bash
winget install GnuWin32.make
```

## Create coe file

## Using Xilinx .coe file
```bash
cd src
py xilinx_coe_parser.py .\fir.coe
```

## Using python script
```bash
cd src
py fir_coe_gen.py
```

## Simulation

### Using Questa:
```bash
cd src/tb
vsim
do wave.do
```

### Using Verilator:
```bash
cd src/tb  
make
```
