# Embedded Temperature Monitoring System

## Prerequisites
- Install GNU Arm Embedded Toolchain: [Download Here](https://developer.arm.com/downloads/-/gnu-rm)
- Add it to your system PATH and verify with: arm-none-eabi-gcc --version

## Overview
A real-time temperature monitoring system for ARM Cortex-based microcontrollers, using FreeRTOS.

## Features
Real-time temperature readings  
Secure AES-encrypted data transmission  
Low-power firmware for battery efficiency  

## Compilation
To compile for a PC (simulation):
```sh
gcc -o embedded_temp src/main.c src/freertos_tasks.c src/sensors.c src/aes_encryption.c -lfreertos -Iinclude
./embedded_temp
