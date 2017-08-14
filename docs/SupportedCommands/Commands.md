## Supported Commands

|          Command           |          Engine Version Support          |
|----------------------------|------------------------------------------|
| `clearNewCommandTimeout`   | 					4.2.5+	 				|
| `clear`          			 | 					4.2.5+	 				|
| `click`                    | 					4.2.1+	 				|
| `down`	                 | 					4.2.7+	 				|
| `findElOrEls`              | 					4.2.1+	 				|
| `getAttribute`             | 					4.2.1+	 				|
| `getContexts`              | 					4.2.1+	 				|
| `getCurrentContext`        | 					4.2.1+	 				|
| `getPageSource`            | 					4.2.1+	 				|
| `getScreenshot`            | 					4.2.1+	 				|
| `getSize`                  | 					4.2.5+	 				|
| `getLocation`              | 					4.2.5+	 				|
| `getText`                  | 					4.2.7+	 				|
| `getSettings`              | 					4.2.5+	 				|
| `getWindowSize`            |          4.4.5+          |
| `implicitWait`             | 					4.2.1+	 				|
| `implicitWaitForCondition` | 					4.2.5+	 				|
| `isSelected`               | 					4.2.5+	 				|
| `isEnabled`                | 					4.2.7+	 				|
| `isDisplayed`              | 					4.2.5+	 				|
| `longclick`                | 					4.2.7+	 				|
| `move`	                 | 					4.2.7+	 				|
| `removeApp`                | 					4.2.1+	 				|
| `setValue`                 | 					4.2.1+	 				|
| `startNewCommandTimeout`   | 					4.2.1+	 				|
| `timeouts`                 | 					4.2.1+	 				|
| `up`		                 | 					4.2.7+	 				|
| `updateSettings`           | 					4.2.5+	 				|

| Proxied Command (iOS, Android)    |
|-----------------------------------|
| `background`                      |
| `closeApp`                        |
| `getLog`                          |
| `getLogTypes`                     |
| `getOrientation`                  |
| `getStrings`                      |
| `isAppInstalled`                  |
| `launchApp`                       |
| `lock`<sup>1</sup>                |
| `setOrientation`                  |

| Proxied Command (iOS only) |
|----------------------------|
| `mobileShake`              |

| Proxied Command (Android only)    |
|-----------------------------------|
| `getNetworkConnection`<sup>2</sup>|
| `isAppInstalled`                  |
| `isLocked`                        |
| `longPressKeyCode`                |
| `pressKeyCode`                    |
| `setNetworkConnection`<sup>2</sup>|
| `toggleLocationServices`          |
| `unlock`                          |


The following attributes can be queried using `attribute`
|          Attribute           |          Engine Version Support          |
|----------------------------|------------------------------------------|
| `className`                | 					4.6.0+	 				|
| `compositeOpacity`         | 					4.2.14+	 				|
| `hasFocus`                 | 					4.6.0+	 				|
| `id`                       | 					4.6.0+	 				|
| `isHittable`               | 					4.6.0+	 				|
| `localOpacity`             | 					4.2.14+	 				|
| `name`                     | 					4.2.1+	 				|

The following commands are used with `getSettings` and `updateSettings`

|      Settings              |          Engine Version Support          |          		Value                	 | 
|----------------------------|------------------------------------------|----------------------------------------|
| `TimeDilation`             | 					4.4.5+		      		| float (>0)	                         |

### Duplicate Touch Commands - Unsupported

| MJWP Command | Notes|
|--------------|------|
| /session/:sessionId/touch/flick|Supported by Touch Action commands|

### JSON Wire Protocol Commands not available to an Appium Client
| JSON Wire Protocol | Notes|
|--------------------|------|
| /wd/hub/status| Not supported by the Appium Java Client|
| /session/:sessionId/element/active | Not supported by the Appium Java Client|
| /session/:sessionId/appium/device/keyevent| Obsoleted by Appium. Use press_keycode.|
| /session/:sessionId/click | Not supported by the Appium Java Client|
| /session/:sessionId/timeouts/implicit_wait | Not supported by the Appium Java Client. Call specific timeout/implicit_wait directly.|