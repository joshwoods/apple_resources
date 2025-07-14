

- os
- OSLogInt32ExtendedFormat
-  OSLogInt32ExtendedFormat.bitrate 

Case

# OSLogInt32ExtendedFormat.bitrate

A format that displays a 32-bit integer as a bit rate.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case bitrate
```

## Discussion

Use this option to format the interpolated value as a bit rate, such as `100 kbps`. The following example applies the `bitrate` formatter to the 32-bit integer value `100_000`:

```
// Create a logger with the specified subsystem and category.
let logger = Logger(subsystem: "com.example.OSLogValueFormatting",
                    category: "Formatter Output")

// Assign the value to interpolate.
let value: Int32 = 100_000

// Write the value to the log using the specified format.
logger.info(".bitrate output is \(value, format: .bitrate)")
```

And the system writes the following message to the log:

```
[Formatter Output] .bitrate output is 100 kbps
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

case bitrateIEC

A format that displays a 32-bit integer as an IEC bit rate.

case byteCount

A format that displays a 32-bit integer as bytes.

case byteCountIEC

A format that displays a 32-bit integer as IEC bytes.

case truth

A format that displays a 32-bit integer as true or false.

case answer

A format that displays a 32-bit integer as yes or no.

