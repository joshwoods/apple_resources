

- SwiftUI
- AppStorage
-  init(\_:store:) 

Initializer

# init(\_:store:)

Creates a property that can read and write an Optional boolean user default.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    _ key: String,
    store: UserDefaults? = nil
) where Value == Bool?
```

Available when `Value` conforms to `ExpressibleByNilLiteral`.

Show all declarations

## Parameters 

`key`  

The key to read and write the value to in the user defaults store.

`store`  

The user defaults store to read and write to. A value of `nil` will use the user default store from the environment.

## Discussion

Defaults to nil if there is no restored value.

## See Also

### Storing a value

init(wrappedValue:_:store:)

Creates a property that can save and restore tab sidebar customizations.

