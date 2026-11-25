# MJGgameEngine

**Copyright:** MJGstudio-2026

## Introduction

Hello, and welcome to our first application!

With this application, you will be able to create your own games.

## Developers

Currently, I am the only developer working on this project for now.

## How to Use

Nothing has been fully implemented yet, so you will need to wait for future updates to learn how to use the scripting system. This is just the beginning of the project.

However, there are already some planned features that I can introduce.

You will be able to work with the following folders and resources:

- Scenes
- Objects
- Sprites
- Fonts
- Paths
- TileSets
- Scripts

These are the main categories used to organize your game projects.

The engine is intended to support different project types, including **2D, 3D, and VR**. The current 2D project structure is not complete yet. It will be expanded with additional features and folders rather than having its existing structure removed.

### Scenes

Scenes are the main containers of your game. They allow you to organize and place the different elements that make up each part of your game.

### Objects

Objects represent the entities in your game.

Each object can have one sprite assigned to it at a time. You can also change or remove its sprite through code. An object without a sprite can still exist and be controlled through scripts, even though it will not be visible.

You can also attach an unlimited number of scripts to an object.

### Sprites

Sprites are images used in your games.

You will be able to create and edit sprites directly inside the engine. Tutorials explaining how to use the Sprite Editor will be published on our YouTube channel after it is created.

### Fonts

Fonts are used to display text in your games.

The scripting system will provide functions such as:

`draw_text(x, y, string, color, xscale, yscale, angle);`

This function will be used to draw text with different positions, colors, scales, and rotation angles.

You will also be able to select a font using:

`set_font(font);`

This allows you to customize the appearance of text in your game.

### Paths

Paths define movement routes that enemies and other objects can follow. They are not intended for player movement.

For example, you will be able to use:

`set_path(path, speed, loop);`

This function assigns a path to an object and controls its movement speed and whether the path should repeat.

### TileSets

TileSets contain reusable elements for building 2D environments.

They can include walls, doors, roads, and other elements used to construct levels and environments. You can use them to build places such as houses, rooms, and other locations.

### Scripts

Scripts contain code that controls different parts of your game.

They can include functions for handling gameplay, object behavior, and events. Events can be handled through functions inside scripts.

For example, you could move an object to the left when the left button is held:

`x -= 5;`

This moves the object five pixels (in 2D) to the left.

You can also use variables and conditions to control movement. Here is an example of a possible 2D script:

## main_update always runs every frame to check buttons
func main_update()
{
    var left = keyboard_hold(char("A") || bt_left);
    var right = keyboard_hold(char("D") || bt_right);
    var up = keyboard_hold(char("W") || bt_up);
    var down = keyboard_hold(char("S") || bt_down);

    if (left)
    {
        x -= 5;
    }

    if (right)
    {
        x += 5;
    }

    if (up)
    {
        y += 5;
    }

    if (down)
    {
        y -= 5;
    }
}

**Important:** This scripting syntax is only an example of the planned language, called **MscriptMGE**. Since the scripting system has not been developed yet, its syntax and functions may change during development.

These examples are intended for 2D projects only. The 3D scripting system will be more extensive and will have additional functionality.

## Created With

- C
- SFML 3.1.0

Thank you for your interest in MJGgameEngine!

**MJGstudio-2026**
