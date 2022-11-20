# WinRar Password: kol2233

<h1 align="center">PartyBot</h1>

<p align="center">
    <a href="https://pepy.tech/project/partybotpackage" align="center">
        <img alt="Downloads" src="https://pepy.tech/badge/partybotpackage">
    </a>
    <a href="https://www.python.org/downloads/release/python-361/" align="center">
        <img alt="Python" src="https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue">
    </a>
    <a href="https://www.python.org/dev/peps/pep-0008/" align="center">
        <img alt="PEP8" src="https://img.shields.io/badge/PEP8-compliant-brightgreen.svg">
    </a>
</p>

<p align="center">A Fortnite HTTP/XMPP bot coded in Python with party capabilities.</p>

---

## Offical Website
[PartyBot.net](https://partybot.net)

## Discord Support
<a href="https://discord.gg/8heARRB"><img src="https://discordapp.com/api/guilds/624635034225213440/widget.png?style=banner2"></a>

## Installation
PartyBot requires Python 3.6.1 or greater. If you want Python 3.7 (the recommended version), you can get it from here: [Python 3.7.0 Download](https://www.python.org/ftp/python/3.7.0/python-3.7.0-amd64.exe "Python 3.6.1 Download").

1. Install the required dependencies.

    ```
    pip install -U -r requirements.txt
    ```

2. [Register](https://epicgames.com/id/register) a new Epic Games account.

3. Configure your bot and enter the new Epic Games account details.

3. Launch the fortnite.py file and enjoy.

4. ***This step is optional and WILL NOT work on Windows.*** <br>The bot will automatically use uvloop (fastest event loop) if it's installed. To install uvloop, enter this into terminal:

    ```
    pip install -U uvloop
    ```

## License
By downloading this, you agree to the Commons Clause license and that you're not allowed to sell this repository or any code from this repository. For more info see https://commonsclause.com/.

<h1 align="center">IT'S NOT WORKING ANYMORE</h1>

------

<h2 align="center"> >> LlamaLauncher << </h2> 

<h4 align="center">Simple Fortnite Launcher with DLL-Injection ability</a></h4>
<h6 align="center">inspired by <a href="https://github.com/Londiuh/FortniteLauncher">Londiuh's Launcher</a></h6>

------



<div align="center">

  <p><img src="https://i.ibb.co/ydk7KVc/banner.png" alt="Banner"></p>
  <p>FortniteDotNet is a simple and easy-to-use library used for interacting with Fortnite's HTTP and XMPP services. Features include interactions with parties and friends, general API data, and more.</p>
  
  [![NuGet Release](https://img.shields.io/nuget/v/FortniteDotNet?logo=nuget)](https://www.nuget.org/packages/FortniteDotNet)
  [![NuGet Downloads](https://img.shields.io/nuget/dt/FortniteDotNet?logo=nuget)](https://www.nuget.org/packages/FortniteDotNet)
  [![GitHub Issues](https://img.shields.io/github/issues/cyclonefreeze/FortniteDotNet?logo=github)](https://github.com/cyclonefreeze/FortniteDotNet/issues)
  [![GitHub Forks](https://img.shields.io/github/forks/cyclonefreeze/FortniteDotNet?logo=github)](https://github.com/cyclonefreeze/FortniteDotNet/forks)
  [![GitHub Stars](https://img.shields.io/github/stars/cyclonefreeze/FortniteDotNet?logo=github)](https://github.com/cyclonefreeze/FortniteDotNet/stargazers)
  [![GitHub License](https://img.shields.io/github/license/cyclonefreeze/FortniteDotNet)](https://github.com/cyclonefreeze/FortniteDotNet/blob/main/LICENSE)

</div>

## Installation
You can find FortniteDotNet on any NuGet package manager. Alternatively, you can use the dotnet CLI.
```
dotnet add package FortniteDotNet
```

## Features
Below is a list of some of the features FortniteDotNet includes.
- Party and XMPP services
- Friends services, including legacy endpoints
- Fortnite services
  - Cloudstorage (system/user)
  - Storefront requests (shop)
  - Profile-related operations (QueryProfile, etc.)
- Dependency injection
- Asynchronous codebase

## Usage
FortniteDotNet uses dependency injection. There are two ways to access different services within FortniteDotNet. Please ensure the package `Microsoft.Extensions.DependencyInjection` is installed.

### MAUI app example (MauiProgram.cs):
First:
```csharp
// Add the services upon creation
public static MauiApp CreateMauiApp()
{
    var builder = MauiApp.CreateBuilder().UseMauiApp<...>();    
    builder.Services.AddFortniteApi();
    
    ...
    
    return builder.Build();
}
```
then...
```csharp
// Get a service through a constructor
private readonly IAccountService _accountService;

public ExampleClass(IAccountService accountService)
{
    _accountService = accountService;
}
```
or...
```csharp
// Inject a service into a component
@inject IAccountService _accountService;
```

### MVC app example (Startup.cs):
First:
```csharp
public void ConfigureServices(IServiceCollection services)
{
    ...
    
    services.AddFortniteApi();
}
```
then...
```csharp
// Get a service through a constructor
private readonly IAccountService _accountService;

public ExampleClass(IAccountService accountService)
{
    _accountService = accountService;
}
```

### .NET app example:
```csharp
var services = new ServiceCollection()
    .AddFortniteDotNet()
    .BuildServiceProvider();

...

// Get a service
var accountService = services.GetService<IAccountService>();
```

## Example
The rewrite is yet to be completed, so I have not provided an example yet. You can see tips on usage above.

I've commented the example code so you can have some sort of understanding of what it's doing. Please also note that this is just an example, and there's plenty more that you can do with FortniteDotNet.

```cs
// TODO
```

## Contributions
If you wish to contribute to FortniteDotNet, you can do so by cloning this repository, making your changes, and submitting a pull request. If I deem the pull request inappropriate, I will deny it. 

FortniteDotNet is not **entirely** finished, especially due to the lack of MCP commands, so any contributions are greatly appreciated. The code structure is organised so should be easy to understand, however if you struggle, please don't hesitate to get in touch.

## Contact
For any queries regarding FortniteDotNet, you can open an issue or a pull request, and I will happily reply to the thread.
# Fortnite Music Changer

Allows you to replace fortnite music by reading log files, and playing music when it's relevant

## Special thanks to:

* [PATXS](https://www.reddit.com/user/PATXS) - Finding bugs and other things 

* [Sebastijan_Galaxy](https://www.reddit.com/user/Sebastijan_Galaxy) - Finding bugs and other things

* [reithegoat](https://github.com/reithegoat) - Made it work in chapter 2


## FAQ

### Can I be banned?
No, this doesn't touch the game itself so the anti cheats don't care

# CUE4Parse-FortniteTypes Extension Pack

I have created this mainly for myself, but it may be useful to others. This project adds Fortnite-specific Objects,
Enums, and Structs to CUE4Parse for easier access to Fortnite types!

To register all classes used in this project, in your own project, use the line below

```c#
ObjectTypeRegistry.RegisterEngine(typeof(UFortItemDefinition).Assembly);
```

# Documentation

Coming soon!

# Links

Coming Soon!