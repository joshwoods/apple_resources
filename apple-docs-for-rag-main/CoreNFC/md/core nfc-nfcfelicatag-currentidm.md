

- Core NFC
- NFCFeliCaTag
-  currentIDm 

Instance Property

# currentIDm

The manufacturer identifier for the system currently selected by the reader session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var currentIDm: Data { get }
```

**Required**

## Discussion

The reader session updates currentIDm each time your app calls the polling(systemCode:requestCode:timeSlot:completionHandler:) method. The data contained in currentIDm is empty when the system selection fails.

## See Also

### Getting Current Information

var currentSystemCode: Data

The system code most recently selected by the reader session during a polling sequence.

**Required**

