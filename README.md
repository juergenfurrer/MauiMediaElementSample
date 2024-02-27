# .NET MAUI MediaElement Sample
Demonstration of crash on iOS when live-stream is AirPlayed to TV

```
{System.OverflowException: TimeSpan overflowed because the duration is too long.
   at System.TimeSpan.IntervalFromDoubleTicks(Double ticks)
   at System.TimeSpan.Interval(Double value, Double scale)
   at System.TimeSpan.FromSeconds(Double value)
   at CommunityToolkit.Maui.Core.Views.MediaManager.ConvertTime(CMTime cmTime)
   at CommunityToolkit.Maui.Core.Views.MediaManager.PlatformUpdatePosition()
   at CommunityToolkit.Maui.Core.Views.MediaManager.UpdateStatus()
   at CommunityToolkit.Maui.Core.Handlers.MediaElementHandler.MapStatusUpdated(MediaElementHandler handler, MediaElement mediaElement, Object args)
   at Microsoft.Maui.CommandMapper`2.<>c__DisplayClass6_0[[CommunityToolkit.Maui.Views.MediaElement, CommunityToolkit.Maui.MediaElement, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null],[CommunityToolkit.Maui.Core.Handlers.MediaElementHandler, CommunityToolkit.Maui.MediaElement, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]].<Add>b__0(IElementHandler h, IElement v, Object o)
   at Microsoft.Maui.CommandMapper.InvokeCore(String key, IElementHandler viewHandler, IElement virtualView, Object args)
   at Microsoft.Maui.CommandMapper.Invoke(IElementHandler viewHandler, IElement virtualView, String property, Object args)
   at Microsoft.Maui.Handlers.ElementHandler.Invoke(String command, Object args)
   at CommunityToolkit.Maui.Views.MediaElement.OnTimerTick(Object sender, EventArgs e)
   at Microsoft.Maui.Dispatching.DispatcherTimer.OnTimerTick()
   at ObjCRuntime.BlockStaticDispatchClass.TrampolineDispatchBlock(IntPtr block) in /Users/builder/azdo/_work/1/s/xamarin-macios/src/ObjCRuntime/Blocks.cs:line 581
   at UIKit.UIApplication.UIApplicationMain(Int32 argc, String[] argv, IntPtr principalClassName, IntPtr delegateClassName) in /Users/builder/azdo/_work/1/s/xamarin-macios/src/UIKit/UIApplication.cs:line 58
   at UIKit.UIApplication.Main(String[] args, Type principalClass, Type delegateClass) in /Users/builder/azdo/_work/1/s/xamarin-macios/src/UIKit/UIApplication.cs:line 94
   at MariaNet.Program.Main(String[] args) in D:\GIT\sdzr\MariaNet\MariaNet\Platforms\iOS\Program.cs:line 13}	System.OverflowException
```
