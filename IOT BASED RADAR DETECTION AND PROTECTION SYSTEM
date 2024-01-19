#include <16f877a.h> 
#fuses hs,NOLVP,NOWDT,NOPROTECT 
#use delay(clock=20m) 
#use rs232(baud=9600, xmit=pin_c6, rcv=pin_c7, bits=8,parity=N, ERRORS)
void main() 
{ 
printf("AT\r\n");
delay_ms(500); 
printf("AT+CMGF=1\r\n");
delay_ms(500); 
printf("AT+CMGS=\"8825675690\"\r\n"); 
delay_ms(500);
printf("test sms\r\n");
delay_ms(500);
 putc(0x1A);
 delay_ms(1000);
 if((input(pin_c0)==1))
{
output_high(pin_d0);
output_high(pin_d1);
printf("ATD8825675690;\r\n");
delay_ms(1000);  
printf("AT\r\n");
delay_ms(500); 
printf("AT+CMGF=1\r\n");
delay_ms(500); 
printf("AT+CMGS=\"8825675690\"\r\n"); 
delay_ms(500);
printf("\f animal dete...");
delay_ms(500);
 putc(0x1A);
 delay_ms(1000);
}
else
{
output_low(pin_d0);
output_low(pin_d1);
 delay_ms(100);
}
}
