# Copyright (c) 2022 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-g491 INTERFACE)

target_sources(mbed-g491
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-g491
    INTERFACE
        .
)

target_link_libraries(mbed-g491 INTERFACE mbed-stm32g491xe)
