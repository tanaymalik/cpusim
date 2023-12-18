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
order matters a lot here

![image](https://github.com/tanaymalik/cpusim/assets/86181483/0be6df0a-5f37-4535-b110-2ba89b26fa26)




# editing machine instructions

STEP1) under edit do the following:

![image](https://github.com/tanaymalik/cpusim/assets/86181483/f94633de-da44-42b7-a85f-9f39606845e4)

STEP2) CREATE 3 'NEW'


![image](https://github.com/tanaymalik/cpusim/assets/86181483/24375f2d-5c65-4952-9ebc-21d76f8a5311)


STEP4) UNDER IO CREATE INPUT AND OUTPUT:

![image](https://github.com/tanaymalik/cpusim/assets/86181483/81cd2059-11c4-427a-9948-f67fd7ff417b)

STEP5) 
under implementation every implementation is followed by an 'end'

so when we insert input from IO we follow it by end

same for output


STEP6) FOR HAULT

![image](https://github.com/tanaymalik/cpusim/assets/86181483/cbf8ca3d-a076-4db6-b86d-5a83d8e804b0)

 CREATE hault bit under setcondt like this 
 and then insert followed by end
 






The machine created using the following instructins is linked in the repository by the name of 'base_machine.cpu'





























