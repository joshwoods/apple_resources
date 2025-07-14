

- Create ML Components
- RandomTransformer
-  Output 

Associated Type

# Output

The output type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
associatedtype Output
```

**Required**

## See Also

### Performing the transformation

func applied(to: Self.Input, generator: inout some RandomNumberGenerator, eventHandler: EventHandler?) async throws -> Self.Output

Performs the random transformation on a single input.

**Required**

associatedtype Input

The input type.

**Required**

