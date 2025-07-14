

- RealityKit
- USD Assets
-  Exporting a Reality Composer Scene to USDZ 

Article

# Exporting a Reality Composer Scene to USDZ

Save a scene or project as USDZ to read, collect, or display in an app or website.

## Overview

Export a scene or project from Reality Composer as USDZ to display it in an AR or 3D app. You can also preview a USDZ file in an AR app or website using AR Quick Look. Because USDZ is a universal file format, you can open a USDZ file in third-party tools that support it and make changes to your scene or project.

### Enable the export preference

To enable USDZ exports, open Reality Composer’s Preferences menu and check the “Enable USDZ export” option under Content.

### Create a USDZ File

From within an open Reality Composer project, choose the File menu \> Export option.

In the export sheet, choose whether to export the scene or project in USDZ format and click the Export button.

Note

Reality Composer doesn’t support exporting a scene that contains reimported `.reality` files.

### Accommodate the custom USD schema and provide feedback

Reality Composer extends the USD specification to include most of the features that `.reality` or `.rcproject` files support, such as anchors, behaviors, and physics. Because these features aren’t available in the current USD specification, Reality Composer’s USDZ exports provide more functionality on Apple devices than USD files created with third-party tools. For more information about Apple’s custom USD schemas, see USDZ schemas for AR.

Note

USDZ exports support horizontal, vertical, image, and face anchors. Apple’s custom USD schema doesn’t support object anchors.

Some or all of the functionality enabled by these custom schemas may eventually funnel into the USD specification itself. To provide feedback on these schemas, use the Feedback Assistant.

## See Also

### Essentials

USDZ schemas for AR

Add augmented reality functionality to your 3D content using USDZ schemas.

Creating USD files for Apple devices

Generate 3D assets that render as expected.

