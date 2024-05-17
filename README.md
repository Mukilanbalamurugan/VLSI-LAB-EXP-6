# SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL

**AIM:**

To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

**APPARATUS REQUIRED:**
 
1.	Laptop with MobaXterm
2.	Cadence tool
	
**PROCEDURE**

**CREATING A NEW LIBRARY:**
1.	In the library manager, execute File - New library. The new library form appears.
2.	In the new library form, type ‘my design lib’ in the name section.
3.	In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
4.	In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
5.	In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
6.	After creating a new library you can verify it from the library manager.
7.	If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

**CREATING A SCHEMATIC CELL VIEW:**

1.	In the CIW or library manager, execute file – new – cell viw.
2.	Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
3.	Click ok when done the above setting. A black schematic window for the inverter design appears.

**ADDING COMPONENTS TO SCHEMATIC:**

1.	In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
2.	Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
3.	After you complete the add instance form move your cursor to the schematic window and click left to place a component.
4.	This is a table of components for building the inverter schematic.
5.	After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.


**ADDING PINS TO SCHEMATIC:**

1.	Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
2.	Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin.
3.	Select cancel and then the schematic window enter window file or press the f bind key.
   
**ADDING WIRES TO SCHEMATIC:**

1.	Click the wire (narrow) icon in the schematic window.
2.	In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
3.	Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
4.	Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

Saving the design:
	Click the check and save icon in the schematic editor window observe CIW output for any errors.

**BUILDING THE INVERTER TEST DESIGN:**

Creating the inverter test cell view:
1.	In the CIW or library manager, execute file – new – cell view.
2.	Setup the newfile as shown below.
3.	Click ok when done. A blank schematic window for the inverter test design appears.
4.	Using the components list and properties/ comments in this table build the inverter test schematic.
5.	Add the above components using create – instance or by pressing I.
6.	Click the wire (narrow) icon and wire your schematic.
7.	Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
8.	Click on the check and save icon to save the design.
 


**ANALOG SIMULATION WITH SPECTRA:**

Starting the simulation environment:
1.	In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears.
Choosing a simulator:
1.	In the simulation window (ADE) execute setup – simulator / directory / host.
2.	In the choosing simulator form, set the simulator field to specra and click ok.
3.	In the simulation window (ADE) execute the setup model libraries.
To complete, move the cursor and click ok.
Choosing Analysis:
1.	Click the choose- Analysis icon in the simulation window (ADE).
2.	The choosing analysis form appears.
3.	To Setup the transient analysis.
a.	In the analysis section select tron.
b.	Set the stop time as 100ns
c.	Click at the moderate or enabled button and the bottom and then click apply.
4.	To set for DC analysis
a.	In the analysis section select DC.
b.	Turn on save DC operating point.
c.	Turn on the component parameters.
d.	Double click the select Vpulse source or Type V0 (capital V zero).
e.	Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8.
f.	Select the enable button and click apply and then click ok.

**SELECTING OUTPUT FOR PLOTTING:**

1.	Execute the o/p’s to be plotted  -select on sschematic in the simulation window.
2.	Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

**RUNNING THE SIMULATION:**

1.	Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
2.	When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.
 
**CMOS INVERTER:**

**CMOS INVERTER SCHEMATIC:**

![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/d0f02630-9717-48b0-9304-7d17065b68e8)

**SPECIFICATIONS**

Vpulse 	V1 = 0	Vdc	= 1
V2 = 1
td = 0,tr=tf=1 n, ton= 100n ,T=200n

**SIMULATION SETTINGS:**

Setup for transient analysis:
1.	Stop time =400n

Setup for D.C analysis
1.	Component to be selected in schematic is	for d.c analysis
2.	Start = -1 Stop = 1 resp.


**CMOS INVERTER TEST CELL VIEW:**

![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/c0051703-49e7-4500-a3eb-c4c97dd06556)

**CMOS INVERTER SIMULATION WITH SPECTRA:**

**TRANSIENT RESPONSE:**
![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/f225fe71-8103-4302-9a0f-18fd9025adcd)

**DC RESPONSE:**

![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/8344e704-c6c7-4b31-960a-a7ddb540a24a)


**CMOS NAND GATE:**

**NAND SCHEMATIC:**

 ![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/01f8be1e-3fc8-4c50-b831-847484cae7c5)


**NAND TEST CELL VIEW:**

 ![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/5ab06930-975d-4a8a-94b1-72754300f72d)


**NAND SIMULATION WITH SPECTRA:**
 
![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/9a392d71-2442-4cea-a3ca-e70d5d68f685)

**CMOS NOR GATE:**

**NOR SCHEMATIC:**

![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/13aa23eb-47f4-4879-acc6-d8b8e0240cfc)


**NOR TEST CELL VIEW:**

![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/8989c1dc-d30a-49d9-b92f-26249f0a7451)

**NOR SIMULATION WITH SPECTRA:**

![image](https://github.com/Nandhak23/VLSI-LAB-EXP-6/assets/160568515/bdf535bd-2c8e-41e8-8cdb-7f2fe17e22dc)


**RESULT:**

The Implementation of CMOS inverter, CMOS NAND and CMOS NOR gate waveforms are verified.
