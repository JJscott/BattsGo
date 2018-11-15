# BattsGo Theme for Sabaki

A theme for [Sabaki](http://sabaki.yichuanshen.de/) based on the [BattsGo](https://www.twitch.tv/battsgo/) Twitch stream. During one of the streams, the chat was talking about making a theme for the host (Dwyrin) and the idea of using the emotes as stones came up. I am a huge fan of Dwyrin, so decided to take that idea as far as I could and came up with this theme.

![Screenshot](./board_example.png)


## Features

### Stones

The stone graphics are emotes featured on the [BattsGo](https://www.twitch.tv/battsgo/) Twitch stream. The original 28x28 pixel graphics were up-sampled to 180x180 pixels using super-resolution deep convolutional neural networks for single-image anime-style art, also known as [waifu2x](http://waifu2x.udp.jp/). The up-samples were then edited to ensure that they were perfectly circular and had a hard edge. When added to the board, the stones will grow into place and will have random slight rotation to break up the visual tiling. The theme features the `battsgBfine` and `battsgWfine` emotes for normal stones and the `battsgBzstone` and `battsgWzstone` for stones that are marked as dead (dimmed) during scoring and estimation.

![Example of dimmed stones](./dimmed_example.png)


### Marks

Markers have been redesigned to fit in with the busy visuals of the stones. The background/fill for marks has been removed in favor of a transparency so there is no conflict between a flat background/fill color and the texture of the board. Text has been outlined using multi-directional text shadows, and the other marks (including lines and arrows) have been reworked to show an outline as well. Nothing can be done to unify the outline of block shapes on the cross and arrow, or to create a transparent center in the triangle, as these are limitations of using pure CSS to generate the shapes.

![Example of markers](./marker_example.png)


### Color

The color scheme was created to present a more striking visual than then typical light theme. A darker background reduces the stress on the eyes and the colors of gold on redwood gives a luxurious feel, both of which complement the busy visuals of the stones. The shadow color is closer to gold and redwood and has been made darker to emphasize the presence of cartoon-ish stones on the photographic board.
 

## Installation

[Download the theme file](https://github.com/JJscott/BattsGo/raw/master/battsgo.asar) `battsgo.asar` (or pack it yourself) and install it directly inside Sabaki under 'Preferences' > 'Themes' > 'Install Theme...'.

### Packing

Make sure you have [node.js and npm](https://nodejs.org/)  installed. If you don't have `asar` installed already, run the following command:

```
$ npm install asar -g
```

To pack your userstyle into a theme, run the following command:

```
$ asar pack ./theme ./battsgo.asar
```

`battsgo.asar` will be created and is ready for distribution.
