

- SwiftUI
- FocusedValue
-  init(\_:) 

Initializer

# init(\_:)

A new property wrapper for the given key path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(_ keyPath: KeyPath)
```

Show all declarations

## Parameters 

`keyPath`  

The key path for the focus value to read.

## Discussion

The value of the property wrapper is updated dynamically as focus changes and different published values go in and out of scope.

