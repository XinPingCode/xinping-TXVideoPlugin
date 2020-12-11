# xinping-TXVideoPlugin
本插件是基于TXLiteAVSDK的腾讯多方视频插件，目前版本实现双人视频通话功能，目前仅支持Module方式的同步调用，sdkAppId、userId、roomId为必传参数
同步调用代码如下：
```javascript
testSyncFunc() {

                // 调用同步方法
                var ret = testModule.testSyncFunc({
                    sdkAppId: 8888888888,
                    userId:  "test123",
                    roomId: 123456
                })

               }
```
