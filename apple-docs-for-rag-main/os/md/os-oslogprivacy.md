

- os
-  OSLogPrivacy 

Structure

# OSLogPrivacy

The privacy options that determine when to redact or display values in log messages.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct OSLogPrivacy
```

## Overview

The OSLogPrivacy structure determines the visibility of interpolated values in log messages. Because people have access to log messages that your app generates, use the privacy options to hide potentially sensitive information. For example, you might use it to hide account information or personal data.

Use the available properties and methods to fetch an appropriately configured version of this structure, and pass it with your interpolated value in the log message. The following example shows how to mark a variable that contains the user’s bank account information as private:

```
Logger().info("User bank account number: \(accountNumber, privacy: .private)")
```

When you want to replace the generic redaction string with a hashed version of the original value, specify privacy options using the auto(mask:), private(mask:), and sensitive(mask:) methods. Using a hash string makes it possible to correlate log messages that contain the same original value, which helps you protect the user’s privacy and still diagnose issues surrounding a specific value.

## Topics

### Getting the Privacy Options

static var auto: OSLogPrivacy

The standard option to let the system determine whether to redact or display a value.

static var `private`: OSLogPrivacy

The standard option to always redact the interpolated value.

static var `public`: OSLogPrivacy

The standard option to always show the interpolated value.

static var sensitive: OSLogPrivacy

The option to always redact interpolated values that contain sensitive information.

### Creating a Custom Privacy Mask

static func auto(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that determines whether to redact or show values according to their type, and customizes the display of redacted values.

static func `private`(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that marks an interpolated value as private, and customizes the display of redacted values.

static func sensitive(mask: OSLogPrivacy.Mask) -> OSLogPrivacy

Returns a privacy structure that marks an interpolated value as sensitive, and customizes the display of redacted values.

enum Mask

A mask that establishes how the system displays a redacted value in a log message.

