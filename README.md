# KProgressHUD
[![Apache License](https://img.shields.io/badge/license-Apache-blue.svg)](http://opensource.org/licenses/Apache-2.0)

Inspired by [MBProgressHUD](https://github.com/jdg/MBProgressHUD) for iOS.

[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb01.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image01.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb02.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image02.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb03.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image03.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb04.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image04.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb05.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image05.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb06.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image06.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb07.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image07.png?raw=true)
[![](https://raw.githubusercontent.com/Kaopiz/KProgressHUD/master/demo/screenshoots/thumb08.png)](https://github.com/Kaopiz/KProgressHUD/blob/master/demo/screenshoots/image08.png?raw=true)

## Compatibility

Android 2.3 and later

## Adding KProgressHUD to your project

### Gradle

Comming soon

### Source code
You can download and import the *library* folder as module to your project.

## Usage

The usage of KProgressHUD is pretty straight forward. You create the HUD, customize its style and show it on the UI thread. Then fire a background thread to work on long-running tasks. When done, call `dismiss()` to close it (if you use a determinate style, the HUD will automatically dismiss if progress reach its max).

```java
KProgressHUD.create(MainActivity.this)
	.setStyle(KProgressHUD.Style.SPIN_INDETERMINATE)
	.setLabel("Please wait")
	.setDetailsLabel("Downloading data");
	.setCancellable(true)
	.setAnimationSpeed(2)
	.setDimAmount(0.5f)
	.show();
```

See [**Javadocs**](http://kaopiz.github.io/KProgressHUD/) or [**sample app**](https://github.com/Kaopiz/KProgressHUD/tree/master/demo/src/main) for more information.

## Contributing
1. Fork it ( https://github.com/Kaopiz/KProgressHUD/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Contributor
* [tuanna-hsp](https://github.com/tuanna-hsp)
* [nafuto](https://github.com/nafuto)

## License
```
   Copyright 2015 Kaopiz Software Co., Ltd.

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```