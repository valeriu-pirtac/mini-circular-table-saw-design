# mini-circular-table-saw-design

MIni circular table saw DIY design project

For an electrical mini circular table saw project, a structured approach is essential for organization, safety, and potential future modifications. This project can be broken down into three main categories: mechanical, electrical, and documentation. Each component should be planned as a separate module, allowing for easier design, fabrication, and troubleshooting.

## Project folder structure template

A project folder is the first step toward creating an organized workflow, separating different elements into their own subdirectories.

```
/mini_table_saw
├── /cad_design
│   ├── /parts
│   │   ├── base_frame.FCStd
│   │   ├── blade_arbor.FCStd
│   │   ├── motor_mount.FCStd
│   │   └── fence.FCStd
│   ├── /assemblies
│   │   ├── saw_assembly.FCStd
│   │   └── full_assembly.FCStd
│   └── /drawings
│       ├── fence_drawing.FCStd
│       └── saw_assembly_drawing.FCStd
├── /electrical
│   ├── wiring_diagram.pdf
│   ├── motor_datasheet.pdf
│   └── switch_box_design.FCStd
├── /prototyping
│   ├── /cnc
│   └── /3d_printing
├── /documentation
│   ├── bill_of_materials.xlsx
│   └── build_log.md
└── /research
    ├── reference_images.zip
    └── reference_tutorials.txt
```
## FreeCAD file structure: Mechanical design

This modular approach isolates individual components in their own FreeCAD files, making them easier to manage. 

### /parts/

Create a separate `.FCStd` file for each individual, non-standard component you are designing, such as custom brackets or the table saw's frame. 

- `base_frame.FCStd`: The file for the saw's main chassis or housing.
- `motor_mount.FCStd`: The file for the custom bracket holding the motor and arbor.
- `fence.FCStd`: The file for the adjustable guide for making cuts. 

### /assemblies/

This directory holds the final assembly files where you use the Assembly4 workbench to join the parts together. 

- `saw_assembly.FCStd`: An assembly file combining the motor, motor mount, and blade arbor.
- `full_assembly.FCStd`: The final, top-level assembly file combining all the parts and sub-assemblies.

### /drawings/

Technical drawings of critical components for manufacturing can be placed here, using the TechDraw workbench.

## Electrical component management

Since FreeCAD primarily focuses on mechanical design, use external files to manage the electrical aspects of the project. 

### /electrical/

This directory stores documentation for the electrical system. 
wiring_diagram.pdf: A schematic diagram showing how the power switch, motor, and power source are connected.

- `motor_datasheet.pdf`: Technical specifications for the motor you are using.
- `switch_box_design.FCStd`: If you design a custom enclosure for the electrical switch and wires, this is where you would store the FreeCAD model.

## General project management and documentation

These elements keep the project on track and organized, which is crucial for any build.

### /documentation/

This folder stores all the non-CAD information necessary for the project.

- `bill_of_materials.xlsx`: A spreadsheet listing all the parts, both custom and off-the-shelf, with quantities, costs, and suppliers.
- `build_log.md`: A text file (like a .md or .txt file) where you track your progress, note challenges, and jot down ideas. 

### /research/

Store inspiration and reference materials here.

- `reference_tutorials.txt`: A file with links to helpful YouTube videos, websites, or other tutorials you find.
- `reference_images.zip`: A compressed folder of images you've collected from other projects for inspiration.