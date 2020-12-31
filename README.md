# DLL-Injection
A DLL Injection method by using process_create_thread

# How to use
1. Download injection.cs from the [Latest release](https://github.com/SantinoCaruso/DLL-Injection/releases/latest).
2. Add the file to the project solution and at the top of the code (in the file you gonna use the injection function) add
```cs
using PROCCES_CREATE_THREAD;
```
3. Execute the function by doing:
```cs
Injection.InjectDLL("process name here (with no .exe)", "dll path here");
```

### Usage example:
If the user is introducing data:
```cs
void inject(string proc, string dllPath) {
  Injection.InjectDLL(proc, dllPath);
}
```

If the variables can't be defined by the user:
```cs
void inject() {
  Injection.InjectDLL("program", "file.dll");
}
```
