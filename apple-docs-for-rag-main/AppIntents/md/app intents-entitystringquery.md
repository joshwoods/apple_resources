

- App Intents
-  EntityStringQuery 

Protocol

# EntityStringQuery

An interface that locates entities using arbitrary string input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol EntityStringQuery : EntityQuery
```

## Mentioned in 

Integrating custom data types into your intents

## Overview

EntityStringQuery adds to a EntityQuery the ability to query instances by `String`. The `String` value against which entities are matched typically represents the name a user would use to refer to a particular instance.

## Topics

### Searching for entities

func entities(matching: String) async throws -> Self.Result

Retrieves instances by string.

**Required**

## Relationships

### Inherits From

- DynamicOptionsProvider
- EntityQuery
- PersistentlyIdentifiable
- Sendable

