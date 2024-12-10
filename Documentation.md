# Orion Library
This documentation is for the stable release of Orion Library.

## Booting the Library
```lua
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
```



## Creating a Window
```lua
local Window = OrionLib:MakeWindow({Name = "Shadow", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})
```



## Creating a Tab
```lua
            local Tab = Window:MakeTab({
              	Name = "XXXXXXX",
              	Icon = "rbxassetid://",
              	PremiumOnly = false
              }
            )

```
## Creating a Section
```lua
local Section = Tab:AddSection({
	Name = "Section"
})

--[[
Name = <string> - The name of the section.
]]
```
You can add elements to sections the same way you would add them to a tab normally.

## Notifying the user
```lua
OrionLib:MakeNotification({
	Name = "Title!",
	Content = "Notification content... what will it say??",
	Image = "rbxassetid://4483345998",
	Time = 5
})
```



## Creating a Button
```lua
      Tab:AddButton({
        	Name = "Button!",
        	Callback = function()
              		
          	end    
        }
      )
```


## Creating a Checkbox toggle
```lua
              Tab:AddToggle({
                	Name = "toggle",
                	Default = false,
                	Callback = function(Value)
                		
              end    
            }
          )
```

### Changing the value of an existing Toggle
```lua
CoolToggle:Set(true)
```



## Creating a Color Picker
```lua
Tab:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})

--[[
Name = <string> - The name of the colorpicker.
Default = <color3> - The default value of the colorpicker.
Callback = <function> - The function of the colorpicker.
]]
```

### Setting the color picker's value
```lua
ColorPicker:Set(Color3.fromRGB(255,255,255))
```


## Creating a Slider
```lua
      Tab:AddSlider({
        	Name = "Slider",
        	Min = 0,
        	Max = 20,
        	Default = 5,
        	Color = Color3.fromRGB(255,255,255),
        	Increment = 1,
        	ValueName = "bananas",
        	Callback = function(Value)
        		
      end    
    }
  )
```

### Change Slider Value
```lua
Slider:Set(2)
```
Make sure you make your slider a variable (local CoolSlider = Tab:AddSlider...) for this to work.


## Creating a Label
```lua
Tab:AddLabel("Label")
```

### Changing the value of an existing label
```lua
CoolLabel:Set("Label New!")
```


## Creating a Paragraph
```lua
Tab:AddParagraph("Paragraph","Paragraph Content")
```

### Changing an existing paragraph
```lua
CoolParagraph:Set("Paragraph New!", "New Paragraph Content!")
```


## Creating an Adaptive Input
```lua
            Tab:AddTextbox({
              	Name = "Textbox",
              	Default = "default box input",
              	TextDisappear = true,
              	Callback = function(Value)
              		
              end	  
            }
          )

```


## Creating a Dropdown menu
```lua
          Tab:AddDropdown({
            	Name = "Dropdown",
            	Default = "",
            	Options = {""},
            	Callback = function(Value)
            		
            end    
          }
        )

```
