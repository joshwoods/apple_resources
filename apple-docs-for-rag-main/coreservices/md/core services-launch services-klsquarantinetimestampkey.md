

- Core Services
- Launch Services
-  kLSQuarantineTimeStampKey 

Global Variable

# kLSQuarantineTimeStampKey

The date and time of the item’s quarantine.

macOS 10.5+

``` source
let kLSQuarantineTimeStampKey: CFString
```

## Discussion

When setting quarantine properties, this property is set automatically to the current date and time if this key is not present in the caller’s dictionary.

## See Also

### Understanding the Quarantine Properties Dictionary

let kLSQuarantineAgentBundleIdentifierKey: CFString

The bundle identifier of the quarantining agent.

let kLSQuarantineAgentNameKey: CFString

The app name of the quarantining agent.

let kLSQuarantineTypeKey: CFString

A symbolic string identifying the reason for the quarantine.

let kLSQuarantineDataURLKey: CFString

The actual URL of the quarantined item.

let kLSQuarantineOriginURLKey: CFString

The URL of the resource originally hosting the quarantined item.

