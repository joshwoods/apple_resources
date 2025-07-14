

- Core NFC
-  NFCMiFareTag 

Protocol

# NFCMiFareTag

An interface for interacting with a MIFARE® tag.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
protocol NFCMiFareTag : NFCNDEFTag, __NFCTag
```

## Overview

The NFCTagReaderSessionDelegate receives an object that conforms to the NFCMiFareTag protocol when the NFCTagReaderSession detects a compatible tag. However, if you include the application identifier `D2760000850101`—the identifier for the NDEF application on MIFARE® DESFire® tags (NFC Forum T4T tag platform)—in the com.apple.developer.nfc.readersession.iso7816.select-identifiers array of your `Info.plist` file, the reader session sends the delegate an NFCISO7816Tag object when it finds a tag matching the identifier. To receive the MIFARE DESFire tag as an NFCMiFareTag object, don’t include `D2760000850101` in the array.

For the delegate to receive the tag object, your app must include the Near Field Communication Tag Reader Session Formats Entitlement.

For the reader session to read and write data to the tag, it must be available to the reader session. Use the isAvailable property to check the tag’s availability.

MIFARE, MIFARE DESFire, MIFARE Ultralight, and MIFARE Plus are registered trademarks of NXP B.V.

## Topics

### Getting Tag Information

var mifareFamily: NFCMiFareFamily

The MIFARE product family identifier for the tag.

**Required**

enum NFCMiFareFamily

Identifiers for the MIFARE product families.

var identifier: Data

The unique hardware identifier of the tag.

**Required**

var historicalBytes: Data?

The historical bytes extracted from an Answer To Select response.

**Required**

### Sending Commands

func sendMiFareCommand(commandPacket: Data, completionHandler: (Data, (any Error)?) -> Void)

Sends a native MIFARE command to the tag.

**Required**

func sendMiFareISO7816Command(NFCISO7816APDU, completionHandler: (Data, UInt8, UInt8, (any Error)?) -> Void)

Sends an ISO 7816 command APDU to the tag and receives a response APDU.

**Required** Default implementation provided.

### Instance Methods

func sendMiFareCommand(commandPacket: Data, resultHandler: (Result&lt;Data, any Error>) -> Void)

func sendMiFareISO7816Command(NFCISO7816APDU, resultHandler: (Result&lt;NFCISO7816ResponseAPDU, any Error>) -> Void)

## Relationships

### Inherits From

- NFCNDEFTag
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Tag types

Creating NFC Tags from Your iPhone

Save data to tags, and interact with them using native tag protocols.

protocol NFCISO7816Tag

An interface for interacting with an ISO 7816 tag.

protocol NFCISO15693Tag

An interface for interacting with an ISO 15693 tag.

protocol NFCFeliCaTag

An interface for interacting with a FeliCa™ tag.

protocol NFCNDEFTag

An interface for interacting with an NDEF tag.

enum NFCTag

An object that represents an NFC tag object.

class NFCTagCommandConfiguration

A set of parameters you use to define the configuration of an NFC tag command.

