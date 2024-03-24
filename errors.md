```
Compiling: platforms/chibios/drivers/serial.c                                                      platforms/chibios/drivers/serial.c:20:6: error: #error "chSysPolledDelayX method not supported on this platform"
   20 | #    error "chSysPolledDelayX method not supported on this platform"
      |      ^~~~~
platforms/chibios/drivers/serial.c: In function 'Thread1':
platforms/chibios/drivers/serial.c:90:9: error: implicit declaration of function 'palWaitLineTimeout' [-Werror=implicit-function-declaration]
   90 |         palWaitLineTimeout(SOFT_SERIAL_PIN, TIME_INFINITE);
      |         ^~~~~~~~~~~~~~~~~~
platforms/chibios/drivers/serial.c: In function 'soft_serial_target_init':
platforms/chibios/drivers/serial.c:103:5: error: implicit declaration of function 'palEnablePadEvent'; did you mean 'pal_lld_enablepadevent'? [-Werror=implicit-function-declaration]
  103 |     palEnablePadEvent(PAL_PORT(SOFT_SERIAL_PIN), PAL_PAD(SOFT_SERIAL_PIN), PAL_EVENT_MODE_FALLING_EDGE);
      |     ^~~~~~~~~~~~~~~~~
      |     pal_lld_enablepadevent
cc1: all warnings being treated as errors
 [ERRORS]
 | 
 | 
 | 
make[1]: *** [builddefs/common_rules.mk:376: .build/obj_spruce_vial/serial.o] Error 1
Make finished with errors
make: *** [Makefile:416: spruce:vial] Error 1
```