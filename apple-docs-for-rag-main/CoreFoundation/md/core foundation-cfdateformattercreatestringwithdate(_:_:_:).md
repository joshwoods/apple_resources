

- Core Foundation
-  CFDateFormatterCreateStringWithDate(\_:\_:\_:) 

Function

# CFDateFormatterCreateStringWithDate(\_:\_:\_:)

Returns a string representation of the given date using the specified date formatter.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFDateFormatterCreateStringWithDate(
    _ allocator: CFAllocator!,
    _ formatter: CFDateFormatter!,
    _ date: CFDate!
) -> CFString!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`formatter`  

The date formatter object that specifies the format of the returned string.

`date`  

The date object for which to create a string representation.

## Return Value

A new string that represents `date` in the specified format. Returns `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating Strings From Data

func CFDateFormatterCreateStringWithAbsoluteTime(CFAllocator!, CFDateFormatter!, CFAbsoluteTime) -> CFString!

Returns a string representation of the given absolute time using the specified date formatter.

func CFDateFormatterCreateDateFormatFromTemplate(CFAllocator!, CFString!, CFOptionFlags, CFLocale!) -> CFString!

Returns a localized date format string representing the given date format components arranged appropriately for the specified locale.

