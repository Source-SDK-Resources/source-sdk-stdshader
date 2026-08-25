# Source 2013 stdshader

This repo contains the setup for compiling a funtional **stdshader_xxx** for Source 2013, where xxx can be **dbg/dx6/dx7/dx8/dx9.**

## Integrating
Download the [DX9 SDK](https://www.microsoft.com/en-us/download/details.aspx?id=6812) and extract it into the src/dx9sdk folder.

Add the following to **vpc_scripts/projects.vgc**:
```
$Project "stdshader_xxx"
{
	"materialsystem\stdshader\stdshader_xxx.vpc"
}
```
Then, in **vpc_scripts/groups.vgc**, add `"stdshader_xxx"` to the group of your choice.

## See Also
The **shader_dll_verify.h/cpp** code is extracted from [Orange Box SDK](https://github.com/Source-SDK-Archives/source-sdk-orangebox/tree/master/materialsystem/shaderlib), with minor fixes.

