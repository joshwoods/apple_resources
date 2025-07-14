

- AppKit
- Text Display
-  Adopting the system text cursor in custom text views 

Article

# Adopting the system text cursor in custom text views

Incorporate the system text cursor into your custom text UI in AppKit.

## Overview

People can enter text into your app in a variety of ways, such as typing, copy and paste, or dictation. macOS 14 introduces enhancements to the system UI for the text cursor to provide a more seamless text experience.

If your app handles text input through standard AppKit views such as NSTextView or NSTextField, your app automatically uses the system UI for the text cursor. This system UI includes the following elements:

- The text cursor that indicates the insertion point of the text

- Text cursor accessories that indicate state, such as current input source language, dictation, and Caps Lock

- Animation effects that surround the text cursor during dictation

If you have a highly customized UI for displaying text, you can adopt this system UI in your AppKit app.

### Add the system text cursor to a custom text view

If your app handles text input through a custom view that builds on NSTextInputClient, you can display the system text cursor manually. Create an NSTextInsertionIndicator view and add it on top of the view that displays text in your app.

```
// Set up the text cursor.
let textCursor = NSTextInsertionIndicator(frame: .zero)
documentView.addSubview(textCursor)
```

When your custom text view becomes active or becomes first responder, update the display mode of the text cursor.

```
// Show the text cursor when the text view becomes active.
func didBecomeActive() {
    textCursor.displayMode = .automatic
}
```

### Configure the text cursor animations

Depending on the behavior you need at a particular point in time, you can determine how the text cursor handles animations by selecting one of these display modes:

- Automatic. Set the NSTextInsertionIndicator.DisplayMode.automatic display mode to stop and start animations for the text cursor automatically. These animations include a blinking effect that applies to the text cursor during typing and dictation, animated transitions between dictation states, and automatic hiding of the text cursor during tracking loops. This display mode is appropriate in the majority of cases when your custom text view is accepting text input.

- Always visible. Set the NSTextInsertionIndicator.DisplayMode.visible display mode to always show the text cursor and disable animations. This display mode is appropriate when the text cursor needs to appear without blinking — for example, to indicate a drop destination as part of a drag and drop interaction.

When you use the automatic display mode, you can further customize the animation options depending on the needs of your app.

- By default, the text cursor hides automatically during tracking loops. Include the showWhileTracking option in automaticModeOptions to show the text cursor during tracking instead.

- By default, the text cursor shows an animated effect during dictation. To completely hide the view that draws the animated effect, remove showEffectsView from automaticModeOptions. To customize the placement of this view in your view hierarchy, specify effectsViewInserter.

The following code shows how to customize the placement of the animated effects view to place it directly below the text cursor.

```
// Specify custom view hierarchy placement for the animated effects view.
textCursor.effectsViewInserter = { view in
    documentView.addSubview(view, positioned: .below, relativeTo: textCursor)
}
```

### Update the text cursor position

Your custom text view is responsible for updating the position of the text cursor when a person inputs text, but the system provides the appropriate animated effect. For example, the following image shows the system animation effect that applies to the text cursor during dictation.

As a person types or inserts text during dictation, update the frame of the NSTextInsertionIndicator view. The view automatically changes its appearance in response to that movement, matching the system UI for the corresponding type of input (typing or dictation).

### Configure the placements of text cursor accessories

The system text cursor displays accessories that indicate state, such as current input source language, dictation, and Caps Lock. For example, the following image shows the text cursor with the dictation indicator and the current input language set to English.

When a person changes the input language, the accessory expands to show the language selection UI in the language switcher accessory.

NSTextInsertionIndicator draws these accessories automatically, but you can specify where in relation to the text cursor to draw them. In your custom text view, you can override the placement of these accessories by specifying preferredTextAccessoryPlacement() in your implementation of NSTextInputClient. When the system renders the text cursor in your custom view, it uses the return value of this method to determine where to draw the accessories.

### Indicate the offscreen text cursor position during dictation

The system text cursor shows a dictation indicator accessory during an active dictation session. When a person scrolls the text cursor offscreen during dictation, the system also draws a scroll-away indicator to indicate the position of the cursor. For example, the following image shows a scroll-away indicator that points downwards, indicating that the text cursor is out of view below.

For the system to show the scroll-away indicator on a custom text view, you need to complete the following steps:

- Adopt NSTextInputClient and implement unionRectInVisibleSelectedRange and documentVisibleRect. These properties provide the system with the coordinate information it needs to draw the scroll-away indicator in the appropriate position.

- Notify the system when a person starts or stops scrolling, so the system can display the indicator at the appropriate time. Call textInputClientWillStartScrollingOrZooming() when scrolling starts, and textInputClientDidEndScrollingOrZooming() when scrolling ends.

### Hide the system text cursor

When your custom text view resigns first responder status, update the display mode of the text cursor to NSTextInsertionIndicator.DisplayMode.hidden.

```
// Hide the text cursor when the text view becomes inactive.
func didBecomeInactive() {
    textCursor.displayMode = .hidden
}
```

If you implement custom text UI in a UIKit app, see Adopting system selection UI in custom text views.

Related sessions from WWDC23

Session 10058: What’s new with text and text interactions

## See Also

### Text input

class NSTextInputContext

An object that represents the Cocoa text input system.

protocol NSTextInputClient

A set of methods that text views need to implement to interact properly with the text input management system.

class NSTextAlternatives

A list of alternative strings for a piece of text.

protocol NSTextContent

A protocol that describes specific kinds of input content types.

class NSTextInsertionIndicator

A view that represents the insertion indicator in text.

enum DisplayMode

Constants that determine how to display the system text cursor in a custom text UI.

struct AutomaticModeOptions

Options that affect the automatic display mode.

