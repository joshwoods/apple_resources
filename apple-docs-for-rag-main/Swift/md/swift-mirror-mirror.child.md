

- Swift
- Mirror
-  Mirror.Child 

Type Alias

# Mirror.Child

An element of the reflected instance’s structure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias Child = (label: String?, value: Any)
```

## Discussion

When the `label` component in not `nil`, it may represent the name of a stored property or an active `enum` case. If you pass strings to the `descendant(_:_:)` method, labels are used for lookup.

