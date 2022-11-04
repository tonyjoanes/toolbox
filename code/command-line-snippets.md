# Command Line Snippets

## Delete `obj` and `bin` folders from project

Windows command line snippet to delete the `obj` and `bin` folders from a .NET project.
This has come in handy when receiving dreaded CSC errors and rebuilds are not working!

> Run this in windows command

```cmd
FOR /F "tokens=*" %G IN ('DIR /B /AD /S obj') DO RMDIR /S /Q "%G"
FOR /F "tokens=*" %G IN ('DIR /B /AD /S bin') DO RMDIR /S /Q "%G"
```
