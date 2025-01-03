# IconExport
Fork of the deprecated IconExport module from TechNet

## Planned Additions
- [ ] Native PowerShell without in-line C#
- [ ] Use of the .NET Core `[Drawing.Icon]::ExtractIcon()` method (if running as PS 7) which allows for both icon index and size, which .NET Framework doesn't contain, only providing `ExtractAssociatedIcon()`.
- [ ] Support for UNC paths.
- [ ] Extracting to the source directory by default.
- [ ] Automatically naming the icon after its source, with the index and size appended to avoid clobbering. The hidden FileInfo and DirectoryInfo property `.PSIsContainer` would help there.

## Possible Additions
- [ ] Support for embedded icons in resources other than EXE and DLL... e.g.:
  - [ ] MSI. No idea how this would be done yet.
  - [ ] LNK. First getting the icon path and then extracting from there.
  - [ ] .Website (?). Easy enough, as if I recall correctly, the file follows an INI format with the field pointing to an icon file.
- [ ] Support for index and sizes other than 32px in PowerShell Desktop.

## Source
© Chrissy LeMaire [@potatoqualitee](https://github.com/potatoqualitee) 2016. I take no credit for the original module.
[PowerShell Gallery](https://www.powershellgallery.com/packages/IconExport)
[Archived Technet Gallery](https://web.archive.org/web/20200923074956/https://gallery.technet.microsoft.com/scriptcenter/Export-Icon-from-DLL-and-9d309047)

Also mentioned are:
[Thomas Levesque](http://bit.ly/1KmLgyN)
[darkfall](http://git.io/vZxRK)