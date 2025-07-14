

- Apple Pay on the Web
-  ApplePayLaterAvailability Deprecated

Enumeration

# ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
enum ApplePayLaterAvailability
```

Deprecated

Apple Pay Later is deprecated.

## Overview

The following table describes the Apple Pay Later availability reasons.

| Availability reason | Description |
|----|----|
| `available` | Apple Pay Later is available.  This is the default. |
| `unavailableItemIneligible` | Apple Pay Later is unavailable because one or more ineligible or prohibited items are in the shopping cart, such as gift cards |
| `unavailableRecurringTransaction` | Apple Pay Later is unavailable because there’s a recurring payment or subscription in the shopping cart. |

Set the `applePayLaterAvailability` property to only one of these reasons as a string, for example:

```
applePayLaterAvailability = “unavailableRecurringTransaction”;
```

## Topics

### Enumeration Cases

available

unavailableItemIneligible

unavailableRecurringTransaction

## See Also

### Setting the Apple Pay Later mode

applePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

