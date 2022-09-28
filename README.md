# A Home Assistant dashboard for mobile, tablet and desktop
This repository contains code examples to support articles written on my blog [TheAwesomeGarage.com](https://theawesomegarage.com).

NOTE! You need to modify this code to work with browser-mod 2. The good news: it's pretty easy! You mostly only have to change the popups.

This is an example of how a popup could look like with browser-mod 2:

```
action: fire-dom-event
browser_mod:
  service: browser_mod.popup
  data:
    size: wide
    title: Energy consumption
    content:
      type: custom:layout-card
      layout_type: custom:horizontal-layout
      layout:
        width: 400
        max_cols: 3
        card_margin: 15px
        margin: 4px 50px 0px 50px
      cards:
        - type: custom:apexcharts-card
        ...
```
