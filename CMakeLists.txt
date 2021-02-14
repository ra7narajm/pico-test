cmake_minimum_required(VERSION 3.12)
  
# Pull in SDK (must be before project)
include(pico_sdk_import.cmake)

project(rrm_pico_test C CXX)
set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

# Initialize the Pico SDK
pico_sdk_init()

add_subdirectory(oled_ssd1306)
