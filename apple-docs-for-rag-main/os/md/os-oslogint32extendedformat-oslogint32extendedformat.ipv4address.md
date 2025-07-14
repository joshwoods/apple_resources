

- os
- OSLogInt32ExtendedFormat
-  OSLogInt32ExtendedFormat.ipv4Address 

Case

# OSLogInt32ExtendedFormat.ipv4Address

A format that displays a 32-bit integer as an IPv4 address.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case ipv4Address
```

## Discussion

Use this option to format the interpolated value as an IPv4 address, such as `127.0.0.1`. The following example applies the `ipv4Address` formatter to the 32-bit integer value `0x0100007f`:

```
// Create a logger with the specified subsystem and category.
let logger = Logger(subsystem: "com.example.OSLogValueFormatting",
                    category: "Formatter Output")

// Assign the value to interpolate.
let value: Int32 = 0x0100007f

// Write the value to the log using the specified format.
logger.info(".ipv4Address output is \(value, format: .ipv4Address)")
```

And the system writes the following message to the log:

```
[Formatter Output] .ipv4Address output is 127.0.0.1
```

## See Also

### Getting the Formats

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

case byteCount

A format that displays a 32-bit integer as bytes.

case byteCountIEC

A format that displays a 32-bit integer as IEC bytes.

case truth

A format that displays a 32-bit integer as true or false.

case answer

A format that displays a 32-bit integer as yes or no.

