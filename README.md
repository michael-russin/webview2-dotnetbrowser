## webview2-dotnetbrowser
When Microsoft revealed their plans for a Chrome based Edge browser the first thing I thought was "I wonder if they are going to support an embedded web browser control"?  Well sure enough they released [WebView2](https://github.com/MicrosoftEdge/WebView2Browser) and I've been keeping an eye on the releases.  Recently I found a great [sample](https://github.com/MicrosoftEdge/WebView2Browser) written by [David Risney](https://github.com/david-risney) and I was inspired to take a shot at putting together a C# version.

This "port" is a dot net web browser built with
* [Microsoft Edge WebView2](https://docs.microsoft.com/en-us/microsoft-edge/hosting/webview2) control
* [WebView2 Interop](https://github.com/michael-russin/webview2-interop)
* [WebView2 Windows Forms Control](https://github.com/michael-russin/webview2-control)

It is a sample Windows desktop application demonstrating the WebView2 control capabilities. It is built as a Windows Forms [Visual Studio 2019](https://visualstudio.microsoft.com/vs/) project and makes use of the WebView2 C++ toolkit, a C# interop and a custom windows forms control.  JavaScript is used in the WebView2 environment to power its features.

## Prerequisites
- [Microsoft Edge (Chromium)](https://www.microsoftedgeinsider.com/en-us/download/) installed on a supported OS.
- [Visual Studio](https://visualstudio.microsoft.com/vs/) with C# desktop development support installed.
Edge Version Canary or Dev channel is recommended for the installation and the minimum version is 80.0.320.5

## Build the browser
Clone the repository and open the solution in Visual Studio. Microsoft.Web.WebView2, MtrDev.WebView2.Interop and MtrDev.WebView2.WinForms are already included as a NuGet packages* in the project!

- Clone this repository
- Open the solution in Visual Studio 2019 (2017 should also work)
- Make the changes listed below if you're using a Windows version below Windows 10.
- Set the target you want to build 
- Build the solution

## Functionality
For now check out the [C++ sample readme](https://github.com/MicrosoftEdge/WebView2Browser/blob/master/README.md) while I find some time to modify it for this project.

## Links
- Project homepage: https://github.com/michael-russin/webview2-dotnetbrowse
- Repository: https://github.com/michael-russin/webview2-dotnetbrowse
- Issue tracker: https://github.com/michael-russin/webview2-dotnetbrowse/issues
- Related projects:
  - WebView2 Interop : https://github.com/michael-russin/webview2-interop
  - WebView2 Windows Forms Control: https://github.com/michael-russin/webview2-control
  - David's awsome C++ sample: https://github.com/MicrosoftEdge/WebView2Browser
  - WebView2 Documentation: https://docs.microsoft.com/en-us/microsoft-edge/hosting/webview2/reference-webview2
  
## Licensing
The code in this project is licensed under MIT license.
