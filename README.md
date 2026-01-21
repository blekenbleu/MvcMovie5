# MVC5movie
 &emsp; *cloned from https://github.com/kexuelou/MvcMovie5*  

Sample application for [Getting Started with ASP.NET MVC 5](https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/introduction/getting-started)
- Creating *new* ASP.NET MVC projects in Visual Studio is problematic.
	- it wants to use `<TargetFrameworkVersion>` newer than `v4.8`
- Hacks
	- let Visual Studio update from v4.5 to v4.8
		- it automagically added `Use64BitIISExpress`
	- [bootstrap bundle change](https://learn.microsoft.com/en-us/answers/questions/502208/@scripts-render(-bundles-bootstrap)-fails)
	- disabled SQL, `MovieDBContext`, `public ActionResult Index()`;  `Movie movie = null;`
	- updated jquery, bootstrap
