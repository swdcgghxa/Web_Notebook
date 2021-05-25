* Xamarin Navigation(導航)
    https://docs.microsoft.com/en-us/xamarin/xamarin-forms/app-fundamentals/navigation/
* Xamarin.Forms(基本概念)
    https://docs.microsoft.com/zh-tw/xamarin/xamarin-forms/app-fundamentals/
* XAML(應用程序標記語言)
    https://docs.microsoft.com/en-us/xamarin/xamarin-forms/xaml/
* DependencyService(依賴服務)
    https://docs.microsoft.com/en-us/xamarin/xamarin-forms/app-fundamentals/dependency-service/
* Xamarin.Essentials(跨平台感測器)
    https://docs.microsoft.com/zh-tw/xamarin/essentials/


* Xamarin.Android - Services(前|背景服務)
    https://docs.microsoft.com/en-us/xamarin/android/app-fundamentals/services/
    **AndroidManifest.xml**
    添加:
    `Android.App.Application.Context.StartService(sendIntent);`
```
[Service]
public class DemoService : Service
{
          
}
```