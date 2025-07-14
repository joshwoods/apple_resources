

- Application Services
- Speech Synthesis Manager
- Speech-Channel Information Constants
-  soCommandDelimiter 

Global Variable

# soCommandDelimiter

macOS 10.0+

``` source
var soCommandDelimiter: OSType { get }
```

## Discussion

Set the embedded speech command delimiter characters to be used for the speech channel. By default the opening delimiter is “`[[`” and the closing delimiter is “`]]`”. Your application might need to change these delimiters temporarily if those character sequences occur naturally in a text buffer that is to be spoken. Your application can also disable embedded command processing by passing empty delimiters (using two `NUL` ASCII characters).The `speechInfo` parameter is a pointer to a delimiter information structure, described in DelimiterInfo.

This selector works with the `SetSpeechInfo` function.

