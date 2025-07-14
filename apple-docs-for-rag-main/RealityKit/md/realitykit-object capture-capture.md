

- RealityKit
-  Object capture 

API Collection

# Object capture

Create 3D objects from a series of photographs using photogrammetry.

## Overview

In iOS 17 and macOS 12 and later, you can create 3D objects from photographs using a process called photogrammetry. You provide RealityKit Object Capture with a series of well-lit photographs taken from many different angles. It analyzes the overlap area between different images to match up landmarks and produces a 3D model of the photographed object.

## Topics

### Model creation

Capturing photographs for RealityKit Object Capture

Take high-quality images of objects to generate 3D models.

Creating 3D objects from photographs

Construct virtual objects to use in your AR experiences.

Scanning objects using Object Capture

Implement a full scanning workflow for capturing objects on iOS devices.

Building an object reconstruction app

Reconstruct objects from user-selected input images by using photogrammetry.

Creating a Photogrammetry Command-Line App

Generate 3D objects from images using RealityKit Object Capture.

Using object capture assets in RealityKit

Create a chess game using RealityKit and assets created using Object Capture.

class PhotogrammetrySession

Manages the creation of a 3D model from a set of images.

struct PhotogrammetrySample

An object that represents one image and its corresponding metadata.

struct ObjectCaptureView

A view that guides a user through capturing images for object capture.

class ObjectCaptureSession

A session object that monitors and controls image capture for photogrammetry.

struct ObjectCapturePointCloudView

Renders the current state of the point cloud from an object capture session.

## See Also

### Asset creation

Designing RealityKit content with Reality Composer Pro

Design RealityKit scenes for your visionOS app.

Swift Splash

Use RealityKit to create an interactive ride in visionOS.

Diorama

Design scenes for your visionOS app using Reality Composer Pro.

Composing interactive 3D content with RealityKit and Reality Composer Pro

Build an interactive scene using an animation timeline.

Presenting an artist’s scene

Display a scene from Reality Composer Pro in visionOS.

Reality Composer

A visual editor for RealityKit AR scenes.

USD Assets

Import and use 3D scenes by importing USD files.

