

- SwiftUI
-  DynamicProperty 

Protocol

# DynamicProperty

An interface for a stored variable that updates an external property of a view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol DynamicProperty
```

## Overview

The view gives values to these properties prior to recomputing the view’s body.

## Topics

### Updating the value

func update()

Updates the underlying value of the stored value.

**Required** Default implementation provided.

## Relationships

### Conforming Types

- AccessibilityFocusState
- AppStorage
- Binding

  Conforms when `Value` conforms to `Copyable` and `Escapable`.

- Environment
- EnvironmentObject
- FetchRequest

  Conforms when `Result` conforms to `NSFetchRequestResult`.

- FocusState
- FocusedBinding
- FocusedObject
- FocusedValue
- GestureState
- NSApplicationDelegateAdaptor
- Namespace
- ObservedObject
- PhysicalMetric
- ScaledMetric
- SceneStorage
- SectionedFetchRequest

  Conforms when `SectionIdentifier` conforms to `Hashable` and `Result` conforms to `NSFetchRequestResult`.

- State
- StateObject
- UIApplicationDelegateAdaptor
- WKApplicationDelegateAdaptor
- WKExtensionDelegateAdaptor

