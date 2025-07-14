

- CarPlay
- CPNowPlayingTemplate
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes an observer from receiving Now Playing template events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func remove(_ observer: any CPNowPlayingTemplateObserver)
```

## Parameters 

`observer`  

An object that implements the CPNowPlayingTemplateObserver protocol.

## Discussion

You must register an observer using the add(_:) method before calling this method.

## See Also

### Observing Now Playing Events

func add(any CPNowPlayingTemplateObserver)

Registers an observer that receives Now Playing template events.

protocol CPNowPlayingTemplateObserver

The methods for responding to the user interacting with the Now Playing template.

