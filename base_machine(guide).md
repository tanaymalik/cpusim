# instructions on how to make a machine

instructions in steps:


STEP1)save machine and enter the ram values like this under the hardware modules section


![image](https://github.com/tanaymalik/cpusim/assets/86181483/fe65038a-46f2-45a7-b199-fa28b44fe046)



STEP2) edit the registers section to the values below

![image](https://github.com/tanaymalik/cpusim/assets/86181483/186367c2-62e0-4bd5-896f-8d23c25369b8)



STEP3) edit the conditionsbit values to:

![image](https://github.com/tanaymalik/cpusim/assets/86181483/03880f50-f08f-44f1-a809-72fe530b1977)



# EDITING MICROSINTRUCTIONS
STEP1) under decode:
DECODE IR -> IR


STEP2) under transferRtoR:

![image](https://github.com/tanaymalik/cpusim/assets/86181483/557ccca0-018c-4f08-9da5-04ac5ae978b2)



STEP 3) Under memoryacess:


![image](https://github.com/tanaymalik/cpusim/assets/86181483/0c22d94b-cb7e-4973-bb0c-bdfeb4c10e37)



STEP5) Under increment:


![image](https://github.com/tanaymalik/cpusim/assets/86181483/1ab64175-c582-4daa-b7d9-084490d163a7)


# EDITING FETCH SEQUENCE:

STEP1)Under transferRtoR insert the AR<PC value
- then under MemoryAccess insert the IR <- RAM[AR]
- Then under increment transfer incr pc
- then under trRtoR transfer AR<-IR(4-15)
- then finally decode IR

It should end up looking like this:


![image](https://github.com/tanaymalik/cpusim/assets/86181483/573139b7-2b65-4d63-a600-922116ab4e3a)



# editing machine instructions

STEP1) under edit do the following:

![image](https://github.com/tanaymalik/cpusim/assets/86181483/f94633de-da44-42b7-a85f-9f39606845e4)




The machine created using the following instructins is linked in the repository by the name of 'base_machine.cpu'





























