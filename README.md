# polyglot-hello

A collection of minimal "Hello, World!" programs in multiple programming languages, built in parallel across Ubuntu, Windows, and macOS via GitHub Actions.

## Compiled Languages

| Language | Source |
|----------|--------|
| C        | [`c/hello.c`](c/hello.c) |
| C++      | [`cpp/hello.cpp`](cpp/hello.cpp) |
| Rust     | [`rust/hello.rs`](rust/hello.rs) |
| Go       | [`go/hello.go`](go/hello.go) |
| C#       | [`csharp/Hello.cs`](csharp/Hello.cs) |
| Java     | [`java/Hello.java`](java/Hello.java) |
| Zig      | [`zig/hello.zig`](zig/hello.zig) |
| Swift    | [`swift/hello.swift`](swift/hello.swift) |
| Kotlin   | [`kotlin/Hello.kt`](kotlin/Hello.kt) |
| Fortran  | [`fortran/hello.f90`](fortran/hello.f90) |
| Pascal   | [`pascal/hello.pas`](pascal/hello.pas) |
| Haskell  | [`haskell/hello.hs`](haskell/hello.hs) |
| Ada      | [`ada/hello.adb`](ada/hello.adb) |
| COBOL    | [`cobol/hello.cob`](cobol/hello.cob) |

## Interpreted Languages (Scripts)

| Language   | Source |
|------------|--------|
| Python     | [`python/hello.py`](python/hello.py) |
| JavaScript | [`js/hello.js`](js/hello.js) |
| Bash       | [`bash/hello.sh`](bash/hello.sh) |
| Lua        | [`lua/hello.lua`](lua/hello.lua) |
| Ruby       | [`ruby/hello.rb`](ruby/hello.rb) |
| Perl       | [`perl/hello.pl`](perl/hello.pl) |
| PowerShell | [`powershell/hello.ps1`](powershell/hello.ps1) |

## CI / Matrix Build

Every push to `main` triggers the [Matrix Build workflow](.github/workflows/build.yml), which compiles the native languages on three runners simultaneously:

- `ubuntu-latest`
- `windows-latest`
- `macos-latest`

Compiled binaries and scripts are uploaded as artifacts per OS. You can download them from the Actions run summary page or via the `gh` CLI:

```bash
gh run download --repo sadlavaarsc/polyglot-hello
```

## License

Public Domain / Unlicense — do whatever you want with it.
