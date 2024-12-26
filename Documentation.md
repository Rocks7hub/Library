# Orion Library - Shadow
This documentation is for the stable release of Orion Library.

## Booting the Library
```lua
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
```



## Creating a Window
```lua
local Window = OrionLib:MakeWindow({Name = "Shadow", HidePremium = false, SaveConfig = true, ConfigFolder = "ShadowLib"})
```



## Creating a Tab
```lua
            local Tab = Window:MakeTab({
              	Name = "Shadow",
              	Icon = "rbxassetid://",
              	PremiumOnly = false
              }
            )

```
## Creating a Section
```lua
            local Section = Tab:AddSection({
            	Name = "Section"
            }
          )
```
You can add elements to sections the same way you would add them to a tab normally.

## Notifying the user
```lua
              OrionLib:MakeNotification({
              	Name = "Shadow",
              	Content = "Cristo É O Senho!",
              	Image = "rbxassetid://4483345998",
              	Time = 5
              })
```



## Creating a Button
```lua
      Tab:AddButton({
        	Name = "Shadow",
        	Callback = function()
              		
          	end    
        }
      )
```


## Creating a Checkbox toggle
```lua
              Tab:AddToggle({
                	Name = "Shadow",
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



### Setting the color picker's value
```lua
ColorPicker:Set(Color3.fromRGB(255,255,255))
```


### Change Slider Value
```lua
Slider:Set(2)
```

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
              	Name = "Shadow",
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
            	Name = "Shadow",
            	Default = "",
            	Options = {""},
            	Callback = function(Value)
            		
            end    
          }
        )

```
