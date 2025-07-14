

- CarPlay
- CPNowPlayingTemplate
-  add(\_:) 

Instance Method

# add(\_:)

Registers an observer that receives Now Playing template events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func add(_ observer: any CPNowPlayingTemplateObserver)
```

## Parameters 

`observer`  

An object that implements the CPNowPlayingTemplateObserver protocol.

## See Also

### Observing Now Playing Events

func remove(any CPNowPlayingTemplateObserver)

Removes an observer from receiving Now Playing template events.

protocol CPNowPlayingTemplateObserver

The methods for responding to the user interacting with the Now Playing template.

