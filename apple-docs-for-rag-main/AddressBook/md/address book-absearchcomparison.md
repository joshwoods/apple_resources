

- Address Book
-  ABSearchComparison 

Type Alias

# ABSearchComparison

Constants used to specify the type of comparison beingmade.

macOS

``` source
typealias ABSearchComparison = CFIndex
```

## Discussion

These constants are used in a call to the ABGroupCreateSearchElement(_:_:_:_:_:) or ABPersonCreateSearchElement(_:_:_:_:_:) functionto specify the type of comparison being made.

## Topics

### Constants

var kABEqual: _ABSearchComparison

Search for elements that are equal to the value.

var kABNotEqual: _ABSearchComparison

Search for elements that are not equal to thevalue.

var kABNotEqualCaseInsensitive: _ABSearchComparison

Search for elements that are not equal to the value, ignoring case.

var kABLessThan: _ABSearchComparison

Search for elements that are less than thevalue.

var kABLessThanOrEqual: _ABSearchComparison

Search for elements that are less than or equalto the value.

var kABGreaterThan: _ABSearchComparison

Search for elements that are greater than thevalue.

var kABGreaterThanOrEqual: _ABSearchComparison

Search for elements that are greater than orequal to the value.

var kABEqualCaseInsensitive: _ABSearchComparison

Search for elements that are equal to the value,ignoring case.

var kABContainsSubString: _ABSearchComparison

Search for elements that contain the value.

var kABContainsSubStringCaseInsensitive: _ABSearchComparison

Search for elements that contain the value,ignoring case.

var kABPrefixMatch: _ABSearchComparison

Search for elements that begin with the value.

var kABPrefixMatchCaseInsensitive: _ABSearchComparison

Search for elements that begin with the value, ignoring case.

var kABSuffixMatch: _ABSearchComparison

Search for elements that end with the value.

var kABSuffixMatchCaseInsensitive: _ABSearchComparison

Search for elements that end with the value, ignoring case.

var kABBitsInBitFieldMatch: _ABSearchComparison

Search for elements that match the bits in ABPersonFlags.

var kABDoesNotContainSubString: _ABSearchComparison

Search for elements that do not contain the value.

var kABDoesNotContainSubStringCaseInsensitive: _ABSearchComparison

Search for elements that do not contain the value, ignoring case.

var kABWithinIntervalAroundToday: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward or backward from today.

var kABWithinIntervalAroundTodayYearless: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward or backward from this day in any year.

var kABNotWithinIntervalAroundToday: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward or backward from today.

var kABNotWithinIntervalAroundTodayYearless: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward or backward from this day in any year.

var kABWithinIntervalFromToday: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward from today.

var kABWithinIntervalFromTodayYearless: _ABSearchComparison

Search for elements that are within a time interval (in seconds) forward from this day in any year.

var kABNotWithinIntervalFromToday: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward from today.

var kABNotWithinIntervalFromTodayYearless: _ABSearchComparison

Search for elements that are *not* within a time interval (in seconds) forward from this day in any year.

## See Also

### Constants

typealias ABSearchConjunction

Constants used to create compound search elements.

