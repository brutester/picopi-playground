add_executable(lcd_ssd1306_i2c
        lcd_ssd1306_i2c.c
        )

# Pull in our (to be renamed) simple get you started dependencies
target_link_libraries(lcd_ssd1306_i2c pico_stdlib hardware_i2c)

# create map/bin/hex file etc.
pico_add_extra_outputs(lcd_ssd1306_i2c)

# add url via pico_set_program_url
example_auto_set_url(lcd_ssd1306_i2c)