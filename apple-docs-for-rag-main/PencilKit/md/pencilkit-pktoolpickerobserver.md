

- PencilKit
-  PKToolPickerObserver 

Protocol

# PKToolPickerObserver

An interface you use to detect when the user changes the selected tools and drawing characteristics of a tool picker object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol PKToolPickerObserver : NSObjectProtocol
```

## Overview

Implement the methods of PKToolPickerObserver to detect when the user changes the configuration of a PKToolPicker view. Each time the user changes the selected tool or other drawing characteristics, the tool picker notifies any registered observers. You use these notifications to update the configuration of the underlying canvas.

To register an observer with a tool picker, call the addObserver(_:) method of the PKToolPicker object.

## Topics

### Detecting tool configuration changes

func toolPickerSelectedToolItemDidChange(PKToolPicker)

Tells the observer when a person selects a new tool item.

func toolPickerIsRulerActiveDidChange(PKToolPicker)

Tells the observer when a person shows or hides the ruler.

### Monitoring visibility changes

func toolPickerVisibilityDidChange(PKToolPicker)

Tells the observer when a person shows or hides the tool picker.

func toolPickerFramesObscuredDidChange(PKToolPicker)

Tells the observer when the area that the tool picker obscures changes.

### Deprecated

func toolPickerSelectedToolDidChange(PKToolPicker)

Tells the observer when a person selects a new tool.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- PKCanvasView

## See Also

### Detecting changes to the picker

func addObserver(any PKToolPickerObserver)

Adds the specified object to the list of objects to notify when the picker configuration changes.

func removeObserver(any PKToolPickerObserver)

Removes the specified object from the list of objects to notify when the picker configuration changes.

