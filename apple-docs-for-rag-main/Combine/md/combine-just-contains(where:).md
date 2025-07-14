

- Combine
- Just
-  contains(where:) 

Instance Method

# contains(where:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func contains(where predicate: (Output) -> Bool) -> Just
```

## See Also

### Applying Matching Criteria to Elements

func contains(Output) -> Just&lt;Bool>

func tryContains(where: (Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func allSatisfy((Output) -> Bool) -> Just&lt;Bool>

func tryAllSatisfy((Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

