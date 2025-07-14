

- TabletopKit
- TabletopAction
-  updateCounter(matching:value:context:) 

Type Method

# updateCounter(matching:value:context:)

visionOS 2.0+

``` source
static func updateCounter(
    matching counterID: ScoreCounter.Identifier,
    value: Int64,
    context: UInt64 = 0
) -> Self
```

Available when `Self` is `UpdateCounterAction`.

## See Also

### Keeping score

static func updateCounter(ScoreCounter, context: UInt64) -> Self

