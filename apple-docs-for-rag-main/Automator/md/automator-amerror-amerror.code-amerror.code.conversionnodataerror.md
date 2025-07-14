

- Automator
- AMError
- AMError.Code
-  AMError.Code.conversionNoDataError 

Case

# AMError.Code.conversionNoDataError

An error that occurs when the converter determines that the conversion, though possible, would produce a nil result.

Mac Catalyst 14.0+macOS 10.4+

``` source
case conversionNoDataError
```

## Discussion

This error isn’t displayed to the user.

## See Also

### Data Conversion Errors

case conversionFailedError

An error that occurs when, for example, the converter encounters an error converting data from one type to another.

case conversionNotPossibleError

An error that occurs when the converter determines that it is unable to convert from one data type to another.

