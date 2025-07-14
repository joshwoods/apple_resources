

- WatchKit
-  WKAudioRecorderControllerOptionsMaximumDurationKey 

Global Variable

# WKAudioRecorderControllerOptionsMaximumDurationKey

The maximum length of recorded audio clips. The value of this key is an NSNumber object with an TimeInterval value containing the maximum duration in seconds. If you do not specify this option, there is no maximum recording time.

watchOS 2.0+

``` source
let WKAudioRecorderControllerOptionsMaximumDurationKey: String
```

## See Also

### Constants

let WKAudioRecorderControllerOptionsActionTitleKey: String

The title to display on the button that the user taps to accept a recording. The value of this key is an NSString object. If you do not specify this option, the button title is set to “Save”.

let WKAudioRecorderControllerOptionsAlwaysShowActionTitleKey: String

The behavior for showing the action button. The value of this key is an NSNumber object with a Boolean value. When the value is true, the recording interface always shows the action button. When the value is false, the sheet shows the button only after the user has recorded some audio. The default value for this option is YES.

let WKAudioRecorderControllerOptionsAutorecordKey: String

The automatic recording behavior of the action sheet. The value of this key is an NSNumber object with a Boolean value. When the value is true, the recording interface starts recording as soon as it is presented. When the value is false, the user must start recording manually. The default value for this option is true.

