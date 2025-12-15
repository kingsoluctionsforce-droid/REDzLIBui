## Component Documentation

### # MakeWindow

Creates the main container for the UI, handling the title and initial load settings.

```lua
local Window = redzlib:MakeWindow({ 
    Title = "Your Title Here",
    SubTitle = "Your Subtitle Here",
    LoadText = "Loading Text",
    Flags = "Your Flag Here"
})

# AddMinimizeButton
Adds the minimize function to the main window. This is usually defined right after the Window is created.
Window:AddMinimizeButton({
    Button = { Image = "rbxassetid://Minimize_Icon_Asset_ID", BackgroundTransparency = 0 },
    Corner = { CornerRadius = UDim.new(35, 1) },
})

# MakeTab
Creates a new tab section within the main window.
local MainTab = Window:MakeTab({
    Name = "Tab Name Here",
    Icon = "rbxassetid://Tab_Icon_Asset_ID"
})

# AddSection
Adds a visual separator/grouping title within a tab.
MainTab:AddSection({
    Name = "Section Name Here"
})

# AddTextBox
Creates an input field for the user to type text.
MainTab:AddTextBox({
    Name = "Input Name Here",
    PlaceholderText = "Placeholder Text Here",
})

# AddToggle
Creates a simple ON/OFF switch.
MainTab:AddToggle({
	Name = "Toggle Name Here",
	Default = false,
})

# AddButton
Creates a clickable button to execute an action.
MainTab:AddButton({
    "Button Label Here",
    nil -- Placeholder for Callback
})

# AddSlider
Creates a draggable bar to select a numeric value within a defined range.
MainTab:AddSlider({
    Name = "Slider Name Here",
    Min = 0,
    Max = 100,
    Default = 16,
})

# AddDropdown
Creates a selectable list of options.
MainTab:AddDropdown({
    Name = "Dropdown Name Here",
    Options = {
        "Option Value 1",
        "Option Value 2",
        "Option Value 3"
    },
    Default = "Default Option Value",
})

# AddDiscordInvite
Adds a dedicated component for displaying a Discord invite link/logo.
MainTab:AddDiscordInvite({
    Name = "Discord Name Here",
    Description = "Discord Description Here",
    Logo = "rbxassetid://Discord_Logo_Asset_ID",
    Invite = "Discord_Invite_URL",
})

# AddParagraph
Adds a multi-line text block for notes or credits.
local Paragraph = MainTab:AddParagraph({
    "Line 1 Text Here", 
    "Line 2 Text Here"
})


