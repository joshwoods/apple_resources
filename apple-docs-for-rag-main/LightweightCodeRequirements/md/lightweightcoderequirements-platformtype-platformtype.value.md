

- LightweightCodeRequirements
- PlatformType
-  PlatformType.Value 

Structure

# PlatformType.Value

Supported Platform Types for a process

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Value
```

## Overview

A platform type is an indication of the runtime enviroment of a process. These runtime enviroments indicate the types of code that can run in the process, the dyld shared cache in use and impact some security policies.

## Topics

### Initializers

init?(rawValue: Int64)

Creates a new instance with the specified raw value.

### Instance Properties

let rawValue: Int64

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let driverKit: PlatformType.Value

The platform type for a driverkit driver.

static let iOS: PlatformType.Value

The platform type for iOS/iPadOS software running on iOS/ipadOS/macOS/visionOS

static let iOSSimulator: PlatformType.Value

The platform type for code running in the iOS Simulator.

static let macCatalyst: PlatformType.Value

The platform type for macCatalyst software.

static let macOS: PlatformType.Value

The platform type for non-macCatalyst macOS software.

static let tvOS: PlatformType.Value

The platform type for native tvOS software.

static let tvOSSimulator: PlatformType.Value

The platform type for code running in the tvOS Simulator.

static let visionOS: PlatformType.Value

The platform type for native visionOS code.

static let visionOSSimulator: PlatformType.Value

The platform type for code running in the visionOS Simulator.

static let watchOS: PlatformType.Value

The platform type for native watchOS software.

static let watchOSSimulator: PlatformType.Value

The platform type for code running in the watchOS Simulator.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

