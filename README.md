# Tiva-C-Series---TM4C123GH6PM
Phase Shifted PWM on TIVA C series Microcontrollers

I'm currently on a project designing a Dual Active Bridge (DAB) DC/DC converter
and the way you go about controlling a DAB is you control the phase shift 
between the PWM of the two legs of the converters. 

The displayed method works for any work cycle, and you can control how you want the phase shift.

A problem detected is that when using different PWM modules, has a delay in enabling the
PWM outputs, which can be a problem because I could not synchronize them globally. Anyway, 
when the PWM outputs are in the same module (PWM 0 or PWM 1) you will have the delayed signal as you wish.
In the example, it generates a 40KHz signal with a 180° lag between them.
