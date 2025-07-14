

- SwiftUI
-  TimeDataSource 

Structure

# TimeDataSource

A source of time related data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TimeDataSource
```

## Overview

Instances of this type provide Text with live and automatically updating values in Widgets, Live Activities, watchOS Complications, and of course regular apps.

## Topics

### Type Properties

static var currentDate: TimeDataSource&lt;Date>

A time data source that produces `Date.now`.

### Type Methods

static func dateRange(endingAt: Date) -> TimeDataSource&lt;Range&lt;Date>>

A time data source that produces `min(date, Date.now)..

static func dateRange(startingAt: Date) -> TimeDataSource&lt;Range&lt;Date>>

A time data source that produces `date..

static func durationOffset(to: Date) -> TimeDataSource&lt;Duration>

A time data source that produces the offset between `Date.now` and the given `date` as a `Duration`.

## Relationships

### Conforms To

- Sendable

## See Also

### Formatting date and time

enum SystemFormatStyle

A namespace for format styles that implement designs used across Apple’s platformes.

