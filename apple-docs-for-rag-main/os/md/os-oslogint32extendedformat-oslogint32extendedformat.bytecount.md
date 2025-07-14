

- os
- OSLogInt32ExtendedFormat
-  OSLogInt32ExtendedFormat.byteCount 

Case

# OSLogInt32ExtendedFormat.byteCount

A format that displays a 32-bit integer as bytes.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case byteCount
```

## Discussion

Use this option to format the interpolated value as bytes, such as `100 kB`. The following example applies the `byteCount` formatter to the 32-bit integer value `100_000`:

```
// Create a logger with the specified subsystem and category.
let logger = Logger(subsystem: "com.example.OSLogValueFormatting",
                    category: "Formatter Output")

// Assign the value to interpolate.
let value: Int32 = 100_000

// Write the value to the log using the specified format.
logger.info(".byteCount output is \(value, format: .byteCount)")
```

And the system writes the folllowing message to the log:

```
[Formatter Output] .byteCount output is 100 kB
```

## See Also

### Getting the Formats

case ipv4Address

A format that displays a 32-bit integer as an IPv4 address.

case secondsSince1970

A format that displays a 32-bit integer as a date.

case darwinErrno

A format that displays a 32-bit integer as a Darwin error number.

case darwinMode

A format that displays a 32-bit integer as a Darwin file mode.

case darwinSignal

A format that displays a 32-bit integer as a Darwin signal.

case bitrate

A format that displays a 32-bit integer as a bit rate.

case bitrateIEC

A format that displays a 32-bit integer as an IEC bit rate.

case byteCountIEC

A format that displays a 32-bit integer as IEC bytes.

case truth

A format that displays a 32-bit integer as true or false.

case answer

A format that displays a 32-bit integer as yes or no.

