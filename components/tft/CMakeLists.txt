set(srcs
    "Ubuntu16.c"
    "comic24.c"
    "def_small.c"
    "DefaultFont.c"
    "DejaVuSans18.c"
    "DejaVuSans24.c"
    "minya24.c"
    "SmallFont.c"
    "tft.c"
    "tftspi.c"
    "tooney32.c"
)

set(includes
    "."
)

idf_component_register(SRCS "${srcs}"
                    INCLUDE_DIRS ${includes}
                    REQUIRES spidriver
)