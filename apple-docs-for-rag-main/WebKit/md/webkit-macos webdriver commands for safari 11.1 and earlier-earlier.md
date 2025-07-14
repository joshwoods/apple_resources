

- WebKit
-  macOS WebDriver Commands for Safari 11.1 and earlier 

Article

# macOS WebDriver Commands for Safari 11.1 and earlier

Test your web content using the WebDriver commands supported by Safari 11.1 and earlier.

## Overview

This table lists the method and the URI template (the *endpoint*) that executes each command. The macOS WebDriver Commands for Safari 11.1 and earlier supports the Selenium JSON Wire Protocol. The macOS WebDriver Commands for Safari 12 and later supports the the W3C WebDriver protocol.

All URI templates listed here work in Safari on macOS 10.11 and later.

Important

WebDriver for Safari supports file upload with the “Element Send Keys “ command. Uploaded files must be world-readable and must respect the `multiple` and `accept` attributes.

| Method | URI template | Supported | Safari Technology Preview release, Safari version |
|----|----|----|----|
| GET | /status | See note below |  |
| POST | /session | ✓ | 14, 10.0 |
| GET | /sessions | See note below |  |
| GET, DELETE | /session/:sessionId | ✓ | 14, 10.0 |
| POST, DELETE | /session/:sessionId/window | ✓ | 14, 10.0 |
| GET | /session/:sessionId/window_handle | ✓ | 14, 10.0 |
| GET | /session/:sessionId/window_handles | ✓ | 14, 10.0 |
| GET, POST | /session/:sessionId/window/:windowHandle/size | ✓ | 14, 10.0 |
| GET, POST | /session/:sessionId/window/:windowHandle/position | ✓ | 14, 10.0 |
| POST | /session/:sessionId/window/:windowHandle/maximize | ✓ | 14, 10.0 |
| GET, POST | /session/:sessionId/url | ✓ | 14, 10.0 |
| POST | /session/:sessionId/forward | ✓ | 14, 10.0 |
| POST | /session/:sessionId/back | ✓ | 14, 10.0 |
| POST | /session/:sessionId/refresh | ✓ | 14, 10.0 |
| POST | /session/:sessionId/frame | ✓ | 14, 10.0 |
| POST | /session/:sessionId/frame/parent | ✓ | 14, 10.0 |
| POST | /session/:sessionId/moveto | ✓ | 14, 10.0 |
| POST | /session/:sessionId/click | ✓ | 14, 10.0 |
| POST | /session/:sessionId/doubleclick | ✓ | 14, 10.0 |
| POST | /session/:sessionId/buttondown | ✓ | 14, 10.0 |
| POST | /session/:sessionId/buttonup | ✓ | 14, 10.0 |
| POST | /session/:sessionId/keys | ✓ | 14, 10.0 |
| POST | /session/:sessionId/execute | ✓ | 14, 10.0 |
| POST | /session/:sessionId/execute_async | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element | ✓ | 14, 10.0 |
| POST | /session/:sessionId/elements | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/text | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/name | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/selected | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/enabled | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/attribute/:name | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/css/:propertyName | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/displayed | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/location | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/location_in_view | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/size | ✓ | 14, 10.0 |
| GET | /session/:sessionId/element/:id/equals/:other | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/:id/element | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/:id/elements | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/active | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/:id/click | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/:id/submit | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/:id/value | ✓ | 14, 10.0 |
| POST | /session/:sessionId/element/:id/clear | ✓ | 14, 10.0 |
| GET | /session/:sessionId/screenshot | ✓ | 14, 10.0 |
| GET | /session/:sessionId/source | ✓ | 14, 10.0 |
| GET | /session/:sessionId/title | ✓ | 14, 10.0 |
| POST | /session/:sessionId/timeouts | ✓ | 14, 10.0 |
| POST | /session/:sessionId/timeouts/async_script | ✓ | 14, 10.0 |
| POST | /session/:sessionId/timeouts/implicit_wait | ✓ | 14, 10.0 |
| GET, POST | /session/:sessionId/alert_text | ✓ | 14, 10.0 |
| POST | /session/:sessionId/accept_alert | ✓ | 14, 10.0 |
| POST | /session/:sessionId/dismiss_alert | ✓ | 14, 10.0 |
| GET, POST, DELETE | /session/:sessionId/cookie | ✓ | 14, 10.0 |
| DELETE | /session/:sessionId/cookie/:name | ✓ | 14, 10.0 |
| GET, POST | /session/:sessionId/apple/permissions | ✓ | 41, 11.1 |
| POST | /session/:sessionId/apple/attach_debugger | ✓ | 42, 11.1 |
| GET, POST | /session/:sessionId/location |  |  |
| GET, POST | /session/:sessionId/orientation |  |  |
| GET, POST, DELETE | /session/:sessionId/session_storage |  |  |
| GET | /session/:sessionId/session_storage/size |  |  |
| GET, DELETE | /session/:sessionId/session_storage/key/:key |  |  |
| GET, POST, DELETE | /session/:sessionId/local_storage |  |  |
| GET | /session/:sessionId/local_storage/size |  |  |
| GET, DELETE | /session/:sessionId/local_storage/key/:key |  |  |
| GET | /session/:sessionId/application_cache/status |  |  |
| POST | /session/:sessionId/log |  |  |
| GET | /session/:sessionId/log/types |  |  |
| POST | /session/:sessionId/touch/click |  |  |
| POST | /session/:sessionId/touch/down |  |  |
| POST | /session/:sessionId/touch/up |  |  |
| POST | /session/:sessionId/touch/move |  |  |
| POST | /session/:sessionId/touch/scroll |  |  |
| POST | /session/:sessionId/touch/doubleclick |  |  |
| POST | /session/:sessionId/touch/longclick |  |  |
| POST | /session/:sessionId/touch/flick |  |  |
| GET | /session/:sessionId/ime/available_engines |  |  |
| GET | /session/:sessionId/ime/active_engine |  |  |
| GET | /session/:sessionId/ime/activated |  |  |
| POST | /session/:sessionId/ime/deactivate |  |  |
| POST | /session/:sessionId/ime/activate |  |  |
| GET | /session/:sessionId/element/:elementId |  |  |

Note

These endpoints are not supported because they are implemented by intermediary nodes only.

## See Also

### WebDriver

macOS WebDriver Commands for Safari 12 and later

Test your web content using the WebDriver commands supported by Safari 12 and later.

About WebDriver for Safari

Enhance testing of your web content using Safari’s enhancements to WebDriver.

Testing with WebDriver in Safari

Enable WebDriver and run a test.

