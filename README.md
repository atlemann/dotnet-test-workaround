# dotnet test net461 workaround
A workaround for running `dotnet test` on Linux/Mac with `net461` (https://github.com/Microsoft/vstest/issues/1284)

1. Add the `netfx.props` file in your `.*proj` file, which points dotnet CLI to the Mono paths according to target framework.
2. Make sure you use the plural form `TargetFrameworks` even when defining a single target (I have no idea why...) 
