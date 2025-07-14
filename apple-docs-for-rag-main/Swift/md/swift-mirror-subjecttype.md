

- Swift
- Mirror
-  subjectType 

Instance Property

# subjectType

The static type of the subject being reflected.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let subjectType: any Any.Type
```

## Discussion

This type may differ from the subject’s dynamic type when this mirror is the `superclassMirror` of another mirror.

