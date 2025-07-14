

- Core Services
- Launch Services
-  kLSQuarantineAgentNameKey 

Global Variable

# kLSQuarantineAgentNameKey

The app name of the quarantining agent.

macOS 10.5+

``` source
let kLSQuarantineAgentNameKey: CFString
```

## Discussion

When setting quarantine properties, this agent name is set automatically to the current process name if this key is not present in the caller’s dictionary.

## See Also

### Understanding the Quarantine Properties Dictionary

let kLSQuarantineAgentBundleIdentifierKey: CFString

The bundle identifier of the quarantining agent.

let kLSQuarantineTimeStampKey: CFString

The date and time of the item’s quarantine.

let kLSQuarantineTypeKey: CFString

A symbolic string identifying the reason for the quarantine.

let kLSQuarantineDataURLKey: CFString

The actual URL of the quarantined item.

let kLSQuarantineOriginURLKey: CFString

The URL of the resource originally hosting the quarantined item.

