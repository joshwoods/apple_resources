

- os
- OSLogInt32ExtendedFormat
-  OSLogInt32ExtendedFormat.darwinMode 

Case

# OSLogInt32ExtendedFormat.darwinMode

A format that displays a 32-bit integer as a Darwin file mode.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case darwinMode
```

## Discussion

Use this option to format the interpolated value as a Darwin file mode, such as `-rwx------`. Because Darwin uses octal values to represent file modes numerically, pass an octal literal to the formatter. Alternatively, convert the octal value to its 32-bit integer equivalent and interpolate that instead. For more information about using octal literals, see Numeric Literals.

The following example formats the octal literal `0o700` using the `darwinMode` formatter:

```
// Create a logger with the specified subsystem and category.
let logger = Logger(subsystem: "com.example.OSLogValueFormatting",
                    category: "Formatter Output")

// Darwin uses octal values to represent file modes. Use Swift's
// support for octal literals to assign a file mode to a 32-bit 
// integer variable.
let value: Int32 = 0o700

// Write the value to the log using the specified format.
logger.info(".darwinMode output is \(value, format: .darwinMode)")
```

And the system writes the following message to the log:

```
[Formatter Output] .darwinMode formats the value as -rwx------
```

## See Also

### Getting the Formats

case ipv4Address

A format that displays a 32-bit integer as an IPv4 address.

case secondsSince1970

A format that displays a 32-bit integer as a date.

case darwinErrno

A format that displays a 32-bit integer as a Darwin error number.

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

