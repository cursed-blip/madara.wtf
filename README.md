<p align="center">
  <a href="https://github.com/cursed-blip/madara.wtf">
    <img src="https://media.discordapp.net/attachments/1497579415947706491/1536767851895988285/image.png?ex=6a7c9a17&is=6a7b4897&hm=e0d2c0b64cba0ee78c5891fde252d2db431b2dcf385fdda067dfcf2dd2960944&=&format=webp&quality=lossless" alt="Madara Logo" width="72" height="72">
  </a>
</p>

<h3 align="center">madara.wtf</h3>

<p align="center">
  <a href="https://discord.gg/tcQSp98FSX">
    <img src="https://img.shields.io/badge/💬%20Join%20Discord-cc0000?style=for-the-badge&logo=discord&logoColor=white" alt="Join Discord">
  </a>
</p>

## Table of Contents

* Tabs, group boxes, and tab boxes
* Fully featured UI components (toggles, sliders, dropdowns, keybinds, color pickers, etc.)
* Automatic scrolling when UI elements exceed available space
* Dependency boxes for dynamically showing/hiding elements
* Config saving and loading support
* Custom themes and styling support
* Notifications and utility features

## Quick Start

Getting started with Madara is simple:

```lua
local Madara = loadstring(game:HttpGet("https://raw.githubusercontent.com/cursed-blip/madara.wtf/main/madara.lua"))()

local Window = Madara:CreateWindow({
    Name = "Madara Example"
})

local Tab = Window:AddTab("Main")
local Section = Tab:AddSection("Example")

Section:AddToggle({
    Name = "God Mode",
    Flag = "GodMode"
})

Section:AddButton({
    Name = "Execute",
    Callback = function()
        print("Executed!")
    end
})
```

## API Structure

```text
Window
└── Tab
    └── Section
        ├── Label
        ├── Toggle
        ├── Button
        ├── Slider
        ├── Dropdown
        ├── SearchBox
        ├── Textbox
        ├── Keybind
        ├── Colorpicker
        ├── Persistence
        └── Designer
```
