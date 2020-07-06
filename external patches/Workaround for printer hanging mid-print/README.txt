Hopefully this is no longer needed with the changes from Marlin
pull-request https://github.com/MarlinFirmware/Marlin/pull/19301

However, even then the hack won't hurt: basically it will check
for potential serial overrun and avoid getting stuck by dropping
some data (which will get repeated by higher level checks
normally).

Change $HOME\.platformio\packages\framework-arduinoststm32-maple\STM32F1\system\libmaple\usart_private.h
from the .orig version in this folder to the new one.  Ensure
the framework (especially the maple library) is cleanly rebuilt
so that the change is actually taken along!
