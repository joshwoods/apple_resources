

- Game Controller
- GCVirtualController
-  GCVirtualController.Configuration 

Class

# GCVirtualController.Configuration

The configuration of a virtual controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class Configuration
```

## Mentioned in 

Adding touch controls to games that support game controllers in iOS

## Overview

You configure a virtual controller by specifying the input elements it contains. Then using the updateConfiguration(forElement:configuration:) method, you can customize individual elements.

## Topics

### Setting the elements

var elements: Set&lt;String>

The input elements of a virtual controller.

### Presenting a custom interface

var isHidden: Bool

A Boolean value that indicates whether the system or the app presents the virtual interface.

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

### Creating virtual controllers

init(configuration: GCVirtualController.Configuration)

Creates a new virtual controller using the configuration you specify.

