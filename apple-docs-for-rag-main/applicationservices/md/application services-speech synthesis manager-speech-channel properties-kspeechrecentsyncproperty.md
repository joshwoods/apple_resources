

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechRecentSyncProperty 

Global Variable

# kSpeechRecentSyncProperty

Get the message code for the most recently encountered synchronization command.

macOS 10.5+

``` source
let kSpeechRecentSyncProperty: CFString
```

## Discussion

The value associated with this property is a `CFNumber` object that specifies the most recently encountered synchronization command. This property works with the CopySpeechProperty(_:_:_:) function.

