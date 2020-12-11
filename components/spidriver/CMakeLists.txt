set(srcs
    "spi_master_lobo.c"
)

set(includes
    "."
)

idf_component_register(SRCS "${srcs}"
                    INCLUDE_DIRS ${includes}
)