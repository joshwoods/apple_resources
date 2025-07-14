

- Swift
- MainActor
-  shared 

Type Property

# shared

The shared actor instance that will be used to provide mutually-exclusive access to declarations annotated with the given global actor type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let shared: MainActor
```

## Discussion

The value of this property must always evaluate to the same actor instance.

