# wcc
## The Microsoft Word C Compiler 

Are you tired of using VS Code and Atom? 
Are you sick of colourful syntax highlighting?
Does vim make you want to die?

And have you ever dreamed of using Word as your text editor of choice?

Say no more! Write all of your wonderful C code in Microsoft Word and compile
using `wcc`! Your C code has never looked so bright!

## Flags 

WCC supports most of the major operations that you would expect from GCC, 
including common flags like `-c` and `-std=`. Support for more flags is coming
soon!

`-Wwarning`: Set warnings, i.e. all, error

`-c`: Compile, but do not link

`-o name`: Specify the output filename 

`-std=std`: Set the C standard to use, i.e. c99

`-h`: Show help menu

## Examples

Here are some examples of how you can use WCC to revolutionize your development!

Compile a simple file into `a.out`:
```sh
wcc myProgram.docx
```

Generate object file and specify the output name
```sh
wcc -c -o output.o myProgram.docx
```

Be very strict with your warnings (recommended)
```sh
wcc -Wall -Werror myProgram.docx
```

When you don't know what to do
```sh
wcc -h
# Or, perhaps more whistfully, `gcc -h`
```