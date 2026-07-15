<p align="center">
  <a href="github.com/cursed-blip/madara.wtf">
    <img src="https://media.discordapp.net/attachments/1497579415947706491/1527061123784904794/Screenshot_2026-07-15_210610.png?ex=6a5949ff&is=6a57f87f&hm=6be1e5d8ec100575e89a52c6701e038cf605df3e7f4658a4d502ebb1bda7c3f2&=&format=webp&quality=lossless&width=434&height=424" alt="Madara Logo" width="72" height="72">
  </a>

  <h3 align="center">madara.wtf</h3>

<p align="center">
  <a href="https://discord.gg/tcQSp98FSX">
    <img src="https://img.shields.io/badge/💬%20Join%20Discord-cc0000?style=for-the-badge&logo=discord&logoColor=white" alt="Join Discord">
  </a>
</p>


## Table of contents

- Tabs, group boxes, and tab boxes
- Fully featured UI components (toggles, sliders, dropdowns, keybinds, color pickers, etc.)
- Automatic scrolling when UI elements exceed available space
- Dependency boxes for dynamically showing/hiding elements
- Config saving and loading support
- Custom themes and styling support
- Notifications and utility features


## Quick start

Getting started with Madara is simple:

```lua
local Madara = loadstring(game:HttpGet("YOUR_LIBRARY_URL"))()

local Window = Madara:CreateWindow({
    Title = "Madara Example",
    Center = true,
    AutoShow = true
})

local Tab = Window:AddTab("Main")

local Groupbox = Tab:AddLeftGroupbox("Settings")

Groupbox:AddToggle("ExampleToggle", {
    Text = "Enable Feature",
    Default = false
})
