

- Core Media
- CMTime
-  negativeInfinity 

Type Property

# negativeInfinity

A value that represents negative infinity.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
static let negativeInfinity: CMTime
```

## Discussion

Don’t test a time against this constant using (time == negativeInfinity) because there are many times that are also negative infinity. Use CMTIME_IS_NEGATIVEINFINITY(_:) instead.

## See Also

### Constants

static let zero: CMTime

A value that represents time zero.

static let invalid: CMTime

A value that represents an invalid time.

static let indefinite: CMTime

A value that represents an indefinite time.

static let positiveInfinity: CMTime

A value that represents positive infinity.

