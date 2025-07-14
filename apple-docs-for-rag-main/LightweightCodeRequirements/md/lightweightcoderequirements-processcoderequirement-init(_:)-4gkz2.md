

- LightweightCodeRequirements
- ProcessCodeRequirement
-  init(\_:) 

Initializer

# init(\_:)

Convert a LaunchCodeRequirement to a ProcessCodeRequirement if possible.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(_ launchRequirement: LaunchCodeRequirement) throws
```

## Discussion

Conversion will fail if the LaunchCodeRequirement contains a constraint that cannot be converted to ProcessConstraint.

