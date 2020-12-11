set(srcs
    "src/main.cpp"
    "src/spiffs/esp_spiffs.c"
    "src/spiffs/spiffs_cache.c"
    "src/spiffs/spiffs_check.c"
    "src/spiffs/spiffs_gc.c"
    "src/spiffs/spiffs_hydrogen.c"
    "src/spiffs/spiffs_nucleus.c"
)

set(includes
    "src/spiffs"
    "src/tclap"
)

idf_component_register(SRCS "${srcs}"
                    INCLUDE_DIRS ${includes}
                    PRIV_REQUIRES spi_flash
)