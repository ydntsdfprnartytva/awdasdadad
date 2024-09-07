# Ghxst Hub

## Booting the Library
```lua
local redzlib = loadstring(game:HttpGet("https://raw.githubusercontent.com/rainhitgrassed/awdasdadad/main/source"))()
```



## Creating a Window
```lua
local Window = redzlib:MakeWindow({
  Title = "Test",
  SubTitle = "hello",
  SaveFolder = "Redz Config"
})
```



## Creating a Tab
```lua
local Tab1 = Window:MakeTab({"Tab 1", "cool"})
```

## Creating a Button
```lua
Tab1:AddButton({"Print", function()
print("Hello World!")
end})
```


## Creating a Checkbox toggle
```lua
local Toggle1 = Tab1:AddToggle({
  Name = "Speed",
  Description = "Idk",
  Default = false
})
```

## Creating a Slider
```lua
Tab1:AddSlider({
  Name = "Speed",
  Min = 1,
  Max = 100,
  Increase = 1,
  Default = 16,
  Callback = function(Value)
  game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
  end
})
