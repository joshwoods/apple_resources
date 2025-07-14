

- AppKit
- NSTextAlternatives
-  noteSelectedAlternativeString(\_:) 

Instance Method

# noteSelectedAlternativeString(\_:)

Sent to the `NSTextAlternatives` object by the text view when the user chooses one of the alternative strings.

macOS 10.8+

``` source
func noteSelectedAlternativeString(_ alternativeString: String)
```

## Parameters 

`alternativeString`  

The alternative string chosen by the user.

## Discussion

The base class implementation sends a notification, `NSTextAlternativesSelectedAlternativeStringNotification`, with the selected alternative string in the user info under the key `@"NSAlternativeString"`. Using this mechanism, arbitrary objects can listen for user selections of alternative strings.

