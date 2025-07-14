

- AVKit
-  AVExperienceController 

Class

# AVExperienceController

An object that controls video experiences.

visionOS 2.0+

``` source
@MainActor
final class AVExperienceController
```

## Overview

Use this class to control, observe, and respond to experience changes for an AVPlayerViewController. A player view controller’s presentation APIs will no longer be honored after attaching an experience controller. Using the other presentation APIs may preclude the use of this class.

## Topics

### Configuring the experience

var allowedExperiences: AVExperienceController.Experiences

The set of experiences the application supports.

var availableExperiences: AVExperienceController.Experiences

The allowed experiences that are available to use on the device at this time.

struct Experiences

A structure that represents a collection of experiences to use with an experience controller.

var experience: AVExperienceController.Experience

The current experience.

enum Experience

The types of experiences the system supports.

var configuration: AVExperienceController.Configuration

The configuration options per experience.

struct Configuration

A structure that stores per-experience configuration.

### Transitioning experiences

func transition(to: AVExperienceController.Experience) async -> AVExperienceController.TransitionContext.TransitionResult

Transitions the video to a different experience.

### Configuring a delegate

var delegate: (any AVExperienceController.Delegate)?

A delegate object for the experience controller.

protocol Delegate

A protocol that defines the methods to implement to respond to experience changes.

### Structures

struct ExpandedConfiguration

A structure that specifies options for an expanded experience.

struct TransitionContext

The state of the transition provided to the delegate object.

## Relationships

### Conforms To

- Sendable

## See Also

### visionOS Playback

Creating a multiview video playback experience in visionOS

Build an interface that plays multiple videos simultaneously and handles transitions to different experience types gracefully.

Adopting the system player interface in visionOS

Provide an optimized viewing experience for watching 3D video content.

Trimming and exporting media in visionOS

Display standard controls in your app to edit the timeline of the currently playing media.

class AVPlayerViewController

A view controller that displays content from a player and presents a native user interface to control playback.

protocol AVPlayerViewControllerDelegate

A protocol that defines the methods to implement to respond to player view controller events.

class AVMultiviewManager

An object that manages viewing multiple videos at once.

class AVGroupExperienceCoordinator

An object that synchronizes viewing environment state across participants in a SharePlay session.

