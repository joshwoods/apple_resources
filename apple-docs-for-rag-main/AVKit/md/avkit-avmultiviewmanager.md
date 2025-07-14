

- AVKit
-  AVMultiviewManager 

Class

# AVMultiviewManager

An object that manages viewing multiple videos at once.

visionOS 2.0+

``` source
@MainActor
final class AVMultiviewManager
```

## Overview

Watch multiple videos at the same time with AVExperienceController.Experience.multiview using multiple AVExperienceController objects.

## Topics

### Accessing the default instance

static var `default`: AVMultiviewManager

Use this default AVMultiviewManager to customize the multiview experience.

### Providing additional UI

var contentSelectionViewController: AVContentSelectionViewController?

A view controller that presents a user interface to select additional video content to display.

class AVContentSelectionViewController

A view controller for providing additional UI to the multiview experience.

### Dismissing the multiview experience

func dismiss()

Dismiss the multiview presentation.

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

class AVExperienceController

An object that controls video experiences.

class AVGroupExperienceCoordinator

An object that synchronizes viewing environment state across participants in a SharePlay session.

