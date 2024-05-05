#Day 1:  
How to talk to computers.

[Introduction to QFN-48 Package, chip, pads, core, die and IPs]

Microcontroller: The image below is a standard arduino microcontroller boart with QFN-48 package.
![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/2b150472-2f50-41fc-a47f-14e5dcdcca63)
There are 3 mail components a IC :

(1)Pads  : Through which Signals  travel from external source or from Ic .

(2)Die  : Part of a silicon wafer from which IC is abricated.

(3)Core : Total area in which designed logic is fabricated.
![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/5139f36f-4e30-40de-aec9-933f62b21184)

**EDA Design Preparation Step**

To enter in to openLane we need to use flow.tcl as it will goes with the flow using the script.And by using interactive switch, we can do step by step processes.Without this intersctive switch it will run complete RTL to GDSII. now open lane has launchd and the promp is changed.

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/26444ce5-695f-4c6f-9e12-39ef59944047)  

Now all the packeges which are required are called to run the flow.

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/5e2b2311-f55c-4492-9fc8-b676376b20e2)
now we are ready to execute the command.

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/bc71338b-1648-4b4a-b185-6180631b4855)
In open lane there are nearly 30-40 example designs which and be used. for example picorv32a.v design . In this design we can see many files are available. i.e., scr, config.tcl, etc. This config.tlc file contains every details about the design. for example, details about enrollment, clock period, clock period port etc...

Now, in openlane, we are going to run the synthesis, but before synthesis, we have to prepare design setup stage. for that command is  'prep -design picorv32a'


![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/6d8737c3-3bde-4ae1-a682-c2067a7cc3d6)

Now it shows preperation is complated.

***Review files after design prep and run synthesis***

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/21199ab9-4e2b-446a-b32b-c1ee40ac0183)
'run_synthesis'

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/acacf543-67f5-42e1-a364-fe1ce7c6d9c0)

synthesis completed

***Steps to characterize synthesis results***

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/8cbf562a-1e1b-46fb-b8e2-1ed080d354de)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/1793b6ff-5771-46a5-b982-eff812118e26)



**#Day 2:** 

**Chip Floor planning **

*Utilization factor and aspect ratio*

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/292b43f9-b622-4bc7-a83a-e96d2fbffc7e)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/26170472-be38-47a3-a013-c645d93dc788)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/5965a314-ee74-40de-8693-c4e0e3f351b7)

*Power Planning*

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/904e58f6-17cc-4ba2-be4a-810c5322b2e8)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/769af649-66fc-4767-a8bd-b6e3bb23a58c)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/6aed959c-571d-44e0-b56b-dc5db18984a1)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/c289f50a-70a1-4bc5-9e96-e9de40931ee7)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/78a76d5e-a40c-4654-90cc-6619ea74a091)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/3f6c3e85-92d5-429d-9f61-ff78fb6e60a5)


**Pin placement and logical cell placement blockage**

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/9e881ac9-419e-4cb6-a19f-119fcaa7c63c)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/15969396-718e-4316-9c1a-1087d9e9d7e9)

![image](https://github.com/K-Ganesh-Rao/VSD_VLSI_Soc_design_and_planning/assets/130823089/866889bd-2cea-4b29-bbb6-adf03729c843)







