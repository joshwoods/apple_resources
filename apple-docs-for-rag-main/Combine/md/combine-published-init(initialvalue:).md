

- Combine
- Published
-  init(initialValue:) 

Initializer

# init(initialValue:)

Creates the published instance with an initial value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(initialValue: Value)
```

## Parameters 

`initialValue`  

The publisher’s initial value.

## Discussion

Don’t use this initializer directly. Instead, create a property with the `@Published` attribute, as shown here:

```
@Published var lastUpdated: Date = Date()
```

## See Also

### Creating a Published Instance

init(wrappedValue: Value)

Creates the published instance with an initial wrapped value.

