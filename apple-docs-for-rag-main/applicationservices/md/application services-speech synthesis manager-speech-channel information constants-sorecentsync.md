

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soRecentSync 

Global Variable

# soRecentSync

macOS 10.0+

``` source
var soRecentSync: OSType { get }
```

## Discussion

Get the message code for the most recentlyencountered synchronization command. If no synchronization commandhas been encountered, 0 is returned. The `speechInfo` parameteris a pointer to a variable of type `OSType`.

This selector works with the `GetSpeechInfo` function.

