

- Core Foundation
- CFDateFormatter
-  Date Formatter Styles 

API Collection

# Date Formatter Styles

Predefined date and time format styles.

## Overview

The format for these date and time styles is not exact because they depend on the locale, user preference settings, and the operating system version. Do not use these constants if you want an exact format, for example if you are parsing an external data file which contains date information in a fixed format. There are several different “lengths” of the formats:

- “long” era names, for example “Anno Domini” instead of “AD”

- “very short” names for months and weekdays; for example, “F” instead of “Friday”

- “standalone” names for months and weekdays (for some locales or languages, a month name displayed in isolation needs to be written differently than a month name within a displayed date)

- names of quarters; for example, “Q2” for a short quarter name

## Topics

### Constants

case noStyle

Specifies no output.

case shortStyle

Specifies a short style, typically numeric only, such as “11/23/37” or “3:30pm”.

case mediumStyle

Specifies a medium style, typically with abbreviated text, such as “Nov 23, 1937”.

case longStyle

Specifies a long style, typically with full text, such as “November 23, 1937” or “3:30:32pm”.

case fullStyle

Specifies a full style with complete details, such as “Tuesday, April 12, 1952 AD” or “3:30:42pm PST”.

## See Also

### Constants

Date Formatter Property Keys

Keys used in key-value pairs to discover and specify the value of date formatter properties—used in conjunction with CFDateFormatterCopyProperty(_:_:) and CFDateFormatterSetProperty(_:_:_:).

Calendar Names

Calendar names used by CFDateFormatter.

