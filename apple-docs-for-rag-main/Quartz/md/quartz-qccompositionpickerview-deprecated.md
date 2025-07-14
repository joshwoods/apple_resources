

- Quartz
-  QCCompositionPickerView Deprecated

Class

# QCCompositionPickerView

The `QCCompositionPickerView` class allows users to browse compositions that are in the Quartz Composer composition repository, and to preview them. You can set the default input parameters for a composition preview by using the method setDefaultValue:forInputKey:.

macOS 10.4–10.15Deprecated

``` source
@MainActor
class QCCompositionPickerView
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

Note that the composition picker view does not automatically refresh its content when the composition repository is updated. It’s your responsibility to perform any necessary updating.

## Topics

### Setting and Getting the Background Color

func setBackgroundColor(NSColor!)

Sets the background color for the composition picker view.

func backgroundColor() -> NSColor!

Returns the background color of the composition picker view.

### Managing Background Drawing

func setDrawsBackground(Bool)

Sets whether the composition picker view draws its background.

func drawsBackground() -> Bool

Returns whether the composition picker view draws its background.

### Setting Composition Input Parameters

func setDefaultValue(Any!, forInputKey: String!)

Sets the default value to use for a composition input parameter.

func resetDefaultInputValues()

Clears all previously set default values for composition input parameters.

### Managing Animation

func startAnimation(Any!)

Starts animating the composition in the composition picker view.

func stopAnimation(Any!)

Stops animating the composition that is currently animating in the composition picker view.

func isAnimating() -> Bool

Returns whether or not the composition picker view is currently animating its composition.

func setMaxAnimationFrameRate(Float)

Sets the maximum frame rate for animating compositions.

func maxAnimationFrameRate() -> Float

Retrieves the maximum frame rate for animating compositions.

### Controlling Display of Composition Names

func setShowsCompositionNames(Bool)

Enables the display of composition names in the composition picker view.

func showsCompositionNames() -> Bool

Retrieves whether composition names can be shown in the composition picker view.

### Setting and Retrieving the View Delegate

func setDelegate(Any!)

Sets the composition picker view delegate.

func delegate() -> Any!

Retrieves the composition picker view delegate.

### Managing the Composition Picker View

func setCompositionsFromRepositoryWithProtocol(String!, andAttributes: [AnyHashable : Any]!)

Sets the compositions in the composition picker view to those that match the specified criteria.

func compositions() -> [Any]!

Returns the list of compositions that are currently in the composition picker view.

func setAllowsEmptySelection(Bool)

Sets whether to allow an empty selection in the composition picker view.

func allowsEmptySelection() -> Bool

Retrieves the empty-selection state of the composition picker view.

func setCompositionAspectRatio(NSSize)

Sets the aspect ratio used to display compositions in the composition picker view.

func compositionAspectRatio() -> NSSize

Retrieves the aspect ratio used to display compositions in the composition picker view.

func setSelectedComposition(QCComposition!)

Sets a composition as selected in the composition picker view.

func selectedComposition() -> QCComposition!

Returns the composition that is currently selected in the composition picker view.

### Working with Columns and Rows

func setNumberOfColumns(Int)

Sets the number of columns in the composition picker view.

func numberOfColumns() -> Int

Retrieves the number of columns in the composition picker view.

func setNumberOfRows(Int)

Sets the number of rows in the composition picker view.

func numberOfRows() -> Int

Retrieves the number of rows in the composition picker view.

## Relationships

### Inherits From

- NSView

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

### Classes

class QCComposition

The `QCComposition` class represents a Quartz Composer composition that either:

Deprecated

class QCCompositionLayer

A layer that loads, plays, and controls Quartz Composer compositions in a Core Animation layer hierarchy.

Deprecated

class QCCompositionParameterView

A class that allows users to edit the input parameters of a composition in real time. The composition can be rendering in any of the following objects: QCRenderer, QCView, or QCCompositionLayer.

Deprecated

class QCCompositionPickerPanel

The `QCCompositionPickerPanel` class represents a utility window that allows users to browse compositions that are in the Quartz Composer composition repository and, if supported, preview the composition. The `QCCompositionPickerPanel` class cannot be subclassed.

Deprecated

class QCCompositionRepository

The `QCCompositionRepository` class represents a system-wide centralized repository of built-in and installed Quartz Composer compositions (`/Library/Compositions` and `~/Library/Compositions`). The `QCCompositionRepository` class cannot be subclassed.

Deprecated

class QCPatchControllerDeprecated

class QCPlugIn

A base class to subclass for writing custom patches.

Deprecated

class QCPlugInViewController

The `QCPlugInViewController` class communicates (through Cocoa bindings) between a custom patch and the view used for the internal settings of the custom patch. Only custom patches that use internal settings exposed to the user need to use the `QCPlugInViewController` class.

Deprecated

class QCRenderer

A base class for low-level rendering.

Deprecated

class QCView

The `QCView` class is a custom `NSView` class that loads, plays, and controls Quartz Composer compositions. It is an autonomous view that is driven by an internal timer running on the main thread.

Deprecated

