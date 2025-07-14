

- Core Media
- CMTime
-  invalid 

Type Property

# invalid

A value that represents an invalid time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
static let invalid: CMTime
```

## Discussion

An invalid time has all of its fields set to `0`.

Don’t test a time against this constant using (time == invalid) because there are many times that are also invalid. Use CMTIME_IS_INVALID(_:) instead.

## See Also

### Constants

static let zero: CMTime

A value that represents time zero.

static let indefinite: CMTime

A value that represents an indefinite time.

static let negativeInfinity: CMTime

A value that represents negative infinity.

static let positiveInfinity: CMTime

A value that represents positive infinity.

