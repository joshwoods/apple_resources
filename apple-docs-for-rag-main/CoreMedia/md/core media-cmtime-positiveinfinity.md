

- Core Media
- CMTime
-  positiveInfinity 

Type Property

# positiveInfinity

A value that represents positive infinity.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
static let positiveInfinity: CMTime
```

## Discussion

Don’t test a time against this constant using (time == positiveInfinity) because there are many times that are also positive infinity. Use CMTIME_IS_POSITIVEINFINITY(_:) instead.

## See Also

### Constants

static let zero: CMTime

A value that represents time zero.

static let invalid: CMTime

A value that represents an invalid time.

static let indefinite: CMTime

A value that represents an indefinite time.

static let negativeInfinity: CMTime

A value that represents negative infinity.

