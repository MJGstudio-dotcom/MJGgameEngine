CopyRight: MJGstudio-2026;

Hello, welcome to us first app. In this app you can make your own game!

Developers:
only me for now.

How To Use:
now nothing created, so for learning scripting you need to wait. This is the start now.
But this app has some things I can say to help you. You can make [Scenes, Objects, Sprites, Fonts, Paths, TileSets, Scripts].
These names are folders. In 2D project you can make [2D, 3D, VR] projects. This folders for 2D not set completely; this needs to change,
not delete but add.
Scenes:the main things, to show everything in game you place in them.
Objects: some things can move, you can select only one sprite(can change by code) at time and you can doesn`t select to be invisble to control game and infinitly scripts you can add.
Sprites: some images. You can edit them in engine. The edit learning in this app will come in YouTube channel after creating it.
Fonts: in the script writing we have draw_text(x,y,string,color,xscale,yscale,angle); for writing text in game. So here set_font(font); is used for making text better.
Paths: some ways the enemy or something else (but not player) can use to move with set_path(path,speed,loop); so this is good.
TileSets: something used for making 2D games like wall, door, ways, and other edit the place or location of the place. Looks like you can make home.
Scripts: I know you know what it is, but somebodies don't know. Some codes control the game, they have some functions for control events and events can be in every script you want. You can code: if left button hold, x -= 5; with speed 5
it moves to left, or you can use vars:

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

It can be changed because MscriptMGE is not created yet, so it can be changed.
These codes I say are only for 2D. The 3D is bigger than this, so wait.

Created With:
C and SFML 3.1.0.

Thank you.
-MJGstudio2026
