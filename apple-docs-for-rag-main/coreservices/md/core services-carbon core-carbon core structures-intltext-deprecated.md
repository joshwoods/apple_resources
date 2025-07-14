

- Core Services
- Carbon Core
- Carbon Core Structures
-  IntlText Deprecated

Structure

# IntlText

International text consists of an ordered series of bytes, beginning with a 4-byte language code and a 4-byte script code that together determine the format of the bytes that follow.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct IntlText
```

Deprecated

Use Unicode text instead.

## Topics

### Initializers

init()

init(theScriptCode: ScriptCode, theLangCode: LangCode, theText: CChar)

### Instance Properties

var theLangCode: LangCode

var theScriptCode: ScriptCode

var theText: CChar

