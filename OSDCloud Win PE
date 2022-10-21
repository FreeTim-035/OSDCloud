Write-Host  -ForegroundColor Yellow "Starting Brooks' Custom OSDCloud ..."
cls
Write-Host "===================== Main Menu =======================" -ForegroundColor Yellow
Write-Host "======================== CROP =========================" -ForegroundColor Yellow
Write-Host "==================== Tim Verwoerd =====================" -ForegroundColor Yellow
Write-Host "=======================================================" -ForegroundColor Yellow
Write-Host "1: Zero-Touch Win10 21H2 | Dutch | Enterprise"-ForegroundColor Yellow
Write-Host "2: Zero-Touch Win10 20H2 | Dutch | Enterprise" -ForegroundColor Yellow
Write-Host "3: Laat me zelf kiezen"-ForegroundColor Yellow
Write-Host "4: Exit`n"-ForegroundColor Yellow
$input = Read-Host "Maak een keuze"

Write-Host  -ForegroundColor Yellow "Loading OSDCloud..."

Import-Module OSD -Force
Install-Module OSD -Force

switch ($input)
{
    '1' { Start-OSDCloud -OSLanguage nl-nl -OSBuild 21H2 -OSEdition Enterprise -ZTI } 
    '2' { Start-OSDCloud -OSLanguage nl-nl -OSBuild 20H2 -OSEdition Enterprise -ZTI } 
    '3' { Start-OSDCloud	} 
    '4' { Exit		}
}

wpeutil reboot
