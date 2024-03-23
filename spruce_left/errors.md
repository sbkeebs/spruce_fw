```
(venv-qmk) astra@pop-os:~/vial-qmk$ make starboards/spruce_left:vial
Making starboards/spruce_left with keymap vial

Generating: .build/obj_starboards_spruce_left_vial/src/default_keyboard.c                           [OK]
arm-none-eabi-gcc (15:10.3-2021.07-4) 10.3.1 20210621 (release)
Copyright (C) 2020 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Size before:
   text	   data	    bss	    dec	    hex	filename
      0	  33702	      0	  33702	   83a6	starboards_spruce_left_vial.bin

Generating: .build/obj_starboards_spruce_left_vial/src/info_config.h                                [OK]
Generating: .build/obj_starboards_spruce_left_vial/src/default_keyboard.h                           [OK]
Compiling: .build/obj_starboards_spruce_left_vial/src/default_keyboard.c                           In file included from platforms/chibios/platform_deps.h:18,
                 from quantum/quantum.h:18,
                 from ./.build/obj_starboards_spruce_left_vial/src/default_keyboard.h:27,
                 from .build/obj_starboards_spruce_left_vial/src/default_keyboard.c:26:
./lib/chibios/os/hal/include/hal.h:132:2: error: #error "invalid configuration file"
  132 | #error "invalid configuration file"
      |  ^~~~~
./lib/chibios/os/hal/include/hal.h:136:2: error: #error "obsolete or unknown configuration file"
  136 | #error "obsolete or unknown configuration file"
      |  ^~~~~
In file included from ./lib/chibios/os/hal/include/hal.h:249,
                 from platforms/chibios/platform_deps.h:18,
                 from quantum/quantum.h:18,
                 from ./.build/obj_starboards_spruce_left_vial/src/default_keyboard.h:27,
                 from .build/obj_starboards_spruce_left_vial/src/default_keyboard.c:26:
./lib/chibios/os/hal/ports/STM32/STM32F0xx/hal_lld.h:503:2: error: #error "Using a wrong mcuconf.h file, STM32F0xx_MCUCONF not defined"
  503 | #error "Using a wrong mcuconf.h file, STM32F0xx_MCUCONF not defined"
      |  ^~~~~
In file included from ./lib/chibios/os/hal/include/hal_serial.h:99,
                 from ./lib/chibios/os/hal/include/hal.h:319,
                 from platforms/chibios/platform_deps.h:18,
                 from quantum/quantum.h:18,
                 from ./.build/obj_starboards_spruce_left_vial/src/default_keyboard.h:27,
                 from .build/obj_starboards_spruce_left_vial/src/default_keyboard.c:26:
./lib/chibios/os/hal/ports/STM32/LLD/USARTv2/hal_serial_lld.h:369:2: error: #error "SERIAL driver activated but no USART/UART peripheral assigned"
  369 | #error "SERIAL driver activated but no USART/UART peripheral assigned"
      |  ^~~~~
In file included from platforms/gpio.h:21,
                 from quantum/matrix.h:22,
                 from quantum/quantum.h:20,
                 from ./.build/obj_starboards_spruce_left_vial/src/default_keyboard.h:27,
                 from .build/obj_starboards_spruce_left_vial/src/default_keyboard.c:26:
platforms/chibios/gpio.h:21:9: error: unknown type name 'ioline_t'
   21 | typedef ioline_t pin_t;
      |         ^~~~~~~~
 [ERRORS]
 | 
 | 
 | 
make[1]: *** [builddefs/common_rules.mk:376: .build/obj_starboards_spruce_left_vial/.build/obj_starboards_spruce_left_vial/src/default_keyboard.o] Error 1
make: *** [Makefile:416: starboards/spruce_left:vial] Error 1
Make finished with errors
```
