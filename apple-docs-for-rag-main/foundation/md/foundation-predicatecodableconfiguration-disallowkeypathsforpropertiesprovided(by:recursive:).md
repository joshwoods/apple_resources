

- Foundation
- PredicateCodableConfiguration
-  disallowKeyPathsForPropertiesProvided(by:recursive:) 

Instance Method

# disallowKeyPathsForPropertiesProvided(by:recursive:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
mutating func disallowKeyPathsForPropertiesProvided(
    by type: T.Type,
    recursive: Bool = false
) where T : PredicateCodableKeyPathProviding
```

## See Also

### Disallowing types and key paths

func disallowPartialType(any Any.Type)

func disallowType(any Any.Type)

