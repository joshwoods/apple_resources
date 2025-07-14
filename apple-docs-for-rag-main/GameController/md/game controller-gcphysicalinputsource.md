

- Game Controller
-  GCPhysicalInputSource 

Protocol

# GCPhysicalInputSource

A protocol for a description of an element without any system-level remapping of the controls.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
protocol GCPhysicalInputSource : NSObjectProtocol
```

## Overview

If necessary, use the properties in this protocol to get the actual input element aliases, localized name, and symbols without the user’s remapping of the controls in the System Game Controller settings. Otherwise, use the localizedName and sfSymbolsName in the GCPhysicalInputElement protocol in your interface.

## Topics

### Getting a localized name

var elementLocalizedName: String?

The localized name for the element without any system-level remapping of the controls.

**Required**

### Displaying a symbol

var sfSymbolsName: String?

A system symbol for the element without any system-level remapping of the controls.

**Required**

### Accessing elements by key

var elementAliases: Set&lt;String>

The element’s true aliases without any system-level remapping of the controls.

**Required**

### Getting directions

var direction: GCPhysicalInputSourceDirection

The directional input, if any, that a physical input source involves.

**Required**

struct GCPhysicalInputSourceDirection

The directions that a physical input source involves.

## Relationships

### Inherits From

- NSObjectProtocol

