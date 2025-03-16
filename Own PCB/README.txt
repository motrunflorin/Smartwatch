for the power traces (3V3), I maintained a width of 0.3 mm, while the rest have 0.127 mm;
!! correction: due to files not being saved properly, I had sync errors between schematics and PCB, and I had to delete the 3V3 traces and modify them with a width of 0.127 mm;

I couldn't group the test pads in a regular shape, and the TX test pad is not in the grouping in order to connect it to the corresponding pin;
(initially, I designed the test pad arrangement as three distinct groups, placed as strategically as possible near the pins they needed to be connected to, in order to have the most optimal traces);

the 100 nF decoupling capacitors were placed as close as possible to the power supply pins;

the main components were placed according to the specifications in the dimensions document, with almost negligible errors, on the order of 10^-3 mm;

the ESP32 module's antenna was placed towards the outer edge of the PCB, and the PCB was cut out as precisely as possible under the antenna;

the test pads, the SD card socket, the LCD connector, and the NOR Flash circuit were placed on the Top layer;

the footprints for the buttons and the LCD display connector were made according to the datasheet;

I tried as much as possible to keep all the component groupings from the schematics together, such as the diode grouping, for example;

I also tried to position the components as close as possible to their corresponding connections from the schematics to the PCB, such as the R1-USB resistor of the USB4110-GF-A module;

ERRORS: resistors R11 and R9 were not connected as I couldn't find a viable trace;

silkscreen was done for the test pads with a width of 0.4 mm.
