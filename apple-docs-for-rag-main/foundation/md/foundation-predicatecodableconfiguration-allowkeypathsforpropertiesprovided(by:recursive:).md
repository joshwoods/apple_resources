

- Foundation
- PredicateCodableConfiguration
-  allowKeyPathsForPropertiesProvided(by:recursive:) 

Instance Method

# allowKeyPathsForPropertiesProvided(by:recursive:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func allowKeyPathsForPropertiesProvided(
    by type: T.Type,
    recursive: Bool = false
) where T : PredicateCodableKeyPathProviding
```

## See Also

### Allowing types and key paths

func allow(PredicateCodableConfiguration)

func allowPartialType(any Any.Type, identifier: String)

func allowType(any Any.Type, identifier: String?)

