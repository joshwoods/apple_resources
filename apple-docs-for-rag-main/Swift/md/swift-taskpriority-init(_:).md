

- Swift
- TaskPriority
-  init(\_:) 

Initializer

# init(\_:)

Convert this `UnownedJob/Priority` to a TaskPriority.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init?(_ p: JobPriority)
```

## Discussion

Most values are directly interchangeable, but this initializer reserves the right to fail for certain values.

