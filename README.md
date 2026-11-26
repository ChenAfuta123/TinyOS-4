
markdown
# TinyOS-4

A tiny preemptive RTOS, drivers and UART bootloader for STM32F401RE (ARM Cortex-M4),
written from scratch in C — no HAL, no vendor libraries.

## Structure
| Folder | Contents |
| --- | --- |
| startup/ | Startup code and linker script |
| boot/ | UART bootloader |
| kernel/ | Scheduler, context switch, synchronization |
| drivers/ | GPIO, UART, I2C, SPI, DMA |
| app/ | Weather station application and shell |
| tests/ | Unit tests (run on PC) |
| tools/ | Python host tools |
| docs/ | Documentation and bug log |

## Hardware
NUCLEO-F401RE, BME280, SSD1306 OLED, DS3231 RTC, microSD module.

## Team

.gitignore

# Build output
build/
*.o
*.elf
*.bin
*.hex
*.map
*.d
*.lst

# Editor (keep shared VS Code config)
.vscode/*
!.vscode/extensions.json
!.vscode/launch.json
!.vscode/tasks.json

# OS / Python
Thumbs.db
.DS_Store
_pycache_/

.clang-format

yaml
BasedOnStyle: LLVM
IndentWidth: 4
ColumnLimit: 100
PointerAlignment: Right
AllowShortFunctionsOnASingleLine: None
AllowShortIfStatementsOnASingleLine: Never
SortIncludes: false

.gitattributes

* text=auto
