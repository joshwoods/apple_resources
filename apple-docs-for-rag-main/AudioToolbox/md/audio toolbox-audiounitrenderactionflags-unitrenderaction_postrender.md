

- Audio Toolbox
- AudioUnitRenderActionFlags
-  unitRenderAction_PostRender 

Type Property

# unitRenderAction_PostRender

Called on a render notification Proc - which is called either before or after the render operation of the audio unit. If this flag is set, the proc is being called after the render operation is completed.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
static var unitRenderAction_PostRender: AudioUnitRenderActionFlags { get }
```

## See Also

### Constants

static var unitRenderAction_PreRender: AudioUnitRenderActionFlags

Called on a render notification Proc - which is called either before or after the render operation of the audio unit. If this flag is set, the proc is being called before the render operation is performed.

static var unitRenderAction_OutputIsSilence: AudioUnitRenderActionFlags

This flag can be set in a render input callback (or in the audio unit’s render operation itself) and is used to indicate that the render buffer contains only silence. It can then be used by the caller as a hint to whether the buffer needs to be processed or not.

static var offlineUnitRenderAction_Preflight: AudioUnitRenderActionFlags

This is used with offline audio units (of type `'auol'`). It is used when an offline unit is being preflighted, which is performed prior to the actual offline rendering actions are performed. It is used for those cases where the offline process needs it (for example, with an offline unit that normalizes an audio file, it needs to see all of the audio data first before it can perform its normalization).

static var offlineUnitRenderAction_Render: AudioUnitRenderActionFlags

Once an offline unit has been successfully preflighted, it is then put into its render mode. So this flag is set to indicate to the audio unit that it is now in that state and that it should perform its processing on the input data.

static var offlineUnitRenderAction_Complete: AudioUnitRenderActionFlags

This flag is set when an offline unit has completed either its preflight or performed render operation.

static var unitRenderAction_PostRenderError: AudioUnitRenderActionFlags

If this flag is set on the post-render call an error was returned by the audio unit’s render operation. In this case, the error can be retrieved through the lastRenderError property and the audio data in `ioData` handed to the post-render notification will be invalid.

static var unitRenderAction_DoNotCheckRenderArgs: AudioUnitRenderActionFlags

If this flag is set, then checks that are done on the arguments provided to render are not performed. This can be useful to use to save computation time in situations where you are sure you are providing the correct arguments and structures to the various render calls.

