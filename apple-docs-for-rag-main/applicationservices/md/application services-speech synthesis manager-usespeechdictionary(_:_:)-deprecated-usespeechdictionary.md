

- Application Services
- Speech Synthesis Manager
-  UseSpeechDictionary(\_:\_:) Deprecated

Function

# UseSpeechDictionary(\_:\_:)

Registers a speech dictionary with a speech channel.

macOS 10.5–13.0Deprecated

``` source
func UseSpeechDictionary(
    _ chan: SpeechChannel,
    _ speechDictionary: CFDictionary
) -> OSErr
```

## Parameters 

`chan`  

The speech channel with which the specified speech dictionary is to be registered.

`speechDictionary`  

A speech dictionary to be registered with the specified speech channel, represented as a `CFDictionary` object. See Speech Dictionary Keys for the keys you can use in the dictionary.

## Return Value

A result code. See Result Codes.

## Discussion

The UseSpeechDictionary function is the Core Foundation-based equivalent of the UseDictionary function.

The `UseSpeechDictionary` function registers the `CFDictionary` object referenced by the `speechDictionary` parameter with the speech channel referenced by the `chan` parameter. Speech dictionaries allow your application to override a synthesizer's default pronunciations of individual words, such as names with unusual spellings. A synthesizer will use whatever elements of the dictionary it considers useful in the speech conversion process. Some speech synthesizers might ignore certain types of dictionary entries.

Multiple dictionaries can be registered with a synthesizer. If the same word appears in multiple dictionaries, the synthesizer will use the one from the dictionary with the most recent date.

Note that because a speech dictionary is a `CFDictionary` object, it can be loaded from an XML-based property list file. An example of such a file is shown below:

&lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?>
&lt;!DOCTYPE plist PUBLIC &quot;-//Apple//DTD PLIST 1.0//EN&quot; &quot;http://www.apple.com/DTDs/PropertyList-1.0.dtd&quot;>
&lt;plist version=&quot;1.0&quot;>
&lt;dict>
    &lt;key>LocaleIdentifier&lt;/key>
    &lt;string>en_US&lt;/string>
    &lt;key>ModificationDate&lt;/key>
    &lt;string>2006-12-21 11:59:25 -0800&lt;/string>
    &lt;key>Pronunciations&lt;/key>
    &lt;array>
        &lt;dict>
            &lt;key>Phonemes&lt;/key>
            &lt;string>_hEY_yUW&lt;/string>
            &lt;key>Spelling&lt;/key>
            &lt;string>Hello&lt;/string>
        &lt;/dict>
    &lt;/array>
    &lt;key>Abbreviations&lt;/key>
    &lt;array>
        &lt;dict>
            &lt;key>Phonemes&lt;/key>
            &lt;string>_OW_sAEkz&lt;/string>
            &lt;key>Spelling&lt;/key>
            &lt;string>OSAX&lt;/string>
        &lt;/dict>
    &lt;/array>
&lt;/dict>
&lt;/plist>

After the `UseSpeechDictionary` function returns, your application is free to release the `CFDictionary` object referenced by the `speechDictionary` parameter.

