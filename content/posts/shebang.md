---
title: "Shebang (#!)"
description: "Shebang: Understanding the mysterious first line of a Linux script"
date: "2023-05-04 12:30:00 +05:30"

author: "Siddharth Arumugam"
tags: ["linux", "bash", "scripting"]
cover: "https://cdn.jsdelivr.net/gh/0xMrNight/blog-images@master/2023/05/shebang.jpg"
---

## What is the shebang?

The shebang (`#!`) is placed at the top of a script and is used to tell the kernel which interpreter to execute to read the script.

Syntax:
```bash
#!/path/to/interpreter [parameters (optional)]
```

The name _shebang_ or _hashbang_ comes from # (SHArp or HASH) and ! (bang).

> Using a shebang like `#!/usr/bin/echo` will output just the filename (linux _echo_ command),
> similarly `#!/usr/bin/cat` will output the contents of the file (linux _cat_ command).

Note: Shebangs max out at 127 characters.

### #!/usr/bin/env name

The `/usr/bin/env` command looks for and runs the first executable it finds in the user's `$PATH` in a separate shell instance.

- The `#!/usr/bin/env` shebang is used to increase portability of code.
- It is also used in cases where the absolute path to the interpreter is unknown or may vary (such as when handling different versions of node with the Node Version Manager ([nvm](https://github.com/nvm-sh/nvm))).

```bash
#!/usr/bin/env node
```

Note: Arguments cannot be passed on to the interpreter when using `#!/usr/bin/env`.

### Why `#!`?

The character sequence `#!`is encoded to the bytes `23 21`, which is the magic number of an executable script.[^1]

> A _magic number_ or _file signature_ is a sequence of bytes at the beginning of a file that allows to identify the type of file.
> For example, a ZIP file has a file signature of `50 4B 03 04`.[^2]

Ref:

- [What the #! shebang really does](https://dev.to/meleu/what-the-shebang-really-does-and-why-it-s-so-important-in-your-shell-scripts-2755) by meleu
- [what is a shebang (#!)?](https://youtu.be/g3VxRdtlMoE) by anthonywritescode

[^1]: [An email from Dennis Ritchie on #!](https://www.in-ulm.de/~mascheck/various/shebang/4.0BSD_newsys_sys1.c.html), 1980
[^2]: [List of file signatures](https://en.wikipedia.org/wiki/List_of_file_signatures)