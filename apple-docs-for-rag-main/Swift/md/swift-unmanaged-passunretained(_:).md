

- Swift
- Unmanaged
-  passUnretained(\_:) 

Type Method

# passUnretained(\_:)

Creates an unmanaged reference without performing an unbalanced retain.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func passUnretained(_ value: Instance) -> Unmanaged
```

## Parameters 

`value`  

A class instance.

## Return Value

An unmanaged reference to the object passed as `value`.

## Discussion

This is useful when passing a reference to an API which Swift does not know the ownership rules for, but you know that the API expects you to pass the object at +0.

```
CFArraySetValueAtIndex(.passUnretained(array), i,
                       .passUnretained(object))
```

