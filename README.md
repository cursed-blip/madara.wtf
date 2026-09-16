<p align="center">
  <a href="https://github.com/cursed-blip/madara.wtf">
    <img src="https://media.discordapp.net/attachments/1497579415947706491/1536767851895988285/image.png?ex=6a7c9a17&is=6a7b4897&hm=e0d2c0b64cba0ee78c5891fde252d2db431b2dcf385fdda067dfcf2dd2960944&=&format=webp&quality=lossless" alt="Madara Logo" width="72" height="72">
  </a>
</p>

<h3 align="center">madara.wtf</h3>

<p align="center">A modern Roblox UI library — clean, fast, and easy to theme.</p>

<p align="center">
  <img src="https://cdn.simpleicons.org/lua/black/white" width="28" height="28" alt="Lua" />
  &nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/roblox/black/white" width="28" height="28" alt="Roblox" />
  &nbsp;&nbsp;
  <a href="https://discord.gg/tcQSp98FSX">
    <img src="https://cdn.simpleicons.org/discord/black/white" width="28" height="28" alt="Discord" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/cursed-blip/madara.wtf/stargazers">
    <img src="https://img.shields.io/github/stars/cursed-blip/madara.wtf?style=flat-square&label=stars" alt="Stars">
  </a>
  <a href="https://github.com/cursed-blip/madara.wtf/network/members">
    <img src="https://img.shields.io/github/forks/cursed-blip/madara.wtf?style=flat-square&label=forks" alt="Forks">
  </a>
</p>

## Table of Contents

- [Features](#features)
- [Preview](#preview)
- [Quick Start](#quick-start)
- [API Structure](#api-structure)

## Features

- Tabs, group boxes, and tab boxes
- Toggles, sliders, dropdowns, keybinds, color pickers, and more
- Automatic scrolling when content overflows
- Dependency boxes for dynamically showing / hiding elements
- Config saving and loading
- Custom themes and styling
- Notifications and utilities

## Preview

<p align="center">
  <img src="https://media.discordapp.net/attachments/1536765627149320202/1536765627392458812/image.png?ex=6aac0e05&is=6aaabc85&hm=b592c86ab4f799819ca2b3ac453ea7a65f4a922b02fe6d9d54703a756fe73375&=&format=webp&quality=lossless" alt="madara.wtf preview" width="100%">
</p>

## Quick Start

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
