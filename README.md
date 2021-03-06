# HolisticWare.DotNetNew.XamarinProjectsStructureTemplate

This `dotnet` template 

*   is premised on the experience that it is easier to remove/delete code (projects in this case), 
    than to add them.

*   is prepared for cross-platform usage, bait-n-switch concept commonly used in libraries like 
    Xamarin.Forms, Xamarin.Essentials, Xamarin.Auth and follows these rules:

    *   All assemblies have the same:

        *   Assembly Name
        
        *   Namespace

*   dotnet template

    https://github.com/holisticware-xamarin/HolisticWare.DotNetNew.XamarinProjectsStructureTemplate

*   github template repo

    https://github.com/holisticware-xamarin/HolisticWare.XamarinProjectsStructureTemplate

*   nuget

    https://www.nuget.org/packages/HolisticWare.DotNetNew.XamarinProjectsStructureTemplate.CSharp

## Usage

```
    dotnet new hw-structure -n SomeProject -o SomeOutputFolder

# Upon succesful creation:

    The template "Custom template for Xamarin cross platform libraries and bindings" was created successfully.
```

See below folder structure generated: [Folder Structure](#folder-structure)

## Installation

    dotnet new \
        --install “HolisticWare.DotNetNew.XamarinProjectsStructureTemplate.CSharp”


## NuGet

HolisticWare.DotNetNew.XamarinProjectsStructureTemplate

```
    # nuget restore invalid version errors
    dotnet new .
    # OK
    dotnet new ./
    
```

```
    nuget push \
        -Source https://www.nuget.org/api/v2/package \
        HolisticWare.DotNetNew.XamarinProjectsStructureTemplate.CSharp.2017.12.2.2.nupkg
```



## Folder structure:


```
    tree Demo

    # Output:
    
    Demo
    ├── External-Dependency-Info.txt
    ├── LICENSE.md
    ├── build.cake
    ├── nuget
    │   └── HolisticWare.Demo.nuspec
    ├── samples
    │   ├── Demo.Sample.XamarinAndroid
    │   │   ├── Assets
    │   │   │   └── AboutAssets.txt
    │   │   ├── Demo.Sample.XamarinAndroid.csproj
    │   │   ├── MainActivity.cs
    │   │   ├── Properties
    │   │   │   ├── AndroidManifest.xml
    │   │   │   └── AssemblyInfo.cs
    │   │   ├── Resources
    │   │   │   ├── AboutResources.txt
    │   │   │   ├── Resource.designer.cs
    │   │   │   ├── layout
    │   │   │   │   └── Main.axml
    │   │   │   ├── mipmap-hdpi
    │   │   │   │   └── Icon.png
    │   │   │   ├── mipmap-mdpi
    │   │   │   │   └── Icon.png
    │   │   │   ├── mipmap-xhdpi
    │   │   │   │   └── Icon.png
    │   │   │   ├── mipmap-xxhdpi
    │   │   │   │   └── Icon.png
    │   │   │   ├── mipmap-xxxhdpi
    │   │   │   │   └── Icon.png
    │   │   │   └── values
    │   │   │       └── Strings.xml
    │   │   ├── bin
    │   │   ├── obj
    │   │   │   └── Debug
    │   │   │       ├── R.cs.flag
    │   │   │       ├── __library_projects__
    │   │   │       │   └── System.Runtime.stamp
    │   │   │       ├── android
    │   │   │       │   └── net
    │   │   │       │       └── holisticware
    │   │   │       │           └── xamarinprojectsstructuretemplate_sample_xamarinandroid
    │   │   │       │               └── R.java
    │   │   │       ├── build.props
    │   │   │       ├── libraryimports.cache
    │   │   │       ├── libraryprojectimports.cache
    │   │   │       └── res
    │   │   │           ├── layout
    │   │   │           │   └── main.xml
    │   │   │           ├── mipmap-hdpi
    │   │   │           │   └── icon.png
    │   │   │           ├── mipmap-mdpi
    │   │   │           │   └── icon.png
    │   │   │           ├── mipmap-xhdpi
    │   │   │           │   └── icon.png
    │   │   │           ├── mipmap-xxhdpi
    │   │   │           │   └── icon.png
    │   │   │           ├── mipmap-xxxhdpi
    │   │   │           │   └── icon.png
    │   │   │           └── values
    │   │   │               └── strings.xml
    │   │   └── packages.config
    │   ├── Demo.Sample.XamarinAndroid.UITests
    │   │   ├── Demo.Sample.XamarinAndroid.UITests.csproj
    │   │   ├── Tests.cs
    │   │   ├── bin
    │   │   ├── obj
    │   │   └── packages.config
    │   ├── Demo.Sample.XamarinIOS
    │   │   ├── AppDelegate.cs
    │   │   ├── Assets.xcassets
    │   │   │   ├── AppIcon.appiconset
    │   │   │   │   └── Contents.json
    │   │   │   ├── Contents.json
    │   │   │   ├── First.imageset
    │   │   │   │   ├── Contents.json
    │   │   │   │   └── vector.pdf
    │   │   │   └── Second.imageset
    │   │   │       ├── Contents.json
    │   │   │       └── vector.pdf
    │   │   ├── Demo.Sample.XamarinIOS.csproj
    │   │   ├── Entitlements.plist
    │   │   ├── FirstViewController.cs
    │   │   ├── FirstViewController.designer.cs
    │   │   ├── Info.plist
    │   │   ├── LaunchScreen.storyboard
    │   │   ├── Main.cs
    │   │   ├── Main.storyboard
    │   │   ├── SecondViewController.cs
    │   │   ├── SecondViewController.designer.cs
    │   │   ├── bin
    │   │   ├── obj
    │   │   └── packages.config
    │   ├── Demo.Sample.XamarinIOS.UITests
    │   │   ├── Demo.Sample.XamarinIOS.UITests.csproj
    │   │   ├── Tests.cs
    │   │   ├── bin
    │   │   ├── obj
    │   │   └── packages.config
    │   └── Demo.Samples.sln
    └── source
        ├── Demo.Bindings.XamarinAndroid
        │   ├── Additions
        │   │   └── AboutAdditions.txt
        │   ├── Demo.Bindings.XamarinAndroid.csproj
        │   ├── Jars
        │   │   └── AboutJars.txt
        │   ├── Properties
        │   │   └── AssemblyInfo.cs
        │   ├── Transforms
        │   │   ├── EnumFields.xml
        │   │   ├── EnumMethods.xml
        │   │   └── Metadata.xml
        │   ├── bin
        │   └── obj
        ├── Demo.Bindings.XamarinIOS
        │   ├── ApiDefinition.cs
        │   ├── Demo.Bindings.XamarinIOS.csproj
        │   ├── Properties
        │   │   └── AssemblyInfo.cs
        │   └── Structs.cs
        ├── Demo.NetStandard10
        │   ├── Demo.NetStandard10.csproj
        │   ├── bin
        │   └── obj
        │       ├── Demo.NetStandard10.csproj.nuget.cache
        │       ├── Demo.NetStandard10.csproj.nuget.g.props
        │       ├── Demo.NetStandard10.csproj.nuget.g.targets
        │       └── project.assets.json
        ├── Demo.Source.sln
        └── Demo.Source.userprefs
```


## `dotnet new` templating links/references

*   https://github.com/dotnet/templating/wiki/Available-templates-for-dotnet-new

*   http://dotnetnew.azurewebsites.net/

*   https://docs.microsoft.com/en-us/dotnet/core/tools/custom-templates

*   https://pioneercode.com/post/how-to-create-a-dot-net-new-project-template-in-dot-net-core

*   https://rehansaeed.com/custom-project-templates-using-dotnet-new/

*   https://github.com/aspnet/templating/blob/dev/src/Microsoft.AspNetCore.SpaTemplates/content/Aurelia-CSharp/.template.config/template.json
