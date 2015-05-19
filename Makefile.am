
AUTOMAKE_OPTIONS  = subdir-objects

FP_FLAGS        = -mfloat-abi=hard -mfpu=fpv4-sp-d16
PREFIX          = arm-none-eabi

CC              = $(PREFIX)-gcc
AR              = $(PREFIX)-ar
CFLAGS          = -Wall -Wextra -Wimplicit-function-declaration \
		  -Wredundant-decls -Wmissing-prototypes -Wstrict-prototypes \
		  -Wundef -Wshadow \
		  -I../../../include -fno-common \
		  -mcpu=cortex-m4 -mthumb $(FP_FLAGS) \
		  -Wstrict-prototypes \
		  -ffunction-sections -fdata-sections -MD -DSTM32F4


lib_LIBRARIES = libmpu9150.a

libmpu9150_a_SOURCES = src/MPU9150.cpp
