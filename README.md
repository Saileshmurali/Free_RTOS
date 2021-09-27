# Free_RTOS
This repository contains free RTOS used in STM32F4 discovery board with cubemx configuration using the CMSIS library for implementing Free RTOS. 
1. Basic_task.c file contains three tasks two of which is toggling of onboard LED connected at PD12 and PD13 at 250 and 500 ms respectively. The third task is toggling LED connected at PD14 when the onboard pushbutton connected to PA0 is used. This has been given the lowest priority. Note that all the three tasks will be implemented only when the task three, the one which involves push button has the least priority. Otherwise, since polling is used, the system CPU time will be allocated to task 3 alone and other tasks won't be executed
\n2.
