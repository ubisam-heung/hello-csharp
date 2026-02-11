# hello-csharp

VS Code에서 CSharp 콘솔 프로젝트를 생성하고 실행/빌드하는 과정을 정리했습니다.

## 1) VS Code 설치

- Visual Studio Code를 설치합니다.
- 설치 후 실행합니다.

## 2) 확장팩 설치

다음 확장팩을 설치합니다.

- C# Dev Kit
- C#
- Material Icon Theme
- Power Mode

## 3) .NET SDK 설치 및 확인

아래 명령으로 설치 여부를 확인합니다.

```powershell
dotnet --version
```

## 4) CSharp 프로젝트 생성

프로젝트 폴더를 만들고 콘솔 앱을 생성합니다.

```powershell
mkdir myProject
cd myProject
dotnet new console -n myProject
```

생성 후 폴더 구조는 다음과 같습니다.

```text
myProject
├─ myProject.csproj
└─ Program.cs
```

## 5) 실행

프로젝트 폴더에서 아래 명령을 실행합니다.

```powershell
dotnet run
```

## 6) 빌드

프로젝트 폴더에서 아래 명령을 실행합니다.

```powershell
dotnet build
```

## 7) CSharp에서 알아두면 좋은 정보

- `.sln`은 솔루션, `.csproj`는 프로젝트 설정 파일입니다.
- 빌드 결과는 `bin/Debug/net8.0` 등에 생성됩니다.
- `Program.cs`에 진입점(메인 코드)이 있습니다.
- NuGet 패키지는 `dotnet add package <패키지명>`으로 추가합니다.
- Release 빌드는 `dotnet build -c Release`로 생성합니다.

## 8) 참고 명령

```powershell
# SDK 및 환경 정보
dotnet --info

# 패키지 목록 확인
dotnet list package
```
