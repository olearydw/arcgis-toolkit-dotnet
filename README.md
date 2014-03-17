# arcgis-toolkit-dotnet

This project contains source code for controls you can use with the ArcGIS Runtime SDK for .NET.  

NOTE: This library requires the ArcGIS Runtime SDK for .NET. See the build instructions below to get started.

## Controls

- Legend - Displays a legend for a set of layers in your map.
- Attribution - Displays copyright/attribution information for layers in your map.
- ScaleLine - Displays current scale reference.
- SignInDialog - (Desktop only) SignIn dialog that challenges the user when accessing ArcGIS secured resources.
- FeatureDataField - Edit control for working with individual feature attributes.
- FeatureDataForm - A simple form layout of all editable fields in a feature using the FeatureDataField for each attribute.

See the [wiki](https://github.com/Esri/arcgis-toolkit-dotnet/wiki) for more details.

## Build 

1. Fork and then clone the repo or download the .zip file.
2. The Toolkit requires the ArcGIS Runtime SDK for .NET.  Confirm that your system meets the requirements for using the ArcGIS Runtime SDK for .NET with [Windows Desktop](http://developers.arcgis.com/net/desktop/guide/system-requirements.htm), [Windows Store](http://developers.arcgis.com/net/store/guide/system-requirements.htm), and/or [Windows Phone](http://developers.arcgis.com/net/phone/guide/system-requirements.htm).  
3. Download and install the [ArcGIS Runtime SDK for .NET](http://esriurl.com/dotnetsdk).  Login to the beta community requires an Esri Global account, which can be created for free.
4. To include Toolkit source in your projects:
 *  In Visual Studio, add the ArcGIS Runtime Toolkit project to your solution. 
    - Windows Desktop (WinDesktop\Esri.ArcGISRuntime.Toolkit\Esri.ArcGISRuntime.Toolkit.proj)
    - Windows Store	(WinStore\Esri.ArcGISRuntime.Toolkit\Esri.ArcGISRuntime.Toolkit.proj)
    - Windows Phone (WinPhone\Esri.ArcGISRuntime.Toolkit\Esri.ArcGISRuntime.Toolkit.proj)
 *  For other projects in the solution, add a reference to the ArcGIS Runtime Toolkit project.
 
#### Optional: Build to distibute the Toolkit
1. Windows Desktop 
 *  Open the solution (WinDesktop-Esri.ArcGISRuntime.Toolkit.sln) in Visual Studio 2012 or 2013 and build the Esri.ArcGISRuntime.Toolkit.dll.
 *  Add a reference to the Esri.ArcGISRuntime.Toolkit.dll in your projects.  
2. Windows Store 
 *  Open the solution (WinStore-Esri.ArcGISRuntime.Toolkit.sln) in Visual Studio 2013 and build the Esri.ArcGISRuntime.Toolkit.dll.   Be sure to build for Release on the ARM, x86, and x64 platforms.
3. Windows Phone: 
 *  Open the solution (WinPhone-Esri.ArcGISRuntime.Toolkit.sln) in Visual Studio 2012 or 2013 and build the Esri.ArcGISRuntime.Toolkit.dll.  Be sure to build for Release on the ARM and x86 platforms.
4. To distribute the Toolkit for use in a Windows Store or Windows Phone project, it should be packaged as Visual Studio extension.  Install the [Visual Studio 2013 SDK](http://msdn.microsoft.com/en-us/library/bb166441.aspx).  This SDK is required to build Visual Studio extension installers (VSIX).  
5. Under the Deployment\VSIX folder in this repo, open the VSIX.sln and build.  If you get errors indicating files cannot be found, be sure to build the Windows Store and Windows Phone Toolkit projects for the release configuration on all platforms.  A set of *.vsix files will be generated in the project output folders. 
6. Run the vsix to install the Toolkit as an extension SDK for Windows Store or Windows Phone projects.  To add a reference in your project, open the Add Reference dialog, navigate to Windows > Extensions, and check the box next to the Toolkit for ArcGIS Runtime. 

## Resources

* [ArcGIS Runtime SDK for .NET](http://esriurl/dotnetsdk)
* [Visual Studio 2013 SDK](http://www.microsoft.com/en-us/download/details.aspx?id=40758)

## Issues

Find a bug or want to request a new feature?  Please let us know by submitting an issue.

## Contributing

Anyone and everyone is welcome to contribute. 

## Licensing
Copyright 2014 Esri

This source is subject to the Microsoft Public License (Ms-PL).
You may obtain a copy of the License at

http://www.microsoft.com/en-us/openness/licenses.aspx#MPL

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt]( https://raw.github.com/Esri/arcgis-toolkit-dotnet/master/license.txt) file.

[](Esri Tags: ArcGIS Runtime SDK .NET WinRT WinStore WPF WinPhone C# C-Sharp DotNet XAML)
[](Esri Language: DotNet)


