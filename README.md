# Disable ActivityCache and widgets completely
## tested on Microsoft Windows 11 Home version 25H2 10.0.26200.7171

  -exec(add) this regfile
  -restart
  -delete following directory
  ``%LocalAppData%\ConnectedDevicesPlatform``
  
  
  check absence of widgets with no widgets appearing in the taskmanager
  additional remove widget package with admin-powershell
  ``Get-AppxPackage *WebExperience* | Remove-AppxPackage``
