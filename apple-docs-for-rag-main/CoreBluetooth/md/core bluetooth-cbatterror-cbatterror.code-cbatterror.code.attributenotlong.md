

- Core Bluetooth
- CBATTError
- CBATTError.Code
-  CBATTError.Code.attributeNotLong 

Case

# CBATTError.Code.attributeNotLong

The ATT read blob request can’t read or write the attribute.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
case attributeNotLong
```

## See Also

### Error Codes

case success

The ATT command or request successfully completed.

case invalidHandle

The attribute handle is invalid on this peripheral.

case readNotPermitted

The permissions prohibit reading the attribute’s value.

case writeNotPermitted

The permissions prohibit writing the attribute’s value.

case invalidPdu

The attribute Protocol Data Unit (PDU) is invalid.

case insufficientAuthentication

Reading or writing the attribute’s value failed for lack of authentication.

case requestNotSupported

The attribute server doesn’t support the request received from the client.

case invalidOffset

The specified offset value was past the end of the attribute’s value.

case insufficientAuthorization

Reading or writing the attribute’s value failed for lack of authorization.

case prepareQueueFull

The prepare queue is full, as a result of there being too many write requests in the queue.

case attributeNotFound

The attribute wasn’t found within the specified attribute handle range.

case insufficientEncryptionKeySize

The encryption key size used for encrypting this link is insufficient.

case invalidAttributeValueLength

The length of the attribute’s value is invalid for the intended operation.

case unlikelyError

The ATT request encountered an unlikely error and wasn’t completed.

case insufficientEncryption

Reading or writing the attribute’s value failed for lack of encryption.

