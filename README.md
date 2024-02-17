# Clang Tidy

This repository holds my personal .clang-tidy file that I use in all my C++ projects and occassionally update.

## Checks enabled

The [list of all Clang Tidy checks can be found here.](https://clang.llvm.org/extra/clang-tidy/checks/list.html)

I have enabled the following subsection:

- `cert-*`: All checks related to the CERT Secure Coding Guidelines.
- `clang-analyzer-*`: All Clang Static Analyzer checks.
- `bugprone-*`: All checks that target bug-prone code constructs.
- `concurrency-*`: All checks related to concurrent programming.
- `cppcoreguidelines-*`: All checks related to the C++ Core Guidelines.
- `modernize-*`: All checks that advocate the usage of modern C++ language constructs.
- `performance-*,portability-*,readability-*`: All checks that target performance, portability and readability related issues, with the exception of `portability-restrict-system-includes` and `readability-suspicious-call-arguments`.
- A few Google and LLVM checks such as `google-explicit-constructor` and `llvm-include-order`.

In addition to Clang Tidy, I rely on CLion's checking of compliance with MISRA C++ 2008.