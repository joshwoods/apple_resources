

- UIKit
-  UIUpdateLink 

Class

# UIUpdateLink

An object you use to observe, participate in, and affect the UI update process.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
class UIUpdateLink
```

## Overview

With a *UI update link*, you can follow the progress of each UI update and express preferences about how those updates happen. Use a UI update link when you need precise and predictable control over the UI update process.

There are multiple use cases for UIUpdateLink, including:

- To monitor when UI updates occur and synchronize your drawing code with each update, similar to how you might use CADisplayLink.

- To influence how UI updates occur by expressing preferences to the system, such as requesting continuous UI updates, immediate rendering of frames, and more.

- To specify precisely at which point in the UI update process to perform certain actions.

- To implement support for low-latency input, such as a custom low-latency drawing implementation for a pencil-drawing app.

To create a UI update link, you associate it with a window or a view. The UI update link activates automatically when you add the view to a visible window, and deactivates when you remove the view from it. If the view moves from one display to another, UIUpdateLink adjusts to the timing of the new display automatically.

```
// Monitor UI updates for a specific view.
let updateLink = UIUpdateLink(view: view)
updateLink.isEnabled = true

// Influence the UI update process by requesting continuous UI updates.
updateLink.requiresContinuousUpdates = true

// Specify one or more actions to perform for each UI update.
// Add an action to the `.beforeCADisplayLinkDispatch` phase, by default.
updateLink.addAction() { link, info in 
    // Code that runs each UI update, after processing input events, 
    // but before `CADisplayLink` callbacks.
    self.view.center.y = sin(info.modelTime) * 100 + self.view.bounds.midY
}

// Add an action to a specific UI update phase that you choose.
updateLink.addAction(to: .afterUpdateScheduled) { link, info in 
    // Code that runs each UI update, after the system schedules the update, 
    // but before processing input events.
    // ...
}
```

Important

Only use UIUpdateLink from the main thread.

## Topics

### Creating a UI update link

init(view: UIView)

Creates a UI update link for the specified view.

init(view: UIView, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified view using the specified action handler.

init(view: UIView, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified view using the specified target and action.

init(windowScene: UIWindowScene)

Creates a UI update link for the specified window.

init(windowScene: UIWindowScene, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified window using the specified action handler.

init(windowScene: UIWindowScene, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified window using the specified target and action.

### Participating in UI updates

var isEnabled: Bool

A Boolean value that determines whether the UI update link is monitoring UI updates.

### Configuring preferences

var requiresContinuousUpdates: Bool

A Boolean value that determines whether the UI update link needs continuous UI updates.

var wantsLowLatencyEventDispatch: Bool

A Boolean value that determines whether the UI update link requests dispatch of low-latency eligible events.

var wantsImmediatePresentation: Bool

A Boolean value that determines whether the UI update link requests immediate frame presentation.

var preferredFrameRateRange: CAFrameRateRange

The range of frame rates the UI update link prefers.

### Getting the current UI update information

func currentUpdateInfo() -> UIUpdateInfo?

Returns an object that describes the current UI update state.

class UIUpdateInfo

An object that contains detailed information about the current UI update state.

### Adding actions

func addAction(handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link.

func addAction(to: UIUpdateActionPhase, handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link for a particular UI update phase.

func addAction(target: Any, selector: Selector)

Adds an action with the specified target and selector to the UI update link.

func addAction(to: UIUpdateActionPhase, target: Any, selector: Selector)

Adds an action with the specified target and selector to the UI update link for a particular UI update phase.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### UI updates

class UIUpdateInfo

An object that contains detailed information about the current UI update state.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

