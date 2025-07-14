

- RealityKit
- Reality Composer
-  Creating 3D Content with Reality Composer 

# Creating 3D Content with Reality Composer

Assemble assets into a dynamic 3D composition that you can add to a scene in your app, or share with AR Quick Look.

## Overview

Apple’s Reality Composer app gives you an intuitive interface for constructing 3D compositions and augmented reality (AR) experiences. You combine 3D models, audio, and other assets—along with a description of how these objects behave—into a file that you add to your RealityKit-enabled app. You can also export your composition as a lightweight AR Quick Look experience that lets users place and preview content.

You start by choosing the kind of real-world object that should anchor your scene, like a horizontal surface or the user’s face. Then position virtual elements within your scene. Choose from Reality Composer’s large collection of customizable assets, or import your own in usdz format. Add animations and sound triggered by events like user taps, as well as behaviors driven by physics simulation.

If you compose on a Mac, you can synchronize your composition with Reality Composer on an iOS device to try it in an AR session. Alternatively, compose directly on the iOS device. Either way, you use the RealityKit framework in your app to load, simulate, and render the composition.

### Get the reality composer app

You automatically get Reality Composer for macOS when you install Xcode 11 or later. The app is one of the developer tools bundled with Xcode. From the menu, choose Xcode \> Open Developer Tool, and select Reality Composer.

To get Reality Composer for iOS, request access to the beta version from the Apple Developer download page.

### Anchor your composition to something in the real world

The first time you open the app, or when you start a new project with the File \> New menu option, Reality Composer prompts you to choose an anchor:

An anchor is the real-world reference around which you build your composition. When a user later interacts with a scene in an AR app, ARKit looks for a real-world item that matches your anchor, and attaches your scene to that.

Pinning content to a particular point in space creates the illusion that your content is part of the real world. By choosing an appropriate anchor, you ensure that users position your content in a sensible way. For example, to create a scene that’s meant to exist on a table top, like a collection of wooden blocks, choose a horizontal plane. That way, the items that you add to the scene appear to rest on the table.

For more information about anchoring your scenes, see Selecting an anchor for a Reality Composer scene

### Add content to your composition

You build a composition by adding, positioning, and configuring 3D objects. If you have assets from an artist in usdz format, you can drag them directly onto the project canvas. Alternatively, Reality Composer offers a large selection of highly configurable objects that you can use freely in your projects.

To add a built-in object, like the simple cube that appears by default in a new project as shown in the figure above, click the Objects button, and double-click or drag an item from the popup onto your canvas.

In some cases, you may first need to download the group of objects by clicking the cloud icon that appears alongside the name of the group.

To configure an object, select it, and if the settings pane isn’t already open, click the Settings button in the Toolbar. The Look panel exposes the available parameters for the selected object. For some objects, you choose a material, along with other object-specific configuration. For example, you can change the default cube to be aluminum with a 1-centimeter bevel radius.

For other objects, you choose between styles like realistic, stylized, and iconic.

Move objects by dragging them around the canvas with your mouse, or dragging them with your finger on an iOS device. You can similarly drag the entire canvas to reposition the view. To focus the view on a particular part of the scene, use the Frame button in the Toolbar to focus on the selected object, or on the scene as a whole.

Name the scene so that you can refer to it after you import the project into Xcode. As shown above, the Name field in the setting pane applies to the entire scene when no objects are selected. Optionally, you can also name individual objects to help you find them inside the scene. Select the object you want to name, and using the same Name field, provide a string that’s unique within the composition to make it easy to find.

For more detailed information about creating Reality Composer scenes, see Adding elements to a 3D scene.

### Trigger movement and sound with behaviors

Add behaviors to your composition to enable animations and sound effects that react to events in the environment, like the user tapping an object or moving close to it. Click the Behaviors button in the Toolbar to reveal the Behaviors pane at the bottom of the composition window, and then click the plus button.

From the popup, choose a behavior like Tap & Flip.

This adds a new tap trigger and flip action, both of which you can configure. For example, you can change the object that reacts to the tap, or the object that does the flipping. You can also change aspects of the animation, like duration and style.

To preview an individual action, click the Play button on that action. To preview the entire sequence, click the Play button on the action sequence.

