# M251BSP_UART_RX_UnknownLength
 M251BSP_UART_RX_UnknownLength

update @ 2023/09/12

1. refer BSP : Level1_UART_ReceiveUnknowDataLengthPkg , and test UART transfer , 

- test RX_BUFFER_SIZE with 128 and 4096

2. when baud rate 115200 , transfer 128 bytes will spend 11.11ms

![image](https://github.com/released/M251BSP_UART_RX_UnknownLength/blob/main/baud_rate_115200_128bytes.jpg)	

when baud rate 115200 , transfer 4096 bytes will spend 355.56ms

![image](https://github.com/released/M251BSP_UART_RX_UnknownLength/blob/main/baud_rate_115200_4096bytes.jpg)	

4. Use Serial Port Utility to test transfer data

when transfer 128 bytes , with 60 ms period , below is transfer result (monitor TX and RX transfer bytes)

![image](https://github.com/released/M251BSP_UART_RX_UnknownLength/blob/main/UART_128BYTES_60ms.jpg)	

when transfer 4096 bytes , with 2000 ms period , below is transfer result ,

![image](https://github.com/released/M251BSP_UART_RX_UnknownLength/blob/main/UART_4096BYTES_2000ms.jpg)	

when transfer 4096 bytes , with 1000 ms period , below is transfer result ,

![image](https://github.com/released/M251BSP_UART_RX_UnknownLength/blob/main/UART_4096BYTES_1000ms.jpg)	


