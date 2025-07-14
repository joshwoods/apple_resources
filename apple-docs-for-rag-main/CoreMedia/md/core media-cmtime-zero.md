

- Core Media
- CMTime
-  zero 

Type Property

# zero

A value that represents time zero.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
static let zero: CMTime
```

## Discussion

Don’t test a time against this constant using (time == zero) because there are many times that are also `0`. Use CMTimeCompare(_:_:) instead.

## See Also

### Constants

static let invalid: CMTime

A value that represents an invalid time.

static let indefinite: CMTime

A value that represents an indefinite time.

static let negativeInfinity: CMTime

A value that represents negative infinity.

static let positiveInfinity: CMTime

A value that represents positive infinity.

