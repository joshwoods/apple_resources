

- ClockKit
- CLKRelativeDateStyle
-  CLKRelativeDateStyle.naturalFull Deprecated

Case

# CLKRelativeDateStyle.naturalFull

A natural date style using unabbreviated units, when possible.

watchOS 6.0–9.0Deprecated

``` source
case naturalFull
```

## Discussion

The text provider breaks the time interval into various components. If there’s enough space, it uses the full word for the units; otherwise, it abbreviates them. For example, it formats 10 hours and 9 minutes as “10 hours 9 minutes”.

## See Also

### Date Styles

case natural

A natural date style.

Deprecated

case naturalAbbreviated

An abbreviated, natural date style.

Deprecated

case offset

An offset date style.

Deprecated

case offsetShort

A short offset date style.

Deprecated

case timer

A timer style.

Deprecated

