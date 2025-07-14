

- ARKit
-  ARCoachingOverlayView 

Class

# ARCoachingOverlayView

A view that displays standardized onboarding instructions to direct users toward a specific goal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
class ARCoachingOverlayView
```

## Overview

This view offers your users a standardized onboarding routine. You can configure this view to automatically display during session initialization and in limited tracking situations, while giving the user specific instructions that best facilitate ARKit’s world tracking.

These illustrations show overlay views with horizontal- and vertical-plane goals, indicating that the user should begin moving the device:

These illustrations show overlay views indicating that the user should continue moving the phone or change the speed with which they move it:

When you start your app, the coaching overlay asks the user to move the device in ways that help ARKit establish tracking. When you choose a specific goal like finding a plane, the view tailors its instructions accordingly. After the coaching overlay determines the goal has been met and no further coaching is required, it hides from the user’s view.

For an example app that uses the coaching overlay, see Placing objects and handling 3D interaction.

### Supporting Automatic Coaching

By default, activatesAutomatically is enabled and therefore you should override coachingOverlayViewWillActivate(_:) to determine whether coaching is in progress. Coordinate your actions to help the user focus on these instructions, for example, by hiding any UI that’s not necessary while the session reinitializes.

### Relocalizing After an Interruption

If relocalization is enabled (see sessionShouldAttemptRelocalization(_:)), ARKit attempts to restore your session if any interruptions degrade your app’s tracking state. In this event, the coaching overlay presents itself and gives the user instructions to assist ARKit with relocalizing.

During this time, the coaching overlay includes a button that lets the user indicate they’d like to start over rather than restore the session.

ARKit notifies you when the user presses Start Over by calling your delegate’s coachingOverlayViewDidRequestSessionReset(_:) function. Implement this callback if your app requires any custom actions to restart the AR experience.

```
func coachingOverlayViewDidRequestSessionReset(_ coachingOverlayView: ARCoachingOverlayView) {    

    // Reset the session.
    let configuration = ARWorldTrackingConfiguration()
    configuration.planeDetection = [.horizontal, .vertical]
    session.run(configuration, options: [.resetTracking])

    // Custom actions to restart the AR experience. 
    // ...
}
```

If you do not implement coachingOverlayViewDidRequestSessionReset(_:), the coaching overlay responds to the Start Over button by resetting tracking, which also removes any existing anchors.

For more information about relocalization, see Managing Session Life Cycle and Tracking Quality.

## Topics

### Delegating Events

var delegate: (any ARCoachingOverlayViewDelegate)?

An object you supply that implements coaching event callbacks.

protocol ARCoachingOverlayViewDelegate

A set of callbacks you implement to be notified of coaching events.

### Defining a Goal

var goal: ARCoachingOverlayView.Goal

A field that indicates your app’s tracking requirements.

enum Goal

The options that specify your app’s tracking requirements.

### Activating the View

var activatesAutomatically: Bool

A flag that indicates whether the coaching view activates automatically, depending on the current session state.

var isActive: Bool

A flag that indicates whether coaching is in progress.

func setActive(Bool, animated: Bool)

Controls whether coaching is in progress.

### Providing the Session

var session: ARSession?

The session this view uses to provide coaching.

var sessionProvider: (any ARSessionProviding)?

An object you designate that provides the current session.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Views

@MainActor @objc @preconcurrency class ARView

A view that enables you to display an AR experience with RealityKit.

class ARSCNView

A view that blends virtual 3D content from SceneKit into your augmented reality experience.

class ARSKView

A view that blends virtual 2D content from SpriteKit into the 3D space of an augmented reality experience.