Add more actions by clicking the action sequence Plus button. New actions occur sequentially by default, but you can make actions occur simultaneously by dragging one onto the other.

### See your content in the real world

Reality Composer lets you focus on your composition while you design it. You work on a blank canvas and move around the composition freely, viewing it from any angle as you place assets and add behaviors. But eventually, you need to see how your composition looks in the real world.

To do this, run Reality Composer on an iPad or iPhone that supports ARKit. If you compose on a Mac, you can synchronize your session between the Mac and an iOS device over a local area network connection. Make sure Reality Composer is running on the device, and then click the Edit on iOS button in the Toolbar on your Mac. Select the iOS device from the list of devices that appear.

From the iPad or iPhone, you can preview your composition in an augmented reality session. Find an anchor in the real world that matches your composition’s anchor, and attach your entity to it. You then physically move the device around the virtual object as you would in any AR session, observing how your composition looks in a real-world setting. You can also trigger behaviors from this mode to see how they perform.

You can even continue to edit your composition while running an AR session.

### Add the composition to your app

After you finish your composition, you can add it to your RealityKit-enabled app. Save the composition as an `.rcproject` file by clicking File \> Save in the menu. Drag this file directly into the navigation pane of your Xcode project.

Xcode automatically generates code that you use to manipulate the stored objects. For example, Xcode generates a class for the scene based on the scene’s name (`MyGreatScene`) inside an enumeration based on the name of the project file (`MyProject.rcproject`). As a convenience, it also provides a `loadMyGreatScene()` method:

```
public enum MyProject {
    public class MyGreatScene: Entity, HasAnchoring { ... }
    public static func loadMyGreatScene() throws -> MyGreatScene { ... }
    ...
}
```

In your code, you call the load method to get the Reality Composer scene’s anchor. You then add the anchor to your AR view (ARView) scene’s anchor collection. All of the objects and behaviors that you define in Reality Composer exist as children of the anchor entity, and therefore appear in your app when you display the AR view.

```
guard let anchor = try? MyProject.loadMyGreatScene() else { return }
arView.scene.anchors.append(anchor)
```

### Export the composition for previewing

You can also save your composition to a `.reality` or `.usdz` file for use as a lightweight AR Quick Look experience in your app or on the web. This allows users to place and preview content in the real world to get a quick sense of what it’s like.

To create a Reality file, choose File \> Export \> Export Project in the Reality Composer menu, and provide a name for the file. You use the Reality file that gets stored to disk just like you would use a usdz file, as described in Previewing a Model with AR Quick Look.

To create a USDZ file, see Exporting a Reality Composer Scene to USDZ.

## Topics

### Scene anchors

Selecting an anchor for a Reality Composer scene

Decide which anchor is right for your scenes.

Taking Control of Scene Anchoring

Create a more interactive user experience by choosing exactly where to anchor Reality Composer scenes.

### Scenes

Loading Reality Composer files using generated code

Leverage automatically generated code to load scenes from Xcode.

Loading Reality Composer files manually without generated code

Load Reality Composer files that aren’t part of your Xcode project.

### Scene elements

Adding elements to a 3D scene

Add assets to your scene from Reality Composer’s library, or import custom assets.

Configuring elements in a scene

Define the appearance and behavior of objects in a scene.

Arranging elements in a scene

Manipulate objects to complete your Reality Composer scene.

Manipulating Reality Composer scenes from code

Make programmatic changes to your scenes at runtime.

Adding procedural assets to a scene

Create procedurally generated shape primitives to your Reality Composer scene.

### Behaviors

Bringing a Reality Composer scene to life

Add animation and handle user input by using behaviors, triggers, and actions.

Building custom behaviors

Create custom behaviors to control objects in your scene.

### Exporting

Exporting a Reality Composer Scene to USDZ

Save a scene or project as USDZ to read, collect, or display in an app or website.

## See Also

### Scene creation

Loading Reality Composer files using generated code

Leverage automatically generated code to load scenes from Xcode.

Loading Reality Composer files manually without generated code

Load Reality Composer files that aren’t part of your Xcode project.

Adding elements to a 3D scene

Add assets to your scene from Reality Composer’s library, or import custom assets.

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

