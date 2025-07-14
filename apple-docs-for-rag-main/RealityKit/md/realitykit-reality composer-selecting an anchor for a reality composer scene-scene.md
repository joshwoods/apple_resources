

- RealityKit
- Reality Composer
-  Selecting an anchor for a Reality Composer scene 

Article

# Selecting an anchor for a Reality Composer scene

Decide which anchor is right for your scenes.

## Overview

*Reality Composer* projects contain virtual scenes that you can add to real-world environments using RealityKit. To place a *Reality Composer* scene into the real world, you must anchor its content to a detected surface, image, face, or object. RealityKit automatically detects appropriate anchors for many types of scenes, though you can also manually detect and place your scenes if you want more control or have more specific anchoring requirements than *Reality Composer* provides.

When you create a new project or add a scene to an existing project, Reality Composer presents you with a sheet asking you to select an anchor type. The anchor type you select defines how your scene’s content is added to the real world by identifying the types of detected real-world surfaces, images, faces, or objects that you can place it in relation to.

Note

You can manually load and anchor Reality Composer scenes using code, like you do with other ARKit content. When you anchor a scene in code, RealityKit ignores the scene’s anchoring information.

*Reality Composer* supports five anchor types: Horizontal, Vertical, Image, Face, and Object. It displays a different set of guides for each anchor type to help you place your content. You can change the anchor type later if you choose the wrong option or change your mind about how to anchor your scene.

For each anchor type, *Reality Composer* automatically creates a default scene for you. You can use the default scene as a placeholder to test your code until you are ready to construct your own scene. If you do not want *Reality Composer* to add content to your newly created scene, deselect the “Create with default content” checkbox at the bottom left of the action sheet.

### Select horizontal anchoring for tables and floors

Horizontal anchoring is the default option when creating a new document or scene. Use this anchor type for scenes containing 3D objects to be placed on a table, floor, or other flat surface. When you select a horizontal anchor for your scene, Reality Composer shows a guide grid to represent the real-world surface onto which it will place your scene.

### Select vertical anchoring for walls and free-floating objects

Use vertical anchoring for scenes that contain objects to be placed against a wall, column, or other vertical surface. A vertical anchor is a good choice for scenes that contain, for example, a shelf, a basketball hoop, or a wall clock. After you select this anchor type, Reality Composer displays a vertical grid that represents the wall or other detected vertical surface to position the scene against.

### Select image anchoring to augment real-world 2D images

Select image anchoring to place your scene over or near an existing two-dimensional image in the real world, such as a poster, painting, or photograph. After you select this anchor type, *Reality Composer* displays a white-square guide to represent the detected real-world image to place your content near. Any object in your scene that is in front of the guide will appear in front of the detected image.

In the Properties inspector, select a reference image asset that you want ARKit to detect. The white square then changes to the selected reference image, indicating that ARKit will look for that specific image and automatically anchor your scene to it. ARKit continues tracking the image’s location so that if the image moves, your scene moves with it. In the scene, you should also select the real-world size of the image you want ARKit to detect, by using the Physical Height and Physical Width controls in the Scene inspector.

Important

RealityKit’s automatic anchoring and tracking will not work for your scene if you do not select a reference image. However, you may wish to leave the reference image empty for some scenes. If, for example, you wish to attach the same scene to multiple reference images, you will need to configure ARKit’s image detection and then anchor your scene manually. For more information about configuring image detection, see Detecting Images in an AR Experience.

### Select face anchoring to place a scene relative to a detected face

Select face anchoring to place content on or near detected human faces in ARKit. When you select this anchor type, *Reality Composer* displays a 3D face to stand in for the real-world face that ARKit has detected. You can’t move or edit the face guide, but the contents of your scene are placed into the real world based on their relative position to the guide face. If, for example, you put a box in front of the eyes of the guide face, a bar is placed in front of a detected person’s eyes in your app’s ARView. For more details about ARKit face detection, see Tracking and visualizing faces.

Note

Face anchoring is only available when using the front-facing camera.

### Select object anchoring to place a scene near detected objects

Select this anchor type to place your scene near a real-world object that ARKit has detected, based on an object that you’ve scanned. RealityKit automatically detects objects matching your scan, and anchors your scene to it. Object anchoring is a good choice for adding content to a real-world object like a toy, tool, or other physical object. For more details about ARKit object detection, see Scanning and Detecting 3D Objects.

After you select object anchoring, *Reality Composer* displays a yellow cube with a red exclamation point inside. The cube represents the object your scene is anchored to, and the exclamation point indicates that you need to identify the type of detected object to anchor your scene to. In the Properties inspector, below the anchor type, select a scanned object asset to use as an anchor. An image of the scanned object then replaces the exclamation point.

Unlike RealityKit image anchoring, object anchoring does not continuously track detected objects. If a detected object moves, it may take a few seconds before the scene’s position is updated to reflect its anchor’s new location.

### Change the selected anchor type

While building your scene, you may realize that a different anchor type is a better fit for what you’re building. With *Reality Composer*, you can change the anchor type of your scene at any time. Simply click or tap your scene’s background to deselect any selected objects. Then check the Scene inspector for a section titled Anchor, which shows the five possible anchor types. Click the new anchor type you that want to use for your scene.

When you select a new anchor, none of your scene’s content changes, but the guides are updated to reflect the new anchor type. You may have to adjust the location of some of your objects to ensure that they still align correctly with the new guides.

