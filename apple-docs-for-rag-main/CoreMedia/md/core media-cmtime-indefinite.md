

- Core Media
- CMTime
-  indefinite 

Type Property

# indefinite

A value that represents an indefinite time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
static let indefinite: CMTime
```

## Discussion

Don’t test a time against this constant using (`time ==` indefinite) because there are many that are also indefinite. Use CMTIME_IS_INDEFINITE(_:) instead.

## See Also

### Constants

static let zero: CMTime

A value that represents time zero.

static let invalid: CMTime

A value that represents an invalid time.

static let negativeInfinity: CMTime

A value that represents negative infinity.

static let positiveInfinity: CMTime

A value that represents positive infinity.

