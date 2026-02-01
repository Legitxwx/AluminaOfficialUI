# Alumina UI
```lua
local Alumina = loadstring(game:HttpGet("https://raw.githubusercontent.com/Legitxwx/AluminaOfficialUI/main/source.lua"))()

local Window = Alumina:CreateWindow({
    Title = "Alumina Master UI"
})

local Tab = Window:Tab({
    Title = "Home"
})

-- Now you can store them all in variables
local Button = Tab:Button({
    Title = "Click Me",
    Callback = function()
        print("Button clicked!")
    end
})

local Toggle = Tab:Toggle({
    Title = "Speed Hack",
    Callback = function(state)
        print("Toggle is:", state)
    end
})

local Slider = Tab:Slider({
    Title = "Gravity Power",
    Min = 0,
    Max = 500,
    Default = 196,
    Callback = function(val)
        workspace.Gravity = val
    end
})

local Input = Tab:Input({
    Title = "Username",
    Placeholder = "Enter name...",
    Callback = function(text)
        print("You entered:", text)
    end
})

local Dropdown = Tab:Dropdown({
    Title = "Select Team",
    List = {"Guards", "Prisoners", "Neutral"},
    Callback = function(choice)
        print("Selected team:", choice)
    end
})
```
