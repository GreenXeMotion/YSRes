# YSRes

A Parser of a certain anime game's data files (WIP)

Current target version: 3.4

## Requirements

- Python 3

## How to run

- Clone this repository
```shell
git clone https://github.com/paimooon/YSRes
```
- Place blk files in `YSRes/blk`
- Edit textMapLanguage and xorKey in `prepare.py`
- Install Python modules
```shell
pip install kaitaistruct XlsxWriter
```
- Run prepare
```shell
python prepare.py
```
- Run main
```shell
# example
python main.py -t -e -o -l KR -i 10000078 -s
```

## Argument usage
```
usage: main.py [-t] [-e] [-o] [-l LANG] [-i ID] [-s]

Arguments:
    -t --textmap        # Dump TextMap (-l argument needed)
    -e --excel          # Dump ExcelBinOutput
    -o --output         # Generate output (-l, -i argument needed)

    -l --lang [LANG]    # Set language (Example: KR)
    -i --id [ID]        # Set character id (Example: 10000078)

    -s                  # Xlsx skill short version
```

## BLK info

```
00/25539185 => ExcelBinOutput (must need)
01/26692920 => CHS
02/27251172 => 
03/25181351 => 
04/25776943 => EN
05/20618174 => 
06/25555476 => 
07/30460104 => 
08/32244380 => 
09/22299426 => KR
10/23331191 => 
11/21030516 => 
12/32056053 => 
13/34382464 => 
```

## Future Goals

- Args support
- GenerateElemBall data

## Credit
- partypooper for the original [KaitaiDumper](https://github.com/partypooperarchive/KaitaiDumper)
- WeedwackerPS for the [DataParser](https://github.com/WeedwackerPS/DataParser)
- Raz for [Studio](https://gitlab.com/RazTools/Studio)
- ToaHartor for [GenshinScripts](https://github.com/ToaHartor/GenshinScripts)
