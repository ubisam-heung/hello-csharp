# hello-csharp

This document summarizes how to create, run, and build a CSharp console project in VS Code.

## 1) Install VS Code

- Install Visual Studio Code.
- Launch it after installation.

## 2) Install extensions

Install the following extensions.

- C# Dev Kit
- C#
- Material Icon Theme
- Power Mode

## 3) Install and verify .NET SDK

Check the SDK with the command below.

```powershell
dotnet --version
```

## 4) Create a CSharp project

Create the folder and generate a console app.

```powershell
mkdir myProject
cd myProject
dotnet new console -n myProject
```

After creation, the folder structure looks like this.

```text
myProject
├─ myProject.csproj
└─ Program.cs
```

## 5) Run

From the project folder, run:

```powershell
dotnet run
```

## 6) Build

From the project folder, run:

```powershell
dotnet build
```

## 7) Essentials to know in CSharp

- `.sln` is the solution, `.csproj` is the project file.
- Build outputs appear in `bin/Debug/net8.0`, etc.
- `Program.cs` contains the entry point.
- Add NuGet packages via `dotnet add package <package-name>`.
- Use `dotnet build -c Release` for Release builds.

## 8) Useful commands

```powershell
# SDK and environment info
dotnet --info

# List installed packages
dotnet list package
```
