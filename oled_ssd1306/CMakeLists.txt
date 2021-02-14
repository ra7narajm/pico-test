add_executable(oled_demo oled_main.c oled_font.h ssd1306_i2c.c ssd1306_i2c.h)

target_link_libraries(oled_demo pico_stdlib hardware_i2c)

# enable usb output, disable uart output
pico_enable_stdio_usb(oled_demo 1)
pico_enable_stdio_uart(oled_demo 0)

# create map/bin/hex/uf2 file etc.
pico_add_extra_outputs(oled_demo)
