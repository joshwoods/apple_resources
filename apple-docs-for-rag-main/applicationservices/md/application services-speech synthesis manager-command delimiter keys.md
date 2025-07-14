

- Application Services
- Speech Synthesis Manager
-  Command Delimiter Keys 

API Collection

# Command Delimiter Keys

Keys used with the `kSpeechCommandDelimiterProperty` property to specify information about the command delimiter strings.

## Topics

### Constants

let kSpeechCommandPrefix: CFString

The command delimiter string that prefixes a command (by default, this is “`[[`”). The string should contain two or fewer characters, which, for best compatibility, should be ASCII characters.

let kSpeechCommandSuffix: CFString

The command delimiter string that suffixes a command (by default, this is “`]]`”). The string should contain two or fewer characters, which, for best compatibility, should be ASCII characters.

