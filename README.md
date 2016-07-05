2559-07-05 01:24:30> Program: Starting Squirrel Updater: --install .
2559-07-05 01:24:30> Program: Starting install, writing to C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 01:24:30> Program: About to install to: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom
2559-07-05 01:24:30> CheckForUpdateImpl: Failed to load local releases, starting from scratch: System.IO.DirectoryNotFoundException: Could not find a part of the path 'C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\packages\RELEASES'.
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileStream.Init(String path, FileMode mode, FileAccess access, Int32 rights, Boolean useRights, FileShare share, Int32 bufferSize, FileOptions options, SECURITY_ATTRIBUTES secAttrs, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.FileStream..ctor(String path, FileMode mode, FileAccess access, FileShare share)
   at Squirrel.Utility.LoadLocalReleases(String localReleaseFile)
   at Squirrel.UpdateManager.CheckForUpdateImpl.<CheckForUpdate>d__3f.MoveNext()
2559-07-05 01:24:30> CheckForUpdateImpl: Reading RELEASES file from C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 01:24:30> CheckForUpdateImpl: First run or local directory is corrupt, starting from scratch
2559-07-05 01:24:30> ApplyReleasesImpl: Writing files to app directory: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\app-1.8.0
2559-07-05 01:25:03> IEnableLogger: Failed to install package to app dir: System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at System.IO.Path.GetFullPath(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
2559-07-05 01:25:03> Unhandled exception: System.AggregateException: One or more errors occurred. ---> System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at System.IO.Path.GetFullPath(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()
   --- End of inner exception stack trace ---
   at System.Threading.Tasks.Task.ThrowIfExceptional(Boolean includeTaskCanceledExceptions)
   at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
   at System.Threading.Tasks.Task.Wait()
   at Squirrel.Update.Program.executeCommandLine(String[] args)
   at Squirrel.Update.Program.main(String[] args)
---> (Inner Exception #0) System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at System.IO.Path.GetFullPath(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()<---

2559-07-05 01:26:46> Program: Starting Squirrel Updater: --install .
2559-07-05 01:26:46> Program: Starting install, writing to C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 01:26:46> Program: About to install to: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom
2559-07-05 01:26:46> Program: Install path C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom already exists, burning it to the ground
2559-07-05 01:26:54> CheckForUpdateImpl: Failed to load local releases, starting from scratch: System.IO.DirectoryNotFoundException: Could not find a part of the path 'C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\packages\RELEASES'.
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileStream.Init(String path, FileMode mode, FileAccess access, Int32 rights, Boolean useRights, FileShare share, Int32 bufferSize, FileOptions options, SECURITY_ATTRIBUTES secAttrs, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.FileStream..ctor(String path, FileMode mode, FileAccess access, FileShare share)
   at Squirrel.Utility.LoadLocalReleases(String localReleaseFile)
   at Squirrel.UpdateManager.CheckForUpdateImpl.<CheckForUpdate>d__3f.MoveNext()
2559-07-05 01:26:54> CheckForUpdateImpl: Reading RELEASES file from C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 01:26:54> CheckForUpdateImpl: First run or local directory is corrupt, starting from scratch
2559-07-05 01:26:55> ApplyReleasesImpl: Writing files to app directory: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\app-1.8.0
2559-07-05 01:27:20> IEnableLogger: Failed to install package to app dir: System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at System.IO.Path.GetFullPath(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
2559-07-05 01:27:20> Unhandled exception: System.AggregateException: One or more errors occurred. ---> System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at System.IO.Path.GetFullPath(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()
   --- End of inner exception stack trace ---
   at System.Threading.Tasks.Task.ThrowIfExceptional(Boolean includeTaskCanceledExceptions)
   at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
   at System.Threading.Tasks.Task.Wait()
   at Squirrel.Update.Program.executeCommandLine(String[] args)
   at Squirrel.Update.Program.main(String[] args)
---> (Inner Exception #0) System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at System.IO.Path.GetFullPath(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()<---

2559-07-05 18:00:08> Program: Starting Squirrel Updater: --install .
2559-07-05 18:00:09> Program: Starting install, writing to C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 18:00:10> Program: About to install to: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom
2559-07-05 18:00:10> Program: Install path C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom already exists, burning it to the ground
2559-07-05 18:00:24> CheckForUpdateImpl: Failed to load local releases, starting from scratch: System.IO.DirectoryNotFoundException: Could not find a part of the path 'C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\packages\RELEASES'.
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileStream.Init(String path, FileMode mode, FileAccess access, Int32 rights, Boolean useRights, FileShare share, Int32 bufferSize, FileOptions options, SECURITY_ATTRIBUTES secAttrs, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.FileStream..ctor(String path, FileMode mode, FileAccess access, FileShare share)
   at Squirrel.Utility.LoadLocalReleases(String localReleaseFile)
   at Squirrel.UpdateManager.CheckForUpdateImpl.<CheckForUpdate>d__3f.MoveNext()
2559-07-05 18:00:24> CheckForUpdateImpl: Reading RELEASES file from C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 18:00:24> CheckForUpdateImpl: First run or local directory is corrupt, starting from scratch
2559-07-05 18:00:26> ApplyReleasesImpl: Writing files to app directory: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\app-1.8.0
2559-07-05 18:01:12> IEnableLogger: Failed to install package to app dir: System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
2559-07-05 18:01:14> Unhandled exception: System.AggregateException: One or more errors occurred. ---> System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()
   --- End of inner exception stack trace ---
   at System.Threading.Tasks.Task.ThrowIfExceptional(Boolean includeTaskCanceledExceptions)
   at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
   at System.Threading.Tasks.Task.Wait()
   at Squirrel.Update.Program.executeCommandLine(String[] args)
   at Squirrel.Update.Program.main(String[] args)
---> (Inner Exception #0) System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()<---

2559-07-05 18:17:19> Program: Starting Squirrel Updater: --install .
2559-07-05 18:17:20> Program: Starting install, writing to C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 18:17:20> Program: About to install to: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom
2559-07-05 18:17:20> Program: Install path C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom already exists, burning it to the ground
2559-07-05 18:17:26> CheckForUpdateImpl: Failed to load local releases, starting from scratch: System.IO.DirectoryNotFoundException: Could not find a part of the path 'C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\packages\RELEASES'.
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileStream.Init(String path, FileMode mode, FileAccess access, Int32 rights, Boolean useRights, FileShare share, Int32 bufferSize, FileOptions options, SECURITY_ATTRIBUTES secAttrs, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.FileStream..ctor(String path, FileMode mode, FileAccess access, FileShare share)
   at Squirrel.Utility.LoadLocalReleases(String localReleaseFile)
   at Squirrel.UpdateManager.CheckForUpdateImpl.<CheckForUpdate>d__3f.MoveNext()
2559-07-05 18:17:27> CheckForUpdateImpl: Reading RELEASES file from C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\SquirrelTemp
2559-07-05 18:17:27> CheckForUpdateImpl: First run or local directory is corrupt, starting from scratch
2559-07-05 18:17:28> ApplyReleasesImpl: Writing files to app directory: C:\Users\Administrator.DN3G8ICFKBAEORE\AppData\Local\atom\app-1.8.0
2559-07-05 18:18:21> IEnableLogger: Failed to install package to app dir: System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
2559-07-05 18:18:22> Unhandled exception: System.AggregateException: One or more errors occurred. ---> System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()
   --- End of inner exception stack trace ---
   at System.Threading.Tasks.Task.ThrowIfExceptional(Boolean includeTaskCanceledExceptions)
   at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
   at System.Threading.Tasks.Task.Wait()
   at Squirrel.Update.Program.executeCommandLine(String[] args)
   at Squirrel.Update.Program.main(String[] args)
---> (Inner Exception #0) System.IO.PathTooLongException: The specified path, file name, or both are too long. The fully qualified file name must be less than 260 characters, and the directory name must be less than 248 characters.
   at System.IO.PathHelper.GetFullPathName()
   at System.IO.Path.NormalizePath(String path, Boolean fullCheck, Int32 maxPathLength, Boolean expandShortPaths)
   at System.IO.Path.GetFullPathInternal(String path)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractEntry(ZipEntry entry)
   at ICSharpCode.SharpZipLib.Zip.FastZip.ExtractZip(Stream inputStream, String targetDirectory, Overwrite overwrite, ConfirmOverwriteDelegate confirmDelegate, String fileFilter, String directoryFilter, Boolean restoreDateTime, Boolean isStreamOwner)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClassb4.<<installPackageToAppDir>b__ad>d__bd.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__50`1.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__7a.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__f.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__38.MoveNext()<---

