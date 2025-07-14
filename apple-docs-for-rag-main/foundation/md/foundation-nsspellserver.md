

- Foundation
-  NSSpellServer 

Class

# NSSpellServer

A server that your app uses to provide a spell checker service to other apps running in the system.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSSpellServer
```

## Overview

A **service provider** is an application that declares its availability in a standard way, so that any other applications that wish to use it can do so. If you build a spelling checker that makes use of the NSSpellServer class and list it as an available service, then users of any application that makes use of NSSpellChecker or includes a Services menu will see your spelling checker as one of the available dictionaries.

## Topics

### Configuring Spelling Servers

var delegate: (any NSSpellServerDelegate)?

Returns the receiver’s delegate.

### Providing Spelling Services

func registerLanguage(String?, byVendor: String?) -> Bool

Notifies the receiver of a language your spelling checker can check.

func run()

Causes the receiver to start listening for spell-checking requests.

### Managing the Spell-Checking Process

func isWord(inUserDictionaries: String, caseSensitive: Bool) -> Bool

Indicates whether a given word is in the user’s list of learned words or the document’s list of words to ignore.

### Constants

Grammatical-Analysis Details

These constants are used as the keys in the outDetails dictionaries returned by NSSpellServer and checkGrammar(of:startingAt:language:wrap:inSpellDocumentWithTag:details:) (NSSpellChecker).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Spelling and Grammar

protocol NSSpellServerDelegate

The optional methods implemented by the delegate of a spell server.

