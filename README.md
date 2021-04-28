# Zeus
 Zeus - Ragnarök Packet Logger/Parser/Recorder

![License](https://img.shields.io/github/license/X-EcutiOnner/Zeus)
![Language](https://img.shields.io/badge/language-C%2B%2B-blue)
![Contributors](https://img.shields.io/github/contributors/X-EcutiOnner/Zeus.svg)

## Requeriments
  - Visual Studio 2019 (C++ support)

## Configuration
You can configure the dll in `config.h`

`Connection_use_WS2 <true|false>` Use Winsock lib instead of Ragnarok CRagConnection Functions
`DEBUG <true|false>` Enable / Disable Packet Dumper
`CRagConnection_instanceR_address 0xFFFFFFFF` CRagConnection_instanceR Hexadecimal Adresss
`CRagConnection_SendPacket_address 0xFFFFFFFF` CRagConnection_SendPacket Hexadecimal Adresss
`CRagConnection_RecvPacket_address 0xFFFFFFFF` CRagConnection_RecvPacket Hexadecimal  Adresss

## Finding CRagConnection Adresses
 1. Use BPE (`info.py`):
https://gitlab.com/4144/bpe/
2. Get it from output folder

## Updating PacketDB
PacketDB is based in recvpackets.txt

## Generating a new DLL
1. Open `Zeus.sln` with Visual Studio 2019
2. Set Compilation to `Release` and `x86`
3. Menu `Compilation` > `Compilate Solution` or `[Ctrl] + [Shift] + [B]`
4. Asi will be created at `release`folder

## Injecting into Ragnarök Client
1. Copy the Zeus.asi to Ragnarök Folder
2. Start Ragnarok

Or use some DLL Injector (recommended):
https://guidedhacking.com/resources/guided-hacking-dll-injector.4/

## Prints
- Packet Logger (DEBUG OFF):
![debugOFF](https://user-images.githubusercontent.com/60170564/116340170-e7f91e80-a808-11eb-96ca-c92895cc7672.png)

- Packet Logger (DEBUG ON):
![debugON](https://user-images.githubusercontent.com/60170564/116340257-11b24580-a809-11eb-8e5e-88ecbae56da6.png)
