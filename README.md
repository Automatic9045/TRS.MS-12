# TRS.MS-12
![メインメニュー](https://user-images.githubusercontent.com/67314487/111030751-58113800-8447-11eb-9fb2-451313fd5809.png)

【開発中】駅の窓口で見かける座席予約端末をモチーフにした、POS向け汎用端末ソフトウェアです。

ダウンロード：https://github.com/Automatic9045/TRS.MS-12/releases/  
自サイト内の紹介ページ：https://Automatic9045.github.io/contents/software/TRS.MS-12/

## 実行に必要なもの
- .NET Framework 4.8
- [Microsoft Point of Service for .NET（POS for .NET）](https://www.microsoft.com/en-us/download/details.aspx?id=55758)
  - EPSON TM-L90向けプリンタープラグインを使用する場合に限り必要です

## 注意

実行する際は、以下のDLLファイルについてプロパティからブロックの解除を行って下さい。  

- Plugins\Basic\OneTimePrinting\OneTimePrinting.dll
- Plugins\TRS\NumberedTickets\NumberedTicket\NumberedTicket.dll
- Plugins\TRS\NumberedTickets\Canecl\Cancel.dll
- Plugins\TRS\PlatformTickets\PlatformTicket\PlatformTicket.dll
- Plugins\TRS\TRSConnector.dll
- Plugins\TRS\TRSTicket.dll
- Printers\Emulators\ImageSaving.dll
- Printers\Epson\TML90.dll
- Printers\Star\TSP100I.dll
- Printers\Star\TSP100II.dll

解除されていないDLLはソフトウェアから動的に読み込めません。

![ブロックの解除方法](https://user-images.githubusercontent.com/67314487/111025068-5898d700-8425-11eb-9a1b-e9053d2cd63a.png)

## 使用ライブラリ
- [CommonServiceLocator](https://www.nuget.org/packages/CommonServiceLocator) &copy; .NET Foundation and Contributors (Ms-PL)
- [Microsoft.Xaml.Behaviors.Wpf](https://www.nuget.org/packages/Microsoft.Xaml.Behaviors.Wpf) &copy; Microsoft (MIT)
- [Prism.Core](https://www.nuget.org/packages/Prism.Core) &copy; Brian Lagunas, Dan Siegel (MIT)
- [Prism.Unity](https://www.nuget.org/packages/Prism.Unity) &copy; Brian Lagunas, Dan Siegel (MIT)
- [Prism.Wpf](https://www.nuget.org/packages/Prism.Wpf) &copy; Brian Lagunas, Dan Siegel (MIT)
- [System.Runtime.CompilerServices.Unsafe](https://www.nuget.org/packages/System.Runtime.CompilerServices.Unsafe) &copy; Microsoft (MIT)
- [System.Threading.Tasks.Extensions](https://www.nuget.org/packages/System.Threading.Tasks.Extensions) &copy; Microsoft (MIT)
- [System.ValueTuple](https://www.nuget.org/packages/System.ValueTuple) &copy; Microsoft (MIT)
- [Unity.Abstractions](https://www.nuget.org/packages/Unity.Abstractions) &copy; Unity Open Source Project (Apache-2.0)
- [Unity.Container](https://www.nuget.org/packages/Unity.Container) &copy; Unity Open Source Project (Apache-2.0)
- [Gayak.ObservableDictionary](https://github.com/gayaK/Gayak.ObservableDictionary) &copy; 2017 gaya_K (MIT)
