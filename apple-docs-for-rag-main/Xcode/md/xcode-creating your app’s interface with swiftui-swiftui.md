

- Xcode
-  Creating your app’s interface with SwiftUI 

Article

# Creating your app’s interface with SwiftUI

Develop apps in SwiftUI with an interactive preview that keeps the code and layout in sync.

## Overview

If you choose the SwiftUI framework to develop your app, you can see an interactive preview as you lay out your user interface. Xcode keeps the changes you make to the source code, the user interface layout, and the inspector in sync. For example, when you edit attributes in the inspector, Xcode adds the corresponding code to the source file.

### Display the SwiftUI preview

To show the preview, select a file that uses SwiftUI in the project navigator, and choose Editor \> Canvas. Then click the Resume button in the upper-right corner of the canvas to start the preview. Xcode builds and runs the code, displaying the results directly in the canvas.

Use the controls at the bottom of the preview to run the app on a simulated device in the canvas, with or without a debug session, or run the app on a connected device.

### Add views and modifiers

To add views and modifiers to your app, click the Library button (+) in the toolbar to open the library, then drag user interface elements from the library to either the canvas or source code. Regardless of where you drop the elements, Xcode keeps the source code and the layout in sync.

### Edit user interface elements

Edit element attributes using either the Action menu or the inspector, or by entering code in the source editor. Command-click the element in the canvas or the structure in the code, choose Show SwiftUI Inspector from the Action menu, then change the attributes in the next pane. Alternatively, choose View \> Inspectors \> Show Attributes Inspector, and change the attributes in the Attributes inspector that appears on the right.

### Embed user interface elements

Additionally, you can modify the user interface by embedding elements in other structures. Command-click an element in the source code or in the canvas, then choose an “Embed in \[Generic Structure\]” action from the pop-up menu. For example, choose “Embed in HStack” to embed an element that arranges a view’s children in a horizontal line.

To learn more about SwiftUI, go to Introducing SwiftUI.

## See Also

### Essentials

Creating an Xcode project for an app

Start developing your app by creating an Xcode project from a template.

Previewing your app’s interface in Xcode

Iterate designs quickly and preview your apps’ displays across different Apple devices.

Building and running an app

Compile your source files and assemble an app bundle to run on a device or simulator.

Xcode updates

Learn about important changes to Xcode.

