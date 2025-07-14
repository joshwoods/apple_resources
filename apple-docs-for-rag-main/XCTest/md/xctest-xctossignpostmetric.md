

- XCTest
-  XCTOSSignpostMetric 

Class

# XCTOSSignpostMetric

A metric to record the time that a performance test spends executing a signposted region of code.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class XCTOSSignpostMetric
```

## Overview

This metric captures the time that elapses between the begin and end events for a specific named os_signpost(_:dso:log:name:signpostID:) region. It doesn’t record any results when there isn’t a matching pair of `begin` and `end` events.

## Topics

### Measuring Specific Signposts

init(subsystem: String, category: String, name: String)

Creates a metric to record a specific signpost.

### Measuring Navigation Transitions

class var customNavigationTransitionMetric: any XCTMetric

A metric that records the duration of custom navigation transitions between views.

class var navigationTransitionMetric: any XCTMetric

A metric that records the duration of navigation transitions between views.

### Measuring Scrolling Properties

class var scrollingAndDecelerationMetric: any XCTMetric

A metric that records scroll-dragging and deceleration animations.

### Deprecated

class var applicationLaunch: XCTOSSignpostMetric

A metric that records the time that elapses during app launch.

Deprecated

class var scrollDecelerationMetric: any XCTMetric

A metric that records scroll deceleration animations.

Deprecated

class var scrollDraggingMetric: any XCTMetric

A metric that records scroll-dragging animations.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- XCTMetric

## See Also

### Measurement Metrics

protocol XCTMetric

A protocol that defines the methods that objects must provide when gathering metrics during performance tests.

class XCTCPUMetric

A metric to record information about CPU activity during a performance test.

class XCTClockMetric

A metric to record the time that elapses during a performance test.

class XCTMemoryMetric

A metric to record the physical memory that a performance test uses.

class XCTStorageMetric

A metric to record the amount of data that a performance test logically writes to storage.

class XCTApplicationLaunchMetric

A metric to record the application launch duration for a performance test.

