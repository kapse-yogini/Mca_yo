Exp8: SERIAL COMMUNICATION

include <pis24520.h>

//Configuration bit setting// #pragma config OSC-HS //oscillator selection pragma config WDT-OFF //Disable Watchdog timer

Spragma config LVF-OFF //Disable Low Voltage Programming #pragma config FBADEN-OFF //Disable PORTS Analog inputs

vold Transmit String unsigned char *string! for(i=0;string[A]1-021+) //loop till end of the string

unsigned char 1=0;

while (PIRibits.TXIF-01

TXREG-string():

unsigned char HSG111 "UART COMMUNICATION NEAR" }; unsigned char M5211- "TRANSMITTING STRING SEA ("SEND 10 Characters \r\n"17

unsigned char MSG31 unsigned char M5041]("Received Data \r\n")

void main(void)

unsigned chas 1-0;

unsigned char RX DATA[20]; unsigned char MSGS[]=("Received Data \r\n");

TRISCbits.TRISC7-1; TRISCbits TRISC6-01

// RXD as Input // TKD as Output

of A

Comedy

RCSTA 0x90;

TXSTA - 0x24 BAUDCON 0x00;

SPARG0x19:

SPBRGH 0:

Transmit String (HSG) Transmit String (MSG2); Transmit String (MSG3);

for (j=0; j<10; 3++)

while(PIRIbits.ROIF -- 0); RX_DATA[3] ACREG;

RX_DATA[10]='\0';
Transmit_String (MSG4); Transmit String (RX_DATA);

while(1);
