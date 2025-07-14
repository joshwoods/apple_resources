

- Group Activities
- SystemCoordinator
-  SystemCoordinator.Configuration 

Structure

# SystemCoordinator.Configuration

A structure that specifies your app’s support for activities that take place in a shared simulation space.

visionOS 1.0+

``` source
struct Configuration
```

## Overview

A SystemCoordinator.Configuration structure stores your app’s preferences for the creation and arrangement of spatial Personas in a FaceTime call. Use this type to tell the system that you support activities that take place in one of your app’s immersive spaces, and how you want the system to arrange spatial Personas around your app’s content. To create a shared simulation space for your activity, set the supportsGroupImmersiveSpace property to `true`.

To specify your app’s preferences, create a new SystemCoordinator.Configuration structure with those preferences and assign it to the configuration property of your SystemCoordinator object. Assign this value before you join the session for the activity.

## Topics

### Creating a configuration structure

init()

Creates the type you use to specify your app’s preferences for shared contexts.

### Specifying spatial position preferences

var spatialTemplatePreference: SpatialTemplatePreference

The preferred arrangement of spatial Personas in your app’s immersive space.

struct SpatialTemplatePreference

A structure that specifies the preferred arrangement of participant spatial Personas in a shared simulation space.

### Supporting activities in immersive spaces

var supportsGroupImmersiveSpace: Bool

A Boolean value that indicates whether your app supports a shared context when an immersive space is open.

## Relationships

### Conforms To

- Sendable

## See Also

### Configuring the system coordinator

var configuration: SystemCoordinator.Configuration

The current configuration of the system coordinator.

