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
You can copy the Character parts name
and change as you want:
- `Head`
The head BodyPart.

- `Torso`
The torso BodyPart.

- `LeftArm`
The left arm BodyPart.

- `RightArm`
The right arm BodyPart.

- `LeftLeg`
The left leg BodyPart.

- `RightLeg`
The right leg BodyPart.
## Functions
This script includes built-in functions to control the Aimbot.
The functions can be accessed by indexing **Functions** in the Environment. Example:
```lua
getgenv().Aimbot.Functions
```
### Their purposes
* `Functions:Exit()`
  - Exits (unexecutes) the script and leaves no traces back.
* `Functions:Restart()`
  - Restarts the script, good for incase the script starts lagging.
* `Functions:ResetSettings()`
  - Factory resets the settings and wipes the previous ones that were saved to the workspace.

- Exit
```lua
getgenv().Aimbot.Functions:Exit()
```
- Restart
```lua
getgenv().Aimbot.Functions:Restart()
```
- Reset Settings
```lua
getgenv().Aimbot.Functions:ResetSettings()
```
## Hotkey
If you want to change the key you want to press to trigger the Aimbot, configure the ***TriggerKey*** setting.
- *Examples* :
```lua
getgenv().Aimbot.Settings.TriggerKey = "E" -- E is the key's name (This is equivalent to Enum.KeyCode.E, except, the script only handles strings)
```
```lua
getgenv().Aimbot.Settings.TriggerKey = "MouseButton1" -- MouseButton1 is the key's name [LMB] (This is equivalent to Enum.UserInputType.MouseButton1, except, the script only handles strings)
```
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
