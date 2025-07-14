

- ARKit
- ARWorldTrackingConfiguration
-  ARWorldTrackingConfiguration.PlaneDetection 

Structure

# ARWorldTrackingConfiguration.PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
struct PlaneDetection
```

## Overview

By default, this configuration disables plane detection. If you enable horizontal or vertical plane detection, the session adds ARPlaneAnchor objects and notifies your ARSessionDelegate, ARSCNViewDelegate, or ARSKViewDelegate object when its analysis of captured video images detects an area that appears to be a flat surface.

Use an empty set literal `[]` to specify no plane detection.

## Topics

### Plane Detection Option Creation

init(rawValue: UInt)

Creates plane detection options.

### Plane Detection Options

static var horizontal: ARWorldTrackingConfiguration.PlaneDetection

The session detects planar surfaces that are perpendicular to gravity.

static var vertical: ARWorldTrackingConfiguration.PlaneDetection

The session detects surfaces that are parallel to gravity, regardless of other orientation.

static var horizontal: ARWorldTrackingConfiguration.PlaneDetection

The session detects planar surfaces that are perpendicular to gravity.

static var vertical: ARWorldTrackingConfiguration.PlaneDetection

The session detects surfaces that are parallel to gravity, regardless of other orientation.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Enabling Plane Detection

var planeDetection: ARWorldTrackingConfiguration.PlaneDetection

A value specifying whether and how the session attempts to automatically detect flat surfaces in the camera-captured image.

