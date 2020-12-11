set(srcs
"spiffs_vfs.c"
"esp_spiffs.c"
"list.c"
"mutex.c"
"spiffs_cache.c"
"spiffs_check.c"
"spiffs_gc.c"
"spiffs_hydrogen.c"
"spiffs_nucleus.c"
)

set(includes
    "."
)

idf_component_register(SRCS "${srcs}"
                    INCLUDE_DIRS ${includes}
                    REQUIRES spi_flash
                    PRIV_REQUIRES spi_flash
)