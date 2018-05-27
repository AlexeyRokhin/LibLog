# LibLog [![Build status](https://ci.appveyor.com/api/projects/status/4v136j3od783udpa?svg=true)](https://ci.appveyor.com/project/damianh/liblog) [![NuGet Badge](https://buildstats.info/nuget/LibLog)](https://www.nuget.org/packages/LibLog/) [![Join the chat at https://gitter.im/damianh/LibLog](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/damianh/LibLog?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Designed specifically for library developers, `LibLog` is a single file for you to either copy/paste or [install via nuget][0], into your library/framework/application to provide a logging abstraction. It also contains transparent built-in support for [NLog][3], [Log4Net][4], [Serilog][9] and [Loupe][10], and allows your users to define a custom provider if necessary.

Please see [Wiki](https://github.com/damianh/LibLog/wiki) for more information.

## Availability for old csproj format

LibLog uses `.pp` file to do a namespace transform (aka [source
transform](https://docs.microsoft.com/en-us/nuget/create-packages/source-and-config-file-transformations))
so it fits into your project's namespace. This is handled transparently by the
new dotnet sdk as of LibLog version 5.0.0. For older project formats, please
continue to use LibLog 4.x versions.

## Compiler Options

 - Define `LIBLOG_PUBLIC` to have the LibLog API as part of your libraries
   _public_ API. Generally you may do this 
 - Define `LIBLOG_EXCLUDE_CODE_COVERAGE` to exclude LibLog from your code
   coverage reports

### License

LibLog is licensed under [MIT Licence][2].

##### Developed with:

[![Resharper](http://neventstore.org/images/logo_resharper_small.gif)](http://www.jetbrains.com/resharper/)
[![dotCover](http://neventstore.org/images/logo_dotcover_small.gif)](http://www.jetbrains.com/dotcover/)
[![dotTrace](http://neventstore.org/images/logo_dottrace_small.gif)](http://www.jetbrains.com/dottrace/)

Feedback, compliments or criticism: [@randompunter][6] 

[0]: https://www.nuget.org/packages/LibLog
[1]: https://github.com/damianh/LibLog/blob/master/src/LibLog/LibLog.cs
[2]: http://www.opensource.org/licenses/MIT
[3]: http://nlog-project.org/
[4]: https://logging.apache.org/log4net/
[6]: https://twitter.com/randompunter
[9]: http://serilog.net/
[10]: http://www.gibraltarsoftware.com/Loupe
