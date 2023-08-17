
## Painting Flat Surfaces using the AMS Paint Tool for Bambu Labs 3D Printers

These instructions will guide you through the process of preparing and painting flat surfaces using the AMS Paint Tool for Bambu Labs 3D Printers.

### Prerequisites:

- A 3D model of a blank plate for a Raspberry Pi. [Download Blank Plate Model](link_to_file)
- A DXF or SVG file of your desired design.
- Fusion 360 software.
- Bambu Labs 3D Printer with AMS Paint Tool.

### Steps:

1. **Import DXF/SVG File:**
   - Open your Fusion 360 project.
   - Import the DXF or SVG file of your design.
   ![Step 1](https://github.com/ItalianSquirel/ItalianSquirel.github.io/blob/master/assets/BambuPaint/step1.png?raw=true)

2. **Extrude and Tiny Gap:**
   - Select the imported design.
   - Extrude the design to a height that's just slightly above the printer's minimal printable height, such as 0.001 mm.
   - Ensure that there's a tiny gap between the extruded surface and the original surface.
   ![Step 2](https://github.com/ItalianSquirel/ItalianSquirel.github.io/blob/master/assets/BambuPaint/step2.png?raw=true)

3. **Save and Export:**
   - Save your Fusion 360 project.
   - Export the modified design as an STL file.
   ![Step 3](https://github.com/ItalianSquirel/ItalianSquirel.github.io/blob/master/assets/BambuPaint/step3.png?raw=true)

4. **Load STL in Bambu Slicer:**
   - Open the Bambu Slicer software.
   - Load the STL file of your modified design.

5. **Prepare for Painting:**
   - In Bambu Slicer, the modified face should be recognized as a new surface due to the tiny gap.
   - Use the fill tool to ensure the new surface is sealed and ready for painting.
   ![Step 4](https://github.com/ItalianSquirel/ItalianSquirel.github.io/blob/master/assets/BambuPaint/step4.png?raw=true)

6. **Color Selection and Painting:**
   - Choose the desired colors for your design.
   - Use the AMS Paint Tool to apply colors to the prepared surface.
   ![Step 5](https://github.com/ItalianSquirel/ItalianSquirel.github.io/blob/master/assets/BambuPaint/step5.png?raw=true)

7. **Preview and Adjust:**
   - Preview the painted design in the Bambu Slicer.
   - Make any necessary adjustments to colors or placement.

8. **Print:**
   - Once you are satisfied with the painted design, initiate the printing process using your Bambu Labs 3D Printer.
   ![Step 7](https://github.com/ItalianSquirel/ItalianSquirel.github.io/blob/master/assets/BambuPaint/step6.jpg?raw=true)

### Notes:

- The small extruded height with a tiny gap is a workaround to allow the slicer to recognize the new face while being mindful of the printer's capabilities.
- Experiment with different colors and patterns in the AMS Paint Tool to achieve your desired look.
- Double-check the preview in the Bambu Slicer before printing to avoid any issues.