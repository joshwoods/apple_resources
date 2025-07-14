

- WebKit JS
- MouseEvent
-  initMouseEvent 

Instance Method

# initMouseEvent

Safari Desktop 3.0+Safari Mobile 1.0+

**Safari Desktop**

``` source
void initMouseEvent(
    optional DOMString type, 
    optional boolean canBubble, 
    optional boolean cancelable, 
    optional DOMWindow? view, 
    optional long detail, 
    optional long screenX, 
    optional long screenY, 
    optional long clientX, 
    optional long clientY, 
    optional boolean ctrlKey, 
    optional boolean altKey, 
    optional boolean shiftKey, 
    optional boolean metaKey, 
    optional unsigned short button, 
    optional any relatedTarget
);
```

**Safari Mobile**

``` source
void initMouseEvent(
    optional DOMString type, 
    optional boolean canBubble, 
    optional boolean cancelable, 
    optional DOMWindow? view, 
    optional long detail, 
    optional long screenX, 
    optional long screenY, 
    optional long clientX, 
    optional long clientY, 
    optional boolean ctrlKey, 
    optional boolean altKey, 
    optional boolean shiftKey, 
    optional boolean metaKey, 
    optional unsigned short button, 
    optional EventTarget? relatedTarget
);
```

