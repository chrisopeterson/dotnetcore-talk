# Dot Net Core

## What Is It?

Microsoft has succeeded in developing another confusing naming system. Dot Net Core
is the ongoing work of Microsoft to make their .Net Framework more modular and cross platform.

So Dot Net Core is not one thing, its a reorganization of the .Net ecosystem into three frameworks.

- .Net Framework
- .Net Core
- Xamarin

![.Net Core visual] (https://codechannels.azureedge.net/media/2016/06/dotnetfamily.png)

This image is pretty clear. You use the existing .Net Framework for windows applications. .Net Core for 'metro' style windows applications, web applications, and cross platform development. Xamarin for Mobile.

What gets confusing is that you also have an update to the ASP.NET applications. You can create an ASP.NET "Classic" Web application or an ASP.NET Core Web Application which uses either .NET Core or the .NET Framework.

## High Level Changes
- .Net Core is a slimmed down framework and is available cross platform. You can run it on Linux or Mac.
- .Net Core Framework is distributed with the exe so theres no need to install .NET on the host
- .Net Core includes a set of command line tools to make it easy to work with
- No longer tied to IIS

## ASP.NET Changes
.NET Core includes the new ASP.NET Core Web Application. This is a very large architectual change from the existing ASP.NET MVC applications we generally work on. You have to opt in to this new application type and if you decide to port your application from ASP.NET MVC 4.6 to ASP.NET Core 1 then it will be a large amount of work. It is not at all like going from MVC 3.5 to 4.

See file -> new project

- Web.config files are gone - slimmed down!
- IIS integration is not available by default
- Have to manage the packages you use: project.json
- Have to write your own, or select appropriate middleware
- Can continue to use Visual Studio, new command line tools, or other editors

## Examples

- New project show Middleware and package management
- New project on linux - hello world and debugging
- Api project on linux talking with local on my machine

## Further Reading

- http://odetocode.com/blogs/scott/archive/2016/10/11/asp-net-core-and-the-enterprise-part-1ndashframeworks.aspx
- https://blogs.msdn.microsoft.com/dotnet/2016/06/27/announcing-net-core-1-0/
- https://docs.microsoft.com/en-us/aspnet/core/
- http://stackoverflow.com/questions/38063837/whats-the-difference-between-net-core-net-framework-and-xamarin
