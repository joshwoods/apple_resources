

- Core NFC
- NFCPresentmentIntentAssertion
-  acquire() 

Type Method

# acquire()

Acquire a presentment intent assertion instance from the system.

iOS 17.4+iPadOS 17.4+

``` source
static func acquire() async throws -> NFCPresentmentIntentAssertion
```

## Return Value

A presentment intent assertion instance you use to prevent the default contactless app from launching.

## Discussion

The returned object remains valid until any of the following occur:

- Your app goes into the background.

- The maximum presentment intent assertion duration expires.

- The object deinitializes.

If the system can’t create a presentment intent assertion object, this method throws an error of type NFCPresentmentIntentAssertion.Error.

Warning

Check to see if the device is capable of using NFC with the NFCReaderSession class property readingAvailable. Attempting to acquire a presentment intent assertion on a device that can’t use NFC raises fatalError(_:file:line:).

