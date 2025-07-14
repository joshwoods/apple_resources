

- Core NFC
-  NFCTag 

Enumeration

# NFCTag

An object that represents an NFC tag object.

iOS 13.0+iPadOS 13.0+Mac Catalyst

``` source
enum NFCTag
```

## Overview

When an NFC reader session detects a tag, it returns an NFCTag object. Use this generic object to determine if the tag is available, and to retrieve an object of a specific tag type.

Listing 1. Getting a MIFARE Ultralight tag from an array of generic tags objects

```
func tagReaderSession(_ session: NFCTagReaderSession, didDetect tags: [NFCTag]) {
    var tag: NFCTag? = nil

    for nfcTag in tags {
        // In this example you are searching for a MIFARE Ultralight tag (NFC Forum T2T tag platform).
        if case let .miFare(mifareTag) = nfcTag {
            if mifareTag.mifareFamily == .ultralight {
                tag = nfcTag
                break
            }
        }
    }

    if tag == nil {
        session.invalidate(errorMessage: "No valid coupon found.")
        return
    }

    session.connect(to: tag!) { (error: Error?) in
        if error != nil {
            session.invalidate(errorMessage: "Connection error. Please try again.")
            return
        }
        self.readCouponCode(from: tag!)
    }
}
```

## Topics

### Getting Information About a Tag

var isAvailable: Bool

A Boolean value that indicates whether a detected tag is available.

### Getting a Specific Tag Type

case iso15693(any NFCISO15693Tag)

Gets a tag as an ISO 15693 tag object.

case iso7816(any NFCISO7816Tag)

Gets a tag as an ISO 7816 tag object.

case feliCa(any NFCFeliCaTag)

Gets a tag as a FeliCa tag object.

case miFare(any NFCMiFareTag)

Get a tag as a MIFARE tag object.

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

protocol NFCMiFareTag

An interface for interacting with a MIFARE® tag.

protocol NFCNDEFTag

An interface for interacting with an NDEF tag.

class NFCTagCommandConfiguration

A set of parameters you use to define the configuration of an NFC tag command.

