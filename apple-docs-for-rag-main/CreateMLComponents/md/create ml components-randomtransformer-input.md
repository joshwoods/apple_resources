

- Create ML Components
- RandomTransformer
-  Input 

Associated Type

# Input

The input type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
associatedtype Input
```

**Required**

## See Also

### Performing the transformation

func applied(to: Self.Input, generator: inout some RandomNumberGenerator, eventHandler: EventHandler?) async throws -> Self.Output

Performs the random transformation on a single input.

**Required**

associatedtype Output

The output type.

**Required**

