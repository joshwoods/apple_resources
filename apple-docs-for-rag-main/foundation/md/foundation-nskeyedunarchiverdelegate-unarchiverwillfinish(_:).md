

- Foundation
- NSKeyedUnarchiverDelegate
-  unarchiverWillFinish(\_:) 

Instance Method

# unarchiverWillFinish(\_:)

Notifies the delegate that decoding is about to finish.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func unarchiverWillFinish(_ unarchiver: NSKeyedUnarchiver)
```

## Parameters 

`unarchiver`  

An unarchiver for which the receiver is the delegate.

## See Also

### Finishing Decoding

func unarchiverDidFinish(NSKeyedUnarchiver)

Notifies the delegate that decoding has finished.

