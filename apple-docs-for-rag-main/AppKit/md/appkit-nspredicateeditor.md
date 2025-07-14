

- AppKit
-  NSPredicateEditor 

Class

# NSPredicateEditor

A defined set of rules that allows the editing of predicate objects.

macOS 10.5+

``` source
@MainActor
class NSPredicateEditor
```

## Overview

`NSPredicateEditor` provides an NSPredicate property—objectValue (inherited from NSControl)—that you can get and set directly, and that you can bind using Cocoa bindings (you typically configure a predicate editor in Interface Builder). `NSPredicateEditor` depends on another class, NSPredicateEditorRowTemplate, that describes the available predicates and how to display them.

Unlike `NSRuleEditor`, `NSPredicateEditor` does not depend on its delegate to populate its rows (and *does not call the populating delegate methods*). Instead, its rows are populated from its `objectValue` property (an instance of `NSPredicate`). `NSPredicateEditor` relies on instances NSPredicateEditorRowTemplate, which are responsible for mapping back and forth between the displayed view values and various predicates.

`NSPredicateEditor` exposes one property, rowTemplates, which is an array of NSPredicateEditorRowTemplate objects.

## Topics

### Managing Row Templates

var rowTemplates: [NSPredicateEditorRowTemplate]

The row templates for the receiver.

class NSPredicateEditorRowTemplate

A template that describes available predicates and how to display them.

## Relationships

### Inherits From

- NSRuleEditor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Controls

Responding to control-based events using target-action

Handle user input by connecting buttons, sliders, and other controls to your app’s code using the target-action design pattern.

class NSButton

A control that defines an area on the screen that a user clicks to trigger an action.

class NSColorWell

A control that displays a color value and lets the user change that color value.

Combo Box

Display a list of values in a pop-up menu that lets the user select a value or type in a custom value.

class NSComboButton

A button with a pull-down menu and a default action.

Date Picker

Display a calendar date and provide controls for editing the date value.

class NSImageView

A display of image data in a frame.

class NSLevelIndicator

A visual representation of a level or quantity, using discrete values.

Path Control

A display of a file system path or virtual path information.

class NSPopUpButton

A control for selecting an item from a list.

class NSProgressIndicator

An interface that provides visual feedback to the user about the status of an ongoing task.

class NSRuleEditor

An interface for configuring a rule-based list of options.

Search Field

Provide a text field that is optimized for text-based search interfaces.

class NSSegmentedControl

Display one or more buttons in a single horizontal group.

Slider

Display a range of values from which the user selects a single value.

