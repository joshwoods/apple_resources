

- Core Foundation
-  CGSize 

Structure

# CGSize

A structure that contains width and height values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGSize
```

## Overview

A CGSize structure is sometimes used to represent a distance vector, rather than a physical size. As a vector, its values can be negative. To normalize a CGRect structure so that its size is represented by positive values, call the standardized function.

## Topics

### Geometric Properties

var width: Double

A width value.

var height: Double

A height value.

### Special Values

static var zero: CGSize { get }

init()

Creates a size with zero width and height.

### Transforming Sizes

func applying(_ t: CGAffineTransform) -> CGSize

### Alternate Representations

var dictionaryRepresentation: CFDictionary { get }

init?(dictionaryRepresentation dict: CFDictionary)

var debugDescription: String

A textual representation of the size’s dimensions.

var customMirror: Mirror

A representation of the size’s structure and display style for use in debugging.

var customPlaygroundQuickLook: PlaygroundQuickLook { get }

A custom playground Quick Look for this instance.

### Comparing Sizes

func CGSizeEqualToSize(_ size1: CGSize, _ size2: CGSize) -> Bool

Returns whether two sizes are equal.

### Initializers

init?(dictionaryRepresentation: CFDictionary)

init(width: Double, height: Double)

init(width: Double, height: Double)

init(width: Int, height: Int)

### Instance Properties

var customPlaygroundQuickLook: PlaygroundQuickLook

A custom playground Quick Look for this instance.

Deprecated

var dictionaryRepresentation: CFDictionary

### Instance Methods

func applying(CGAffineTransform) -> CGSize

func equalTo(CGSize) -> Bool

### Type Properties

static var zero: CGSize

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Structures

struct CGAffineTransform

struct CGAffineTransformComponents

struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

struct CGPoint

struct CGRect

struct CGVector

A structure that contains a two-dimensional vector.

