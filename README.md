# Shadow.cc

## Booting the Library
```lua
loadstring(game:HttpGet('https://raw.githubusercontent.com/rainhitgrassed/awdasdadad/main/ui'))()
```



## Creating a Window
```lua
local Library = initLibrary()
local Window = Library:Load({name = "xan", sizeX = 425, sizeY = 512, color = Color3.fromRGB(255, 255, 255)})
```



## Creating a Tab
```lua
local Tab = Window:Tab("Aiming")
```

## Creating a Section
```lua
local Aimingsec1 = Tab:Section{name = "Aim Assist", column = 1}
```

## Creating a toggle
```lua
       Aimingsec2:Toggle {
    Name = "Enabled",
    flag = "ooolol", 
    callback = function(bool)

    end
}
```

## Creating a Slider
```lua
    Aimingsec1:Slider {
    Name = "Smoothing",
    Default = 0,
    Min = 0,
    Max = 30,
    Decimals = 1,
    Flag = "moooooo",
    callback = function(bool)

    end
}
```
