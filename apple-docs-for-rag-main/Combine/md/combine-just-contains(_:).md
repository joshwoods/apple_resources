

- Combine
- Just
-  contains(\_:) 

Instance Method

# contains(\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func contains(_ output: Output) -> Just
```

Available when `Output` conforms to `Equatable`.

## See Also

### Applying Matching Criteria to Elements

func contains(where: (Output) -> Bool) -> Just&lt;Bool>

func tryContains(where: (Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func allSatisfy((Output) -> Bool) -> Just&lt;Bool>

func tryAllSatisfy((Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

