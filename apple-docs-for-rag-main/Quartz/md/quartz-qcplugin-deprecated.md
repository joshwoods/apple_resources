

- Quartz
-  QCPlugIn Deprecated

Class

# QCPlugIn

A base class to subclass for writing custom patches.

macOS 10.4–10.15Deprecated

``` source
class QCPlugIn
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

The `QCPlugIn` class provides the base class to subclass for writing custom Quartz Composer patches. You implement a custom patch by subclassing `QCPlugIn`, overriding the appropriate methods, packaging the code as an `NSBundle` object, and installing the bundle in the appropriate location. A bundle can contain more than one subclass of `QCPlugIn`, allowing you to provide a suite of custom patches in one bundle. Quartz Composer Custom Patch Programming Guide provides detailed instructions on how to create and package a custom patch. *QCPlugIn Class Reference* supplements the information in the programming guide.

The methods related to the executing the custom patch (called when the Quartz Composer engine is rendering) are passed an opaque object that conforms to the QCPlugInContext protocol. This object represents the execution context of the `QCPlugIn` object. You should not retain the execution context or use it outside of the scope of the execution method that it is passed to.

## Topics

### Defining the Characteristics of a Custom Patch

class func executionMode() -> QCPlugInExecutionMode

Returns the execution mode of the custom patch.

class func timeMode() -> QCPlugInTimeMode

Returns the time mode for the custom patch.

### Executing a Custom Patch

func execute((any QCPlugInContext)!, atTime: TimeInterval, withArguments: [AnyHashable : Any]!) -> Bool

Performs the processing or rendering tasks appropriate for the custom patch.

### Performing Custom Tasks During Execution

func startExecution((any QCPlugInContext)!) -> Bool

Allows you to perform custom setup tasks before the Quartz Composer engine starts rendering.

func enableExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the execution of the `QCPlugIn` object is resumed.

func disableExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the execution of the `QCPlugIn` object is paused.

func stopExecution((any QCPlugInContext)!)

Allows you to perform custom tasks when the `QCPlugIn` object stops executing.

### Defining Patch and Property Port Attributes

class func attributes() -> [AnyHashable : Any]!

Returns a dictionary that contains strings for the user interface that describe the custom patch.

class func attributesForPropertyPort(withKey: String!) -> [AnyHashable : Any]!

Returns a dictionary that contains strings for the user interface that describe the optional attributes for ports created from properties.

### Defining Internal Settings

func createViewController() -> QCPlugInViewController!

Creates and returns a view controller for the Settings pane of a custom patch.

class func plugInKeys() -> [Any]!

Returns the keys for the internal settings of a custom patch.

### Supporting Saving and Retrieving Internal Settings

func serializedValue(forKey: String!) -> Any!

A method implemented to override serialization.

func setSerializedValue(Any!, forKey: String!)

Provides custom deserialization for patch internal settings that were previously serialized using the method serializedValue(forKey:).

### Adding Ports Dynamically

func addInputPort(withType: String!, forKey: String!, withAttributes: [AnyHashable : Any]!)

Adds an input port of the specified type and associates a key and attributes with the port.

func removeInputPort(forKey: String!)

Removes the input port for a given key.

func addOutputPort(withType: String!, forKey: String!, withAttributes: [AnyHashable : Any]!)

Adds an output port of the specified type and associates a key and attributes with the port.

func removeOutputPort(forKey: String!)

Removes the output port for a given key.

### Getting and Setting Port Values

func didValue(forInputKeyChange: String!) -> Bool

Returns whether the input port value changed since the last execution of the custom patch.

func value(forInputKey: String!) -> Any!

Returns the current value for an input port.

func setValue(Any!, forOutputKey: String!) -> Bool

Sets the value of an output port.

### Loading Bundle and Custom Patches Manually

class func load(atPath: String!) -> Bool

Loads a Quartz Composer plug-in bundle from the specified path.

class func registerClass(AnyClass!)

Registers a `QCPlugIn` subclass.

### Ordering Property Ports

class func sortedPropertyPortKeys() -> [Any]!

Returns and array of property port keys in the order you want them to appear in the user interface.

### Constants

Patch Attributes

Attributes for custom patches.

Input and Output Port Attributes

Attributes for input and output ports.

Port Input and Output Types

Data types for input and output ports.

Pixel Formats

Supported image pixel formats.

Execution Arguments

Arguments to the method execute(_:atTime:withArguments:).

struct QCPlugInExecutionMode

Execution modes for custom patches.

struct QCPlugInTimeMode

Time modes for custom patches.

### Instance Methods

func executionTime(for: (any QCPlugInContext)!, atTime: TimeInterval, withArguments: [AnyHashable : Any]!) -> TimeInterval

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

## See Also

### Related Documentation

Quartz Composer Custom Patch Programming Guide

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

class QCCompositionPickerView

The `QCCompositionPickerView` class allows users to browse compositions that are in the Quartz Composer composition repository, and to preview them. You can set the default input parameters for a composition preview by using the method setDefaultValue:forInputKey:.

Deprecated

class QCCompositionRepository

The `QCCompositionRepository` class represents a system-wide centralized repository of built-in and installed Quartz Composer compositions (`/Library/Compositions` and `~/Library/Compositions`). The `QCCompositionRepository` class cannot be subclassed.

Deprecated

class QCPatchControllerDeprecated

class QCPlugInViewController

The `QCPlugInViewController` class communicates (through Cocoa bindings) between a custom patch and the view used for the internal settings of the custom patch. Only custom patches that use internal settings exposed to the user need to use the `QCPlugInViewController` class.

Deprecated

class QCRenderer

A base class for low-level rendering.

Deprecated

class QCView

The `QCView` class is a custom `NSView` class that loads, plays, and controls Quartz Composer compositions. It is an autonomous view that is driven by an internal timer running on the main thread.

Deprecated

