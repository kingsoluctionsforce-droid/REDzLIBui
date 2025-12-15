# REDz Lib UI – Full Example

## Library Load
```lua
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/kingsoluctionsforce-droid/1010183818289192028382899283818283828918282719393828283838828182838/refs/heads/main/REDzHubui"))()
```

## Window
```lua
local Window = redzlib:MakeWindow({ 
    Title = "my script",
    SubTitle = "Your Subtitle Here",
    LoadText = "Loading Text",
    Flags = "Your Flag Here"
})
```

## Minimize Button
```lua
Window:AddMinimizeButton({
    Button = {
        Image = "rbxassetid://Minimize_Icon_Asset_ID",
        BackgroundTransparency = 0
    },
    Corner = {
        CornerRadius = UDim.new(35, 1)
    },
})
```

## Tab
```lua
local MainTab = Window:MakeTab({
    Name = "",
    Icon = "rbxassetid://Tab_Icon_Asset_ID"
})
```

## Section
```lua
MainTab:AddSection({
    Name = "Main Section Name"
})
```

## TextBox
```lua
MainTab:AddTextBox({
    Name = "",
    PlaceholderText = "Placeholder Text Here",
})
```

## Discord Invite
```lua
MainTab:AddDiscordInvite({
    Name = "",
    Description = "",
    Logo = "rbxassetid://Discord_Logo_Asset_ID",
    Invite = "Discord_Invite_URL",
})
```

## Dropdown
```lua
MainTab:AddDropdown({
    Name = "",
    Options = {
        "Option Value 1",
        "Option Value 2",
        "Option Value 3"
    },
    Default = "Default Option Value",
})
```

## Paragraph
```lua
local Paragraph = MainTab:AddParagraph({
    "",
    ""
})
```

## Button
```lua
MainTab:AddButton({
    "",
    nil
})
```

## Toggle
```lua
MainTab:AddToggle({
    Name = "",
    Default = false,
})
```

## Section (Player)
```lua
MainTab:AddSection({
    Name = "Player Section Name"
})
```

## Slider
```lua
MainTab:AddSlider({
    Name = "",
    Min = 0,
    Max = 100,
    Default = 16,
})
```
