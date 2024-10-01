## Get Loadstring
```lua
local VenomLibrary = loadstring(game:HttpGet(('https://raw.githubusercontent.com/ydntsdfprnartytva/Venom.cc-Library/refs/heads/main/source')))()
```
## Create Window
```lua
local Window = VenomLibrary:MakeWindow({Name = "Title of the library", HidePremium = false, SaveConfig = true, ConfigFolder = "Venom Test"})
```
## Create Tab
```lua
local tab1 = Window:MakeTab({
	Name = "Main",
	Icon = "", -- dont add a icon
	PremiumOnly = false
})
```
## Create Section
```lua
local sec1 = tab1:AddSection({
	Name = "Stuff"
})
```
## Create Button
```lua
tab1:AddButton({
	Name = "Button!",
	Callback = function()
      		print("button pressed")
  	end    
})
```
## Create Toggle
```lua
tab1:AddToggle({
	Name = "Fly",
	Default = false,
	Callback = function(Value)
		print(Value)
	end    
})
```
## Create Slider
```lua
Tab:AddSlider({
	Name = "Walkspeed",
	Min = 0,
	Max = 25,
	Default = 5,
	Color = Color3.fromRGB(77,12,214),
	Increment = 1,
	ValueName = "", -- do not add nothing to it
	Callback = function(Value)
		print(Value)
	end    
})
```
## Create Dropdown
```lua
tab1:AddDropdown({
	Name = "Dropdown",
	Default = "1",
	Options = {"1", "2"},
	Callback = function(Value)
		print(Value)
	end    
})
```
## Create Keybind
```lua
tab1:AddBind({
	Name = "Bind",
	Default = Enum.KeyCode.E,
	Hold = false,
	Callback = function()
		print("press")
	end    
})
```
## Create ColorPick
```lua
tab1:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})
```
## End/Finish the script
```lua
VenomLibrary:Init()
```
