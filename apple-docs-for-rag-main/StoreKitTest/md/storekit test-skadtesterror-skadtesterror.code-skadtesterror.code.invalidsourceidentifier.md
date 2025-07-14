

- StoreKit Test
- SKAdTestError
- SKAdTestError.Code
-  SKAdTestError.Code.invalidSourceIdentifier 

Case

# SKAdTestError.Code.invalidSourceIdentifier

The postback’s identifier isn’t two, three, or four digits.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+

``` source
case invalidSourceIdentifier
```

## Discussion

A valid postback includes two to four digits of the impression’s sourceIdentifier. For more information about the varying length of source identifiers, see Receiving postbacks in multiple conversion windows.

## See Also

### Other Errors

case invalidVersion

A postback contains an incorrect version number.

case invalidImpressionId

The impression ID isn’t a valid UUID string.

case invalidSourceAppAdamId

The app ID is less than zero.

case invalidSourceDomain

The source domain isn’t in the correct format.

case unknownError

An unknown error occurred in the testing environment.

case invalidVersion

A postback contains an incorrect version number.

case invalidImpressionId

The impression ID isn’t a valid UUID string.

case invalidSourceAppAdamId

The app ID is less than zero.

case invalidSourceDomain

The source domain isn’t in the correct format.

case unknownError

An unknown error occurred in the testing environment.

