

- Playground Support
-  PlaygroundValue 

Enumeration

# PlaygroundValue

The types you can save in the key-value store or send in messages to live views.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
enum PlaygroundValue
```

## Overview

The example below stores a dictionary in a `PlaygroundValue` instance and then stores the value in a PlaygroundKeyValueStore.

let myData = [
    &quot;animal&quot;: PlaygroundValue.string(&quot;Llama&quot;),
    &quot;count&quot;: PlaygroundValue.integer(5)
]

PlaygroundKeyValueStore.current.keyValueStore[&quot;AnimalCountDict&quot;] = .dictionary(myData)

For information about using `PlaygroundValue` instances to send messages, see Send and Receive Messages.

## Topics

### Representing Data

case boolean(Bool)

A value that represents a Boolean.

case data(Data)

A value that represents raw data.

case date(Date)

A value that represents a date.

case floatingPoint(Double)

A value that represents a floating-point number.

case integer(Int)

A value that represents an integer.

case string(String)

A value that represents a string.

### Representing Data Collections

case array([PlaygroundValue])

A value that represents an array that contains `PlaygroundValue` instances.

case dictionary([String : PlaygroundValue])

A value that represents a mapping from strings to `PlaygroundValue` instances.

## See Also

### Data Persistence

class PlaygroundKeyValueStore

A data storage container you use to persist information across different sessions.

let playgroundSharedDataDirectory: URL

The path to the directory containing data shared between all playgrounds in Xcode.

