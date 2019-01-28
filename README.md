# quickxorhash-cs
Command line project to generate the OneDrive Quick XOR Hash value for a file using Microsoft's sample implementation.

## Build
https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/compiler-options/command-line-building-with-csc-exe
```powershell
csc.exe .\quickxorhash.cs
```

## Run
```powershell
.\quickxorhash.exe .\quickxorhash.cs
20mzVy/qZgDosgNEkl58h+DHTD8=
```

## Benchmark
Via powershell
```powershell
Measure-Command {.\quickxorhash.exe .\quickxorhash.cs}
Measure-Command {Get-FileHash .\quickxorhash.cs -Algorithm MD5}
Measure-Command {Get-FileHash .\quickxorhash.cs -Algorithm SHA1}
```
