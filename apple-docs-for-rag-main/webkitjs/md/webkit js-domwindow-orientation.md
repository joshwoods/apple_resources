

- WebKit JS
- DOMWindow
-  orientation 

Instance Property

# orientation

Specifies the orientation of the device.

Safari Mobile 9.0+

``` source
readonly attribute long orientation;
```

## Discussion

This property is set to one of the values in Table 1. For example, if the user starts with the device in portrait orientation and then changes to landscape orientation by turning the device to the right, the window’s `orientation` property is set to `-90`. If the user instead changes to landscape by turning the device to the left, the window’s `orientation` property is set to `90`. The default value is `0`.

| Value | Description |
|----|----|
| `0` | Portrait orientation. This is the default value. |
| `-90` | Landscape orientation with the screen turned clockwise. |
| `90` | Landscape orientation with the screen turned counterclockwise. |
| `180` | Portrait orientation with the screen turned upside down. This value is currently not supported on iPhone. |

**Table 1** Window orientation values

## See Also

### Getting Orientation and Motion Events

ondevicemotion

The event listener that is called when the device motion changes.

ondeviceorientation

The event listener that is called while the device orientation changes around the x, y, and z axes.

