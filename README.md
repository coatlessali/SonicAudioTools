# Sonic Audio Tools

A set of tools to modify CRIWARE file formats. Library fork for HoneyPatcher by coatlessali.

## Changes

- Removed setting console cursor position as it causes an error on Windows if not run through CMD.
- Changed the AcbEditor and CsbEditor classes to public, and their Main() methods to AcbEdit() and CsbEdit().

## Building

Instructions are for building on Arch Linux.

1. Install `mono` and `mono-msbuild`.
2. Clone from [GitHub](https://github.com/coatlessali/SonicAudioTools.git) `git clone https://github.com/coatlessali/SonicAudioTools.git`
3. `cd SonicAudioTools`
4. `cd` into either `AcbEditor` or `CsbEditor`, depending on which one you want to build.
5. Use `msbuild` on the `.csproj` file.
6. Copy produced DLLs to HoneyPatcher source directory.

The rest of the readme is left mostly untouched:

## Projects

If you wish to see more detailed information about the projects, visit the upstream [wiki](https://github.com/blueskythlikesclouds/SonicAudioTools/wiki) page.

### [Sonic Audio Library](https://github.com/blueskythlikesclouds/SonicAudioTools/tree/master/Source/SonicAudioLib)

This is the main library of the solution.  Contains classes for IO and file formats.

### [ACB Editor](https://github.com/blueskythlikesclouds/SonicAudioTools/tree/master/Source/AcbEditor)

This tool allows you to edit the audio content of an ACB file.  

### [ACB Finder](https://github.com/blueskythlikesclouds/SonicAudioTools/tree/master/Source/AcbFinder)

This tool allows you to find AWB files and link them back to the ACB, required in extracting certain ACB files.
Useful for games where the AWB files may be renamed or hidden (like Phantasy Star Online 2)

### [ACB Injector](https://github.com/blueskythlikesclouds/SonicAudioTools/tree/master/Source/AcbInjector)

This tool allows you to inject audio file directly into ACB without repacking its AWB.  
Useful for background music ACBs that use huge AWB files.

### [CSB Builder](https://github.com/blueskythlikesclouds/SonicAudioTools/tree/master/Source/CsbBuilder)

This tool allows you to create or edit CSB files. You can do things like adding/removing cues, editing real-time sound parameters, and more.

### [CSB Editor](https://github.com/blueskythlikesclouds/SonicAudioTools/tree/master/Source/CsbEditor)

This tool allows you to edit the audio content of a CSB file.  
It works like ACB Editor, and it is a lot simpler to use than CSB Builder.

## License

See [LICENSE.md](https://github.com/blueskythlikesclouds/SonicAudioTools/blob/master/LICENSE.md) for details.
