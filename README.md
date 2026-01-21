# MVC5movie
 &emsp; *cloned from https://github.com/kexuelou/MvcMovie5*  

## `net45`, Runtime Version v4.0.30319 [ASP.NET MVC 4](https://learn.microsoft.com/en-us/aspnet/mvc/mvc4)
Sample application for [Getting Started with ASP.NET MVC 5](https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/introduction/getting-started)
- Creating *new* ASP.NET MVC projects in Visual Studio is problematic.
	- it wants to use `<TargetFrameworkVersion>` newer than `v4.8`
- Hacks
	- let Visual Studio update from v4.5 to v4.8
		- it automagically added `Use64BitIISExpress`
	- [bootstrap bundle change](https://learn.microsoft.com/en-us/answers/questions/502208/@scripts-render(-bundles-bootstrap)-fails)
	- disabled SQL, `MovieDBContext`, `public ActionResult Index()`;  `Movie movie = null;`
	- updated jquery, bootstrap, other NuGet packages with exploit warnings
- with Visual Studio stopped, removed `.vs MvcMovie/bin MvcMovie/obj`
	- then restarting VS and rebuilding MvcMovie5 eliminated NuGet version warnings

- removed `EntityFramework`;&nbsp; evidently only for SQL

### Replacing IISExpress
- [IIS alternatives?](https://www.reddit.com/r/dotnet/comments/1c921xk/iis_alternatives/)
	- [YARP with Kestrel]()
