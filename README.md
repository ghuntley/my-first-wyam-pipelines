```csharp
            Exception while processing document [unknown source] in module Razor: The model item passed into the ViewDataDictionary is of type 'Wyam.Core.Documents.Document', but this ViewDataDictionary instance requires a model item of type 'Google.Apis.YouTube.v3.Data.PlaylistItemListResponse'.
            Error while executing module Razor
        Error while executing pipeline RenderYouTube
Exception during execution: System.AggregateException: One or more errors occurred. ---> System.InvalidOperationException: The model item passed into the ViewDataDictionary is of type 'Wyam.Core.Documents.Document', but this ViewDataDictionary instance requires a model item of type 'Google.Apis.YouTube.v3.Data.PlaylistItemListResponse'.
   at Microsoft.AspNetCore.Mvc.ViewFeatures.ViewDataDictionary.EnsureCompatible(Object value)
   at Microsoft.AspNetCore.Mvc.ViewFeatures.ViewDataDictionary..ctor(ViewDataDictionary source, Object model, Type declaredModelType)
   at lambda_method(Closure , ViewDataDictionary )
   at Microsoft.AspNetCore.Mvc.Razor.RazorPageActivator.Activate(IRazorPage page, ViewContext context)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.RenderPageCoreAsync(IRazorPage page, ViewContext context)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.<RenderPageAsync>d__14.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.<RenderLayoutAsync>d__17.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.<RenderAsync>d__13.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Wyam.Razor.RazorCompiler.RenderPage(RenderRequest request) in C:\Dropbox\OSS\wyamio\youtube\src\extensions\Wyam.Razor\RazorCompiler.cs:line 80
   at Wyam.Razor.RazorService.Render(RenderRequest request) in C:\Dropbox\OSS\wyamio\youtube\src\extensions\Wyam.Razor\RazorService.cs:line 27
   at Wyam.Razor.Razor.<>c__DisplayClass16_0.<Execute>b__1(IDocument input) in C:\Dropbox\OSS\wyamio\youtube\src\extensions\Wyam.Razor\Razor.cs:line 246
   at Wyam.Common.Execution.TraceExceptionsExtensions.TraceExceptions[TResult](IExecutionContext context, IDocument document, Func`2 func) in C:\Dropbox\OSS\wyamio\youtube\src\core\Wyam.Common\Execution\TraceExceptionsExtensions.cs:line 55
   at System.Linq.Parallel.PartitionedDataSource`1.ListContiguousIndexRangeEnumerator.MoveNext(T& currentElement, Int32& currentKey)
   at System.Linq.Parallel.PipelineSpoolingTask`2.SpoolingWork()
   at System.Linq.Parallel.SpoolingTaskBase.Work()
   at System.Linq.Parallel.QueryTask.BaseWork(Object unused)
   at System.Threading.Tasks.Task.Execute()
   --- End of inner exception stack trace ---
   at System.Linq.Parallel.QueryTaskGroupState.QueryEnd(Boolean userInitiatedDispose)
   at System.Linq.Parallel.AsynchronousChannelMergeEnumerator`1.MoveNextSlowPath()
   at System.Linq.Parallel.QueryOpeningEnumerator`1.MoveNext()
   at System.Linq.Enumerable.WhereEnumerableIterator`1.MoveNext()
   at System.Linq.Buffer`1..ctor(IEnumerable`1 source)
   at System.Linq.Enumerable.ToArray[TSource](IEnumerable`1 source)
   at System.Collections.Immutable.ImmutableArray.CreateRange[T](IEnumerable`1 items)
   at Wyam.Core.Execution.ExecutionPipeline.Execute(ExecutionContext context, IEnumerable`1 modules, ImmutableArray`1 inputDocuments) in C:\Dropbox\OSS\wyamio\youtube\src\core\Wyam.Core\Execution\ExecutionPipeline.cs:line 191
   at Wyam.Core.Execution.ExecutionPipeline.Execute(Engine engine, Guid executionId) in C:\Dropbox\OSS\wyamio\youtube\src\core\Wyam.Core\Execution\ExecutionPipeline.cs:line 85
   at Wyam.Core.Execution.Engine.Execute() in C:\Dropbox\OSS\wyamio\youtube\src\core\Wyam.Core\Execution\Engine.cs:line 286
---> (Inner Exception #0) System.InvalidOperationException: The model item passed into the ViewDataDictionary is of type 'Wyam.Core.Documents.Document', but this ViewDataDictionary instance requires a model item of type 'Google.Apis.YouTube.v3.Data.PlaylistItemListResponse'.
   at Microsoft.AspNetCore.Mvc.ViewFeatures.ViewDataDictionary.EnsureCompatible(Object value)
   at Microsoft.AspNetCore.Mvc.ViewFeatures.ViewDataDictionary..ctor(ViewDataDictionary source, Object model, Type declaredModelType)
   at lambda_method(Closure , ViewDataDictionary )
   at Microsoft.AspNetCore.Mvc.Razor.RazorPageActivator.Activate(IRazorPage page, ViewContext context)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.RenderPageCoreAsync(IRazorPage page, ViewContext context)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.<RenderPageAsync>d__14.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.<RenderLayoutAsync>d__17.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Microsoft.AspNetCore.Mvc.Razor.RazorView.<RenderAsync>d__13.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.ExceptionServices.ExceptionDispatchInfo.Throw()
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Wyam.Razor.RazorCompiler.RenderPage(RenderRequest request) in C:\Dropbox\OSS\wyamio\youtube\src\extensions\Wyam.Razor\RazorCompiler.cs:line 80
   at Wyam.Razor.RazorService.Render(RenderRequest request) in C:\Dropbox\OSS\wyamio\youtube\src\extensions\Wyam.Razor\RazorService.cs:line 27
   at Wyam.Razor.Razor.<>c__DisplayClass16_0.<Execute>b__1(IDocument input) in C:\Dropbox\OSS\wyamio\youtube\src\extensions\Wyam.Razor\Razor.cs:line 246
   at Wyam.Common.Execution.TraceExceptionsExtensions.TraceExceptions[TResult](IExecutionContext context, IDocument document, Func`2 func) in C:\Dropbox\OSS\wyamio\youtube\src\core\Wyam.Common\Execution\TraceExceptionsExtensions.cs:line 55
   at System.Linq.Parallel.PartitionedDataSource`1.ListContiguousIndexRangeEnumerator.MoveNext(T& currentElement, Int32& currentKey)
   at System.Linq.Parallel.PipelineSpoolingTask`2.SpoolingWork()
   at System.Linq.Parallel.SpoolingTaskBase.Work()
   at System.Linq.Parallel.QueryTask.BaseWork(Object unused)
   at System.Threading.Tasks.Task.Execute()<---
```