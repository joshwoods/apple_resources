

- Swift Testing
- TimeLimitTrait
-  TimeLimitTrait.Duration 

Structure

# TimeLimitTrait.Duration

A type representing the duration of a time limit applied to a test.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Swift 6.0+Xcode 16.0+

``` source
struct Duration
```

## Overview

This type is intended for use specifically for specifying test timeouts with TimeLimitTrait. It is used instead of Swift’s built-in `Duration` type because test timeouts do not support high-precision, arbitrarily short durations. The smallest allowed unit of time is minutes.

## Topics

### Type Methods

static func minutes(some BinaryInteger) -> TimeLimitTrait.Duration

Construct a time limit duration given a number of minutes.

## Relationships

### Conforms To

- Sendable

