

- AppKit
-  Animation 

API Collection

# Animation

Animate your views and other content to create a more engaging experience for users.

## Topics

### View-Based Animations

class NSViewAnimation

An animation of an app’s views, limited to changes in frame location and size, and to fade-in and fade-out effects.

protocol NSAnimatablePropertyContainer

A set of methods that defines a way to add animation to an existing class with a minimum of API impact.

class NSAnimationContext

An animation context, which contains information about environment and state.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

enum NSAnimationEffect

The type for standard system animation effects, which include both display and sound.

Deprecated

### Presentations

protocol NSViewControllerPresentationAnimator

A set of methods that let you define animations to play when transitioning between two view controllers.

### Custom Animations

class NSAnimation

An object that manages the timing and progress of animations in the user interface.

protocol NSAnimationDelegate

A set of optional methods implemented by delegates of NSAnimation objects.

## See Also

### User Interface

Views and Controls

Present your content onscreen and handle user input and events.

View Management

Manage your user interface, including the size and position of views in a window.

View Layout

Position and size views using a stack view or Auto Layout constraints.

Appearance Customization

Add Dark Mode support to your app, and use appearance proxies to modify your UI.

Windows, Panels, and Screens

Organize your view hierarchies and facilitate their display onscreen.

Sound, Speech, and Haptics

Play sounds and haptic feedback, and incorporate speech recognition and synthesis into your interface.

Supporting Continuity Camera in Your Mac App

Incorporate scanned documents and pictures from a user’s iPhone, iPad, or iPod touch into your Mac app using Continuity Camera.

