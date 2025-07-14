

- Image Playground
-  ImagePlaygroundPersonalizationPolicy 

Enumeration

# ImagePlaygroundPersonalizationPolicy

A policy for enabling or disabling personalization in the system interface.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
enum ImagePlaygroundPersonalizationPolicy
```

## Overview

Use this type to configure the personalization behavior for the view controllers and SwiftUI view modifiers you use in your interface.

## Topics

### Getting the policy

case automatic

An option to choose the most appropriate personalization behavior.

case enabled

An option to enable personalization features in the view controller.

case disabled

An option to disable personalization features in the view controller.

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Specifying the configuration of the playground

var selectedGenerationStyle: ImagePlaygroundStyle

Generation style to pre-select upong launching the playground among those in `allowedGenerationStyles`.

var allowedGenerationStyles: [ImagePlaygroundStyle]

A list of allowed generation styles to choose from in the playground.

var personalizationPolicy: ImagePlaygroundPersonalizationPolicy

The policy to apply when determining whether to include people in generated images.

