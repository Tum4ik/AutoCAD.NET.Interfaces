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

## Installation
[![NuGet: AutoCAD.NET.Interfaces](https://img.shields.io/badge/NuGet-AutoCAD.NET.Interfaces-004880)](https://www.nuget.org/packages/AutoCAD.NET.Interfaces)

## Important Notes
- All static members of the classes are converted to dynamic members for testing purposes.

## Currently Available APIs
| AutoCAD.NET                                    | AutoCAD.NET.Interfaces                                                                                          |
|------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|
| Autodesk.AutoCAD.EditorInput.**Editor**        | Autodesk.AutoCAD.EditorInput.IoC.**IEditor** <br> Autodesk.AutoCAD.EditorInput.IoC.**EditorImpl**               | 
| Autodesk.AutoCAD.DatabaseServices.**Database** | Autodesk.AutoCAD.DatabaseServices.IoC.**IDatabase** <br> Autodesk.AutoCAD.DatabaseServices.IoC.**DatabaseImpl** |
