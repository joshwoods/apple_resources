

- os
- OSLogInt32ExtendedFormat
-  OSLogInt32ExtendedFormat.darwinSignal 

Case

# OSLogInt32ExtendedFormat.darwinSignal

A format that displays a 32-bit integer as a Darwin signal.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case darwinSignal
```

## Discussion

Use this option to format the interpolated value as a Darwin signal, such as `sigsegv: Segmentation fault`. The following example applies the `darwinSignal` formatter to the 32-bit integer value `25`:

```
// Create a logger with the specified subsystem and category.
let logger = Logger(subsystem: "com.example.OSLogValueFormatting",
                    category: "Formatter Output")

// Assign the value to interpolate.
let value: Int32 = 25

// Write the value to the log using the specified format.
logger.info(".darwinSignal output is \(value, format: .darwinSignal)")
```

And the system writes the following message to the log:

```
[Formatter Output] .darwinSignal output is [sigxfsz: Filesize limit exceeded]
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

