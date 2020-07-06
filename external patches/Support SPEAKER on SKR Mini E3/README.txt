For STM32_HIGH_DENSITY, change
	#define TONE_CHANNEL 8
to
	#define TONE_CHANNEL 4
  
in $HOME\.platformio\packages\framework-arduinoststm32-maple\STM32F1\cores\maple\tone.cpp
(see supplied original and modified tone.cpp)