

- Foundation
- NSKeyedUnarchiver
-  init(forReadingFrom:) 

Initializer

# init(forReadingFrom:)

Initializes an archiver to decode data from the specified location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(forReadingFrom data: Data) throws
```

## Parameters 

`data`  

An archive previously encoded by NSKeyedArchiver.

## Discussion

This initializer enables requiresSecureCoding by default, and sets the decodingFailurePolicy to NSCoder.DecodingFailurePolicy.setErrorAndReturn.

Call finishDecoding() when you finish decoding data

This method throws an error if `data` isn’t a valid keyed archive.

Important

If you are adapting existing code to use this initializer, make sure you have adopted NSSecureCoding in the types you decode. If any call to a `decode`-prefixed method fails, the default decodingFailurePolicy sets the error rather than throwing an exception. In this case, the current and all subsequent decode calls return `0` or `nil`.

## See Also

### Creating a Keyed Unarchiver

init()

Initializes an archiver to decode data.

Deprecated

init(forReadingWith: Data)

Initializes an archiver to decode data from the specified location.

Deprecated

