

- Application Services
- Speech Synthesis Manager
- VoiceDescription
-  script 

Instance Property

# script

The encoding code of the text that the voice can process.

macOS 10.0+

``` source
var script: Int16
```

## Discussion

Note that this field contains a 16-bit value. You can use any of the 16-bit values described in External String Encodings or CFStringBuiltInEncodings. However, if you need to use a 32-bit value, such as UTF8, you pass the value in the first array element of the reserved field, and you also need to specify `-1` or kCFStringEncodingInvalidId in the script field.

