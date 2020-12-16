# xinping-TXVideoPlugin
**1.插件描述** 本插件是基于TXLiteAVSDK的腾讯多方视频插件，目前版本实现双人视频通话功能。  
  
**2.使用方法** 插件提供了一个方法：
  
TXVideoSyncFunc:通过Module方式的同步调用弹出双人视频通话页面
  
**3.参数说明**
  
| 参数名 | 类型 | 说明 |
| :----:| :----: | :----: |
| sdkAppId | Number | 应用标识 [必填]，腾讯云基于 sdkAppId 完成计费统计 |
| userId | String | 用户标识 [必填]，当前用户的 userId，相当于登录用户名 |
| roomId | Number | 字符串房间号码[必填]，在同一个房间里的用户（userId）可以彼此看到对方并进行视频通话 |

  
**4.代码示例**


同步调用代码如下：  

```javascript
var TXVideoPluginModule = uni.requireNativePlugin("xinping-TXVideoPlugin-TXVideoPluginModule")
TXVideoSyncFunc() {
				let params = {
					sdkAppId:this.sdkAppId,
					userId:this.userId,
					roomId:this.roomId
				};
				// 调用同步方法
			 TXVideoPluginModule.TXVideoSyncFunc(params);

		   }               

```
