# Aimbot-V.2-KRNL
![image](https://user-images.githubusercontent.com/83071353/198825626-0e56ed9d-25b4-46f9-9b5b-aeda6a1b99ef.png)

## Information
This script is a universal aim-locking script. Works on all games which use the default character. This is the modified version you can use a original version here: https://github.com/Exunys/Aimbot-V2

## Configuration
This script includes settings which can be easily configured to your preference.
### Preview Of The Settings
```lua
getgenv().Aimbot.Settings = {
    SendNotifications = true,
    SaveSettings = true, -- Re-execute upon changing
    ReloadOnTeleport = true,
    Enabled = true,
    TeamCheck = false,
    AliveCheck = true,
    WallCheck = false, -- Laggy
    Sensitivity = 0, -- Animation length (in seconds) before fully locking onto target
    ThirdPerson = false, -- Uses mousemoverel instead of CFrame to support locking in third person (could be choppy)
    ThirdPersonSensitivity = 3, -- Boundary: 0.1 - 5
    TriggerKey = "E",
    Toggle = false,
    LockPart = "Head" -- Body part to lock on (Character part's name)
}

getgenv().Aimbot.FOVSettings = {
    Enabled = true,
    Visible = true,
    Amount = 90,
    Color = "255, 255, 255",
    LockedColor = "255, 70, 70",
    Transparency = 0.5,
    Sides = 60,
    Thickness = 1,
    Filled = false
}
```
### Body Part Settings Name
-Head
The head BodyPart.

-Torso
The torso BodyPart.

-LeftArm
The left arm BodyPart.

-RightArm	
The right arm BodyPart.

-LeftLeg
The left leg BodyPart.

-RightLeg
The right leg BodyPart.
## Script
### Default Version
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/LoveMig6334/Aimbot-V.2-KRNL/main/Resources/Scripts/main.lua"))()
```
### With Config Version
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/LoveMig6334/Aimbot-V.2-KRNL/main/Resources/Scripts/main.lua"))()
getgenv().Aimbot.Settings = {
    SendNotifications = true,
    SaveSettings = true, -- Re-execute upon changing
    ReloadOnTeleport = true,
    Enabled = true,
    TeamCheck = false,
    AliveCheck = true,
    WallCheck = false, -- Laggy
    Sensitivity = 0, -- Animation length (in seconds) before fully locking onto target
    ThirdPerson = false, -- Uses mousemoverel instead of CFrame to support locking in third person (could be choppy)
    ThirdPersonSensitivity = 3, -- Boundary: 0.1 - 5
    TriggerKey = "E",
    Toggle = false,
    LockPart = "Head" -- Body part to lock on (Character part's name)
}

getgenv().Aimbot.FOVSettings = {
    Enabled = true,
    Visible = true,
    Amount = 90,
    Color = "255, 255, 255",
    LockedColor = "255, 70, 70",
    Transparency = 0.5,
    Sides = 60,
    Thickness = 1,
    Filled = false
}
```
