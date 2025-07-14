

- Combine
- Just
-  tryContains(where:) 

Instance Method

# tryContains(where:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryContains(where predicate: (Output) throws -> Bool) -> Result.Publisher
```

## See Also

### Applying Matching Criteria to Elements

func contains(Output) -> Just&lt;Bool>

func contains(where: (Output) -> Bool) -> Just&lt;Bool>

func allSatisfy((Output) -> Bool) -> Just&lt;Bool>

func tryAllSatisfy((Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

