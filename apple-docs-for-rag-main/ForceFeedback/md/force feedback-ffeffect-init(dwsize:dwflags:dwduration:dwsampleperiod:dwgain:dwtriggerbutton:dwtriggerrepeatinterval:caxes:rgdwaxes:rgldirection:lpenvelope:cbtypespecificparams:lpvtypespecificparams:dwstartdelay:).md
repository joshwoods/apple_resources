

- Force Feedback
- FFEFFECT
-  init(dwSize:dwFlags:dwDuration:dwSamplePeriod:dwGain:dwTriggerButton:dwTriggerRepeatInterval:cAxes:rgdwAxes:rglDirection:lpEnvelope:cbTypeSpecificParams:lpvTypeSpecificParams:dwStartDelay:) 

Initializer

# init(dwSize:dwFlags:dwDuration:dwSamplePeriod:dwGain:dwTriggerButton:dwTriggerRepeatInterval:cAxes:rgdwAxes:rglDirection:lpEnvelope:cbTypeSpecificParams:lpvTypeSpecificParams:dwStartDelay:)

Mac Catalyst 13.0+macOS 10.2+

``` source
init(
    dwSize: DWORD,
    dwFlags: DWORD,
    dwDuration: DWORD,
    dwSamplePeriod: DWORD,
    dwGain: DWORD,
    dwTriggerButton: DWORD,
    dwTriggerRepeatInterval: DWORD,
    cAxes: DWORD,
    rgdwAxes: LPDWORD!,
    rglDirection: LPLONG!,
    lpEnvelope: PFFENVELOPE!,
    cbTypeSpecificParams: DWORD,
    lpvTypeSpecificParams: UnsafeMutableRawPointer!,
    dwStartDelay: DWORD
)
```

## See Also

### Initializers

init()

