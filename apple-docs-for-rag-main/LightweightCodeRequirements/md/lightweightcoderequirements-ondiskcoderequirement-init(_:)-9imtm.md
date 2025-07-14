

- LightweightCodeRequirements
- OnDiskCodeRequirement
-  init(\_:) 

Initializer

# init(\_:)

Convert a ProcessCodeRequirement to an OnDiskCodeRequirement if possible.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(_ processRequirement: ProcessCodeRequirement) throws
```

## Discussion

Conversion will fail if the ProcessCodeRequirement contains a constraint that cannot be converted to OnDiskConstraint.

