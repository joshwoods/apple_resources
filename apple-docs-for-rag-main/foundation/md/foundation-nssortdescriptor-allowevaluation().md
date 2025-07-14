

- Foundation
- NSSortDescriptor
-  allowEvaluation() 

Instance Method

# allowEvaluation()

Forces a securely decoded sort descriptor to allow evaluation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func allowEvaluation()
```

## Discussion

When securely decoding NSSortDescriptor objects that are encoded using NSSecureCoding, evaluation is disabled because it is potentially unsafe to evaluate descriptors you get out of an archive.

Before you enable evaluation, you should validate key paths, selectors, and related properties to ensure no erroneous or malicious code will be executed. Once you’ve preflighted the sort descriptor, you can enable the sort descriptor for evaluation by calling allowEvaluation().

## See Also

### Using Sort Descriptors

func compare(Any, to: Any) -> ComparisonResult

Returns a comparison result value that indicates the sort order of two objects.

var reversedSortDescriptor: Any

Returns a sort descriptor that reverses the sort order.

