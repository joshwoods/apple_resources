

- SwiftUI
-  Clipboard 

API Collection

# Clipboard

Enable people to move or duplicate items by issuing Copy and Paste commands.

## Overview

When people issue standard Copy and Cut commands, they expect to move items to the system’s Clipboard, from which they can paste the items into another place in the same app or into another app. Your app can participate in this activity if you add view modifiers that indicate how to respond to the standard commands.

In your copy and paste modifiers, provide or accept types that conform to the Transferable protocol, or that inherit from the NSItemProvider class. When possible, prefer using transferable items.

## Topics

### Copying transferable items

func copyable&lt;T>(@autoclosure () -> [T]) -> some View

Specifies a list of items to copy in response to the system’s Copy command.

func cuttable&lt;T>(for: T.Type, action: () -> [T]) -> some View

Specifies an action that moves items to the Clipboard in response to the system’s Cut command.

func pasteDestination&lt;T>(for: T.Type, action: ([T]) -> Void, validator: ([T]) -> [T]) -> some View

Specifies an action that adds validated items to a view in response to the system’s Paste command.

### Copying items using item providers

func onCopyCommand(perform: (() -> [NSItemProvider])?) -> some View

Adds an action to perform in response to the system’s Copy command.

func onCutCommand(perform: (() -> [NSItemProvider])?) -> some View

Adds an action to perform in response to the system’s Cut command.

func onPasteCommand(of:perform:)

Adds an action to perform in response to the system’s Paste command.

func onPasteCommand(of:validator:perform:)

Adds an action to perform in response to the system’s Paste command with items that you validate.

## See Also

### Event handling

Gestures

Define interactions from taps, clicks, and swipes to fine-grained gestures.

Input events

Respond to input from a hardware device, like a keyboard or a Touch Bar.

Drag and drop

Enable people to move or duplicate items by dragging them from one location to another.

Focus

Identify and control which visible object responds to user interaction.

System events

React to system events, like opening a URL.

