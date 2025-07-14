

- Media Player
- MPMusicPlayerPlayParameters
-  init(dictionary:) 

Initializer

# init(dictionary:)

Returns a new play parameters object using information from MusicKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
init?(dictionary: [String : Any])
```

## Parameters 

`dictionary`  

The JSON information returned from a MusicKit query.

## Return Value

A new play parameters object consisting of the information retrieved from MusicKit.

## Discussion

Create a new `MPMusicPlayerPlayParameters` object using the JSON information returned from a MusicKit query.

