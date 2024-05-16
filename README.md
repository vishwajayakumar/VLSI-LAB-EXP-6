**6.SCHEMATIC ENTRY AND SIMULATION OF CMOS INVERTER,CMOS NAND and CMOS NOR USING CADENCE TOOL**

**AIM:**

To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

**APPARATUS REQUIRED:**

Laptop with MobaXterm
Cadence tool

**PROCEDURE:**

**CREATING A NEW LIBRARY:**

1.In the library manager, execute File - New library. The new library form appears.

2.In the new library form, type ‘my design lib’ in the name section.

3.In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.

4.In the next ‘technology file for new library form select option attach to an existing tech file and click ok.

5.In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.

6.After creating a new library you can verify it from the library manager.

7.If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

**CREATING A SCHEMATIC CELL VIEW:**

1.In the CIW or library manager, execute file – new – cell view.

2.Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.

3.Click ok when done the above setting. A black schematic window for the inverter design appears.

**ADDING COMPONENTS TO SCHEMATIC:**

1.In the inverter schematic window, click the instance fixed menu icon to display the add instance form.

2.Click on the browse button. This opens up a library browser from which you can select components and the symbol view.

3.After you complete the add instance form move your cursor to the schematic window and click left to place a component.

4.This is a table of components for building the inverter schematic.

5.After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.

**ADDING PINS TO SCHEMATIC:**

1/Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.

2.Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin.

3.Select cancel and then the schematic window enter window file or press the f bind key.

**ADDING WIRES TO SCHEMATIC:**

1.Click the wire (narrow) icon in the schematic window.

2.In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.

3.Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

Saving the design: Click the check and save icon in the schematic editor window observe CIW output for any errors.

**BUILDING THE INVERTER TEST DESIGN:**

Creating the inverter test cell view:

1.In the CIW or library manager, execute file – new – cell view.

2.Setup the newfile as shown below.

3.Click ok when done. A blank schematic window for the inverter test design appears.

4.Using the components list and properties/ comments in this table build the inverter test schematic.

5.Add the above components using create – instance or by pressing I.

6.Click the wire (narrow) icon and wire your schematic.

7.Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.

8.Click on the check and save icon to save the design.

**ANALOG SIMULATION WITH SPECTRA:**

Starting the simulation environment:

1/In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:

2.In the simulation window (ADE) execute setup – simulator / directory / host.

3.In the choosing simulator form, set the simulator field to specra and click ok.

4.In the simulation window (ADE) execute the setup model libraries. To complete, move the 5.cursor and click ok. Choosing Analysis:

6.Click the choose- Analysis icon in the simulation window (ADE).
The choosing analysis form appears.

7.To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.

8.To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.

**SELECTING OUTPUT FOR PLOTTING:**

1.Execute the o/p’s to be plotted -select on sschematic in the simulation window.

2.Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

**RUNNING THE SIMULATION:**

1.Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.

2.When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.

**CMOS INVERTER:**

**CMOS INVERTER SCHEMATIC:**

![330388633-a490dfb2-234a-4d31-a932-e07d29eb8bb2](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/7b241f18-eef6-4fb7-bd7c-6c799d87e2b2)

**SPECIFICATIONS**

Vpulse V1 = 0 Vdc = 1 V2 = 1 td = 0,tr=tf=1 n, ton= 100n ,T=200n

**SIMULATION SETTINGS:**

Setup for transient analysis:

Stop time =400n
Setup for D.C analysis

Component to be selected in schematic is for d.c analysis
Start = -1 Stop = 1 resp.

**CMOS INVERTER TEST CELL VIEW:**

![330387481-4efd0030-64ad-4cbb-8723-3a89a9b53117](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/c4988275-bb13-4541-b9e6-f6340442e5a3)


**CMOS INVERTER SIMULATION WITH SPECTRA:**

**TRANSIENT RESPONSE:**

![330387548-99f63f38-f5d2-4b16-a103-c38b3ad8d027](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/08bd6097-ca67-4f25-be48-69a2b5b7547a)

**DC RESPONSE:**

![330387581-941a021f-244a-460d-900d-e882e8f14671](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/67be9b5f-48a7-4b8a-9b3d-301082a62c82)

**CMOS NAND GATE:**

**NAND SCHEMATIC:**

![330387674-ca872dcb-05be-40ec-b566-7eaa804a5c96](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/c199c64e-1545-4fd3-9750-2fcf4d864be0)



**NAND TEST CELL VIEW:**

![330387730-b2b5b7e8-40d1-419b-9c96-477b105fc9f6](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/57b65a3e-2ca9-48f4-a0f0-7d05285fca9e)


**NAND SIMULATION WITH SPECTRA:**

![330387771-0a8f3246-1a76-4f3a-9667-4b5df40df977](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/21ecf6a1-a312-40e2-8e00-7ec935099443)


**CMOS NOR GATE:**

**NOR SCHEMATIC:**

![330387840-5cad3e7e-6513-4444-a8e3-5cfbb8dd4f56](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/8892637a-7b16-4edf-bc43-4782768d4d36)



**NOR TEST CELL VIEW:**

![330387869-1e716a28-49f4-4ad0-a8bc-713b82779e7b](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/7b19b7ab-e240-47e9-a81b-56209cbd8a75)

**NOR SIMULATION WITH SPECTRA:**

![330387901-c5b18e7f-cf0d-46f8-8c69-5d915788deb9](https://github.com/vishwajayakumar/VLSI-LAB-EXP-6/assets/169515345/2aecc60b-9ed2-4569-925d-5b9447fb9f47)



**RESULT:**

The Implementation of CMOS inverter, CMOS NAND and CMOS NOR gate waveforms are verified.
