

- Xcode
-  Creating an Xcode project for an app 

Article

# Creating an Xcode project for an app

Start developing your app by creating an Xcode project from a template.

## Overview

To create an Xcode project for your app, choose a template for the platform on which your app will run, and select the type of app you wish to develop, such as a single view, game, or document-based for iOS. Xcode templates include essential project configuration and files that help you start developing your app quickly.

### Prepare configuration information

Before you create a project, collect the information that Xcode needs to identify your app and you as a developer:

- **Product name.** The name of your app as it will appear in the App Store and appear on a device when installed. The product name must be at least 2 characters and no more than 255 bytes, and should be similar to the app name that you enter later in App Store Connect.

- **Organization identifier.** A reverse DNS string that uniquely identifies your organization. If you don’t have a company identifier, use `com.example.` followed by your organization name, and replace it before you distribute your app.

- **Organization name.** The name that appears in boilerplate text throughout your project folder. For example, the source and header file copyright strings contain the organization name. The organization name in your project isn’t the same as the organization name that appears in the App Store.

Important

The organization identifier is part of the bundle ID (CFBundleIdentifier) by default. Xcode uses the bundle ID to register an App ID when you first run your app on a device. The number of App IDs are limited if you are not a member of the Apple Developer Program, and you can’t change the App ID after you upload a build to App Store Connect, so choose the organization identifier carefully.

### Create a project

Launch Xcode, then click “Create a new Xcode project” in the Welcome to Xcode window or choose File \> New \> Project. In the sheet that appears, select the target operating system or platform and a template under Application. In the following sheets, fill out the forms and choose options to configure your project.

You must provide a *product name* and *organization identifier* because they are used to create the *bundle identifier* that identifies your app throughout the system. Also enter an *organization name*. If you don’t belong to an organization, enter your name.

To develop for all platforms and see an interactive preview of your layout, choose SwiftUI as the user interface before you click Next on this sheet.

### Manage files in the main window

When you create a project or open an existing project, the *main window* appears, showing the necessary files and resources for developing your app.

You can access different parts of your project from the *navigator area* in the main window. Use the *project navigator* to select files you want to edit in the *editor area*. For example, when you select a Swift file in the project navigator, the file opens in the *source editor,* where you can modify the code and set breakpoints.

Details about the selected file also appear in the *inspector area* on the right. In the inspector area, you can select the Attributes inspector to edit properties of a file or user interface element. If you want to hide the inspector to make more room for the editor, click the “Hide or show the Inspectors” button in the upper-right corner of the toolbar.

You use the *toolbar* to build and run your app on a simulated or real device. For iOS apps, choose the app target and a simulator or device from the run destination menu in the toolbar, then click the Run button.

For macOS apps, just click the Run button. When your app launches, the *debug area* opens, where you can control the execution of your app and inspect variables. When the app stops at the breakpoint, use the controls in the debug area to step through the code or continue execution. When you are done running the app, click the Stop button in the toolbar.

If you use SwiftUI, you can see an interactive preview of the user interface while you create your app. Xcode keeps the changes you make in the source file, the canvas on the right, and the inspector in sync. You can use the controls in the preview to run the app with the debugger, too. For details, see Creating your app’s interface with SwiftUI.

To change properties you entered when creating your project, select the project name in the project navigator that appears at the top, then the *project editor* opens in the editor area. Most of the properties you entered appear on the *General pane* of the project editor.

## See Also

### Essentials

Creating your app’s interface with SwiftUI

Develop apps in SwiftUI with an interactive preview that keeps the code and layout in sync.

Previewing your app’s interface in Xcode

Iterate designs quickly and preview your apps’ displays across different Apple devices.

Building and running an app

Compile your source files and assemble an app bundle to run on a device or simulator.

Xcode updates

Learn about important changes to Xcode.

