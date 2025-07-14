

- Application Services
- Speech Synthesis Manager
- SpeechErrorInfo
-  count 

Instance Property

# count

The number of errors that have occurred in processing the current text buffer since the last call to the `GetSpeechInfo` function with the `soErrors` selector. Of these errors, you can find information about only the first and last error that occurred.

macOS 10.0+

``` source
var count: Int16
```

