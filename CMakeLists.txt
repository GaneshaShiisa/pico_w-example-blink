cmake_minimum_required(VERSION 3.12)

set(PICO_SDK_PATH "C:/Program Files/Raspberry Pi/Pico SDK v1.5.0/pico-sdk")
set(PICO_BOARD "pico_w")

# Pull in SDK (must be before project)
include(pico_sdk_import.cmake)

# set the project name
project(picow_blink)

set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

# Initialize the SDK
pico_sdk_init()

# Subdirectory
add_subdirectory(src)
