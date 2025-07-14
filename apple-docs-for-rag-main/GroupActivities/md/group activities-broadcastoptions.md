

- Group Activities
-  BroadcastOptions 

Structure

# BroadcastOptions

Options for how to broadcast media on the shared communications channel.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct BroadcastOptions
```

## Overview

Use these options to alter how the system presents audio and video associated with an activity’s FaceTime call. For example, you might mirror video during a workout activity to make it easier to follow the instructor’s movements.

## Topics

### Getting the broadcast options

static let mirroredVideo: BroadcastOptions

An option to mirror video on its vertical axis.

### Creating options from a raw value

init(rawValue: Int)

Creates a set of options from a raw value.

let rawValue: Int

The raw value.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Specifying media-related behavior

var supportsContinuationOnTV: Bool

A Boolean value that indicates whether your app supports activity continuation on an Apple TV.

var preferredBroadcastOptions: BroadcastOptions

Preferences for how to present audio and video on the main communication channel.

