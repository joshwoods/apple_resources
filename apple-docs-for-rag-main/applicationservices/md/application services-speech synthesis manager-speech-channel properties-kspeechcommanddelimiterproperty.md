

- Application Services
- Speech Synthesis Manager
- Speech-Channel Properties
-  kSpeechCommandDelimiterProperty 

Global Variable

# kSpeechCommandDelimiterProperty

Set the embedded speech command delimiter characters to be used for the speech channel.

macOS 10.5+

``` source
let kSpeechCommandDelimiterProperty: CFString
```

## Discussion

By default, the opening delimiter is “`[[`” and the closing delimiter is “`]]`”. Your application might need to change these delimiters temporarily if those character sequences occur naturally in a text buffer that is to be spoken. Your application can also disable embedded command processing by passing empty delimiters (as empty strings). The value associated with this property is a `CFDictionary` object that contains the delimiter information. See Command Delimiter Keys for the keys you can use to specify values in this dictionary.

This property works with the SetSpeechProperty(_:_:_:) function.

