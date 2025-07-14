

- SwiftUI
- SceneStorage
-  init(\_:) 

Initializer

# init(\_:)

Creates a property that can save and restore an Optional boolean.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(_ key: String) where Value == Bool?
```

Available when `Value` conforms to `ExpressibleByNilLiteral`.

Show all declarations

## Parameters 

`key`  

A key used to save and restore the value.

## Discussion

Defaults to nil if there is no restored value

## See Also

### Storing a value

init(wrappedValue:_:)

Creates a property that can save and restore an integer, transforming it to a `RawRepresentable` data type.

