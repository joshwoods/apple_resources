

- RealityKit
- Reality Composer
-  Adding elements to a 3D scene 

Article

# Adding elements to a 3D scene

Add assets to your scene from Reality Composer’s library, or import custom assets.

## Overview

To build a scene in *Reality Composer*, you import assets from usdz or Reality files, or select them from Reality Composer’s extensive library of configurable 3D objects you can customize by changing parameter values in the Properties inspector. Once the assets are in your scene, you can move, rotate, and scale them relative to the scene’s anchor guides. For more information about manipulating assets you’ve added to your scene, see Arranging elements in a scene.

### Add a library asset

To add an asset from *Reality Composer*’s Object library, click or tap the plus button (+) in the toolbar to bring up the library popover, then drag the object you want into your scene view to place it.

Every library asset has a different set of parameters that you can change to alter its appearance. Although certain parameter sections, such as Transform and Physics, are available for all assets, most are available only when they make sense for the selected object. The clock asset, for example, lets you specify a time to display in the inspector, but other assets do not.

### Import a custom 3D asset from a file

To import your own custom assets into a scene, use the Import button in the library popover, then navigate to a usdz or Reality file containing the asset you wish to import. On the Mac, you can also drag usdz or Reality files onto your Reality Composer project or select Import from the File menu.

The asset contained in the selected file is imported into your project and added to the current scene. Imported assets are available in Reality Composer’s library whenever you’re working with this project.

### Create a chart from a data source

Reality Composer’s library contains two chart assets: a pie chart and a bar chart. In addition to requiring you to provide parameter values for configuring their appearance, these two chart objects also require you to provide a data source in the form of a comma-separated values (CSV) file containing the data to be charted.

The CSV file requires two pieces of data for each item in the graph: a label and a numeric value. Your CSV file can represent the data you’re charting in columns or rows, and you can choose to include or exclude headers.

If you tap or click a chart object in your scene, the Property inspector shows a button for importing a data source. Click or tap that button and select your CSV file. The chart then automatically updates to reflect the labels and values contained in the imported file.

## See Also

### Scene creation

Creating 3D Content with Reality Composer

Assemble assets into a dynamic 3D composition that you can add to a scene in your app, or share with AR Quick Look.

Loading Reality Composer files using generated code

Leverage automatically generated code to load scenes from Xcode.

Loading Reality Composer files manually without generated code

Load Reality Composer files that aren’t part of your Xcode project.

Configuring elements in a scene

Define the appearance and behavior of objects in a scene.

Arranging elements in a scene

Manipulate objects to complete your Reality Composer scene.

Manipulating Reality Composer scenes from code

Make programmatic changes to your scenes at runtime.

Adding procedural assets to a scene

Create procedurally generated shape primitives to your Reality Composer scene.

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

