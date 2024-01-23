# ==============================================================================
# AMS CMake File
# ==============================================================================

# program objects --------------------------------------------------------------
SET(PROG_SRC
        ABSStatServerOptions.cpp
        ABSStatServer.cpp
        )

# final build ------------------------------------------------------------------
ADD_EXECUTABLE(abs-ijobstat ${PROG_SRC})

TARGET_LINK_LIBRARIES(abs-ijobstat ${ALL_LIBS})

INSTALL(TARGETS
            abs-ijobstat
        DESTINATION
            sbin
        )

