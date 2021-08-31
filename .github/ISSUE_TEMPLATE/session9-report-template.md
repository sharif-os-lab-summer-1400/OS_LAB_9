Team Name: `97110285-97101286`

Student Name of member 1: `Mohammadreza Abdi`
Student No. of member 1: `97110285`

Student Name of member 2: `Alireza Ilami`
Student No. of member 2: `97101286`

- [x] Read Session Contents.

## Section 9.3
- [x] Printing all linux interrupts
    - [x] ![image](https://user-images.githubusercontent.com/45389577/131242119-e8e8c55e-4cc3-4bfd-896b-4eff868db86f.png)
    - [x] At first, we open the file with fopen. If it is null, we print the related error. Then, we read the file line by line using the fgets function. Each line is our buffer at the time. After everything is read and printed, we close the filereader.
    - [x] /proc/interrupts: recording number of interrupts per IRQ, type of interrupt, device name, num of interrupts per CPU, etc.
          First col: IRQ number. The IRQ number is a numeric way to assign the priority that the devices have with the CPU
          Second col: Number of interrupts per CPU. This could extend to col 2,3 and more; depending on your cpu numbers.
          Third col: Type of the interrupt.
          Last col: The device name which is located on that IRQ.
    - [x] ![image](https://user-images.githubusercontent.com/45389577/131242152-13494b2c-b236-4e2a-ab5f-3822b3995e77.png)  
    - [x] نیازمندی خاصی برای نوشتن این برنامه وجود نداشت. صرفا نیاز بود که هدرفایل های زیر را اول کد اضافه کنیم:
          <stdio.h>, <stdlib.h>

## Section 9.4
- [x] Adding a new interrupt  
    - [x] Just the discription:
          Two functions should be used: request_irq(), and free_irq()
          We have to write a kernel module in which it creates an interrupt with the request_irq() function. This function returns an integer which if is 0, it means the interrupts creation is ok. Anything else means a failure. Finally, we should resolve the interrupt and put it out of the /proc/interrupts list with free_irq() function. 
    - [x] The code is not implemented. I just searched how this could be done.
