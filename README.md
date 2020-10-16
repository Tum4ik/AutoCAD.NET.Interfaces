# AutoCAD.NET.Interfaces
The interfaces pack for [AutoCAD.NET](https://www.nuget.org/packages/AutoCAD.NET) API classes to use for dependency injection.
```csharp
if (you want to bring IoC pattern and testability into your AutoCAD plugin)
{
  you are in the correct place;
}
```

## Requirements
- .NET Framework 4.7 and higher
- AutoCAD 2021 and higher

## Installation
[![NuGet: AutoCAD.NET.Interfaces](https://img.shields.io/badge/NuGet-AutoCAD.NET.Interfaces-004880)](https://www.nuget.org/packages/AutoCAD.NET.Interfaces)
[![NuGet: Downloads](https://img.shields.io/nuget/dt/AutoCAD.NET.Interfaces?style=social)](https://www.nuget.org/packages/AutoCAD.NET.Interfaces)

## Important Notes
- Interfaces and their implementations are generated to follow next patterns:
    - **namespace:** Autodesk.AutoCAD.<ins>{ApiNamespace}</ins>.IoC
    - **interface:** I<ins>{ApiType}</ins>
    - **implementation:** <ins>{ApiType}</ins>Impl
    
  So, for example, to get the inteface and implementation for the `Editor`, you should import `IEditor` and `EditorImpl` from the `Autodesk.AutoCAD.EditorInput.IoC`.
- All static members of the classes are converted to dynamic members for testing purposes.
- The original code documentation is kept.

## Currently Available APIs
| AutoCAD.NET                                    | AutoCAD.NET.Interfaces                                                                                          |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|
| Autodesk.AutoCAD.EditorInput.**Editor**        | Autodesk.AutoCAD.EditorInput.IoC.**IEditor** <br> Autodesk.AutoCAD.EditorInput.IoC.**EditorImpl**               | 
| Autodesk.AutoCAD.DatabaseServices.**Database** | Autodesk.AutoCAD.DatabaseServices.IoC.**IDatabase** <br> Autodesk.AutoCAD.DatabaseServices.IoC.**DatabaseImpl** |
| Autodesk.AutoCAD.ApplicationServices.**Document** | Autodesk.AutoCAD.ApplicationServices.IoC.**IDocument** <br> Autodesk.AutoCAD.ApplicationServices.IoC.**DocumentImpl** |
| Autodesk.AutoCAD.GraphicsInterface.**TransientManager** | Autodesk.AutoCAD.GraphicsInterface.IoC.**ITransientManager** <br> Autodesk.AutoCAD.GraphicsInterface.IoC.**TransientManagerImpl** |
