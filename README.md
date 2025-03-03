Functionalities:

* Wi-Fi and BLE communication via ESP32
* IMU 6-axis BMI085 for motion sensing
* DRV2605L for haptic feedback
* LiPo battery with MCP73831 charging circuit
* USB-C port for programming and charging
* 1.28-inch LCD display, 240x240 pixels for visual output
* Electronics must fit into the provided case

(All datasheets and schematics are in the Components folder)

Constraints:

* No straight angles in traces.
* Power traces must meet the required dimensions.
* Decoupling capacitors (100nF) should be placed as close as possible to the power pins of modules and ICs.
* For double-sided boards, avoid vias in power traces.
* Main components should be placed according to the mechanical dimension and placement document.
* Power traces (VCC, VUSB, VBUS, 3V3, etc.) should have a width of 0.3mm, and data signals at least 0.125mm.
* The ESP32 antenna should be placed toward the PCB edge, with the PCB cutout beneath it.


Notes and Recommendations:

* Use SMD resistors and capacitors in 0402 package, unless specified otherwise (e.g., 0603, tantalum).
* Component placement should be on the TOP layer (except for test pads, SD card socket, LCD connector, and NOR Flash).
* Routing can be on both top and bottom layers. If using two layers, ensure the ground plane is appropriately designed.
* For DRC checks, load the verification file from the provided archive.
* Apply Via Stitching between the two ground planes, especially near the ESP32 module.
* Ignore "Only INPUT pins on NET ID" error.
* Do not route signals under the ESP32 antenna; the area beneath it must be cut out to minimize interference.
* Errors due to button, header, and USB port placement are disregarded.
* Test pads should be placed only on the back of the PCB, clearly marked in silkscreen with signal names.
* Use the provided library ([hector_watch.zip file]) for component symbols and footprints, except for:
    - Buttons ([button.pdf file])
    - LCD connector (draw your own footprints based on the LCD datasheet).

Files:

* Schematics: Schematics.zip file
* DRC check: DRC_check.zip file
* PCB Dimensions & Placement: [dimensions.pdf file]

Additional Notes:

* The recommended PCB dimensions and component placement can be found in the [dimensions.pdf file], with all measurements in mm.
* The placement is just a recommendation to ensure the PCB buttons align with the physical buttons on the case.
* You are free to modify the placement, as long as you also adjust the case.
* Additionally, modify the case to allow access to the SD card and USB-C port if they do not align properly.
