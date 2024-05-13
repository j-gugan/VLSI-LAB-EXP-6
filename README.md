# SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER, CMOS NAND and CMOS NOR USING CADENCE TOOL

# AIM:
To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

# APPARATUS REQUIRED:
 
1.Laptop with MobaXterm
2.Cadence tool


# PROCEDURE
# SCHEMATIC ENTRY:
# Creating a new library:

1.In the library manager, execute File - New library. The new library form appears.


2.In the new library form, type ‘my design lib’ in the name section.


3.In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.

4.In the next ‘technology file for new library form select option attach to an existing tech file and click ok.

5.In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.


6.After creating a new library you can verify it from the library manager.


7.If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

# Creating a schematic cell view:

1.In the CIW or library manager, execute file – new – cell viw.


2.Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.

3.Click ok when done the above setting. A black schematic window for the inverter design appears.

# Adding components to schematic:

1.In the inverter schematic window, click the instance fixed menu icon to display the add instance form.


2.Click on the browse button. This opens up a library browser from which you can select components and the symbol view.


3.After you complete the add instance form move your cursor to the schematic window and click left to place a component.

![exp 06](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/481a68a3-a5aa-42d9-85ff-bc132a2725da)


4.This is a table of components for building the inverter schematic.

5.After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.
![image](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/09af89b9-abcd-4492-90ec-494e46037143)
# Adding pins to schematic:
1.Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.

2.Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin.

![2](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/29c14cf0-1bfb-4cf1-8d22-4009b2d5e073)


Select cancel and then the schematic window enter window file or press the f bind key.

# Adding wires to schematic:

1.Click the wire (narrow) icon in the schematic window.

2.In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.

3.Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.

4.Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

# Saving the design:
	Click the check and save icon in the schematic editor window observe CIW output for any errors.

# BUILDING THE INVERTER TEST DESIGN:
# Creating the inverter test cell view:


1.In the CIW or library manager, execute file – new – cell view.

2.Setup the newfile as shown below.

3.Click ok when done. A blank schematic window for the inverter test design appears.

4.Using the components list and properties/ comments in this table build the inverter test schematic.

![3](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/00fc1aff-67a8-4c28-9eee-3701583a65c4)


5.Add the above components using create – instance or by pressing I.

6.Click the wire (narrow) icon and wire your schematic.

7.Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.

8.Click on the check and save icon to save the design.

![4](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/28d95774-8da9-47e3-b726-3e1b69fc4ca3)
# ANALOG SIMULATION WITH SPECTRA:
# Starting the simulation environment:
   1.In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears.
   
# Choosing a simulator:

1.In the simulation window (ADE) execute setup – simulator / directory / host.

2.In the choosing simulator form, set the simulator field to specra and click ok.

3.In the simulation window (ADE) execute the setup model libraries.

To complete, move the cursor and click ok.
# Choosing Analysis:
1.Click the choose- Analysis icon in the simulation window (ADE).
  
2.The choosing analysis form appears.

3.To Setup the transient analysis.

    a.In the analysis section select tron.

    b.Set the stop time as 100ns

    c.Click at the moderate or enabled button and the bottom and then click apply.

3.To set for DC analysis

    a.In the analysis section select DC.

    b.Turn on save DC operating point.

    c.Turn on the component parameters.

    d.Double click the select Vpulse source or Type V0 (capital V zero).


    e.Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8.


    f.Select the enable button and click apply and then click ok.

# Selecting output for plotting:
1.Execute the o/p’s to be plotted  -select on sschematic in the simulation window.

2.Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

# Running the simulation:
1.Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.

2.When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.
![5](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/74d98fc4-a754-4179-8a76-debb53da0e01)
![6](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/2e73e6ae-774c-4bd0-b982-9d2bb6b7da50)
# CMOS NAND GATE
# NAND SCHEMATIC
![7](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/bd4faacf-de41-4db3-9dea-c512d262820d)
# NAND TEST CELL VIEW
![8](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/2490772a-95d1-461b-ab7f-596d3a3a41f7)
# NAND SIMULATION WITH SPECTRA
![9](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/d0ad22f6-5a5f-4d50-91f9-80fb819fc8b7)

# CMOS NOR GATE
# NOR SCHEMATIC
![10](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/238b06df-6801-43bc-b4dd-63fa30df2115)
# NOR TEST CELL VIEW
![11](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/fd1a7122-1e3b-4152-8a76-35eb2c05aa16)
# NOR SIMULATION WITH SPECTRA
![12](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/163828735/2ae1a5c0-eebc-403f-b7a5-b86b2fcad7d3)

# RESULT
Thus, the CMOS INVERTER, CMOS NAND and CMOS NOR using Cadence tool was simulated and designed.




