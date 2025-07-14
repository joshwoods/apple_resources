

- Audio Toolbox
- AUMessageChannel
-  callAudioUnit(\_:) 

Instance Method

# callAudioUnit(\_:)

Sends an audio unit a custom data message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
optional func callAudioUnit(_ message: [AnyHashable : Any]) -> [AnyHashable : Any]
```

## Parameters 

`message`  

The data to send the audio unit.

## Return Value

A dictionary with custom data.

## Discussion

The valid values for key and value types are `NSArray`, `NSDictionary`, `NSOrderedSet`, `NSSet`, `NSString`, `NSData`, `NSNull`, `NSNumber`, and `NSDate`.

