CopyRight: MJGstudio-2026;

Hello, welcome to my first app. In this app you can make your own game!

Developers:
only me for now.

How To Use:
now nothing created, so for learning scripting you need to wait. This is the start now.
But this app has some things I can say to help you. You can make [Objects, Sprites, Fonts, Paths, TileSets, Scripts].
These names are folders. In 2D project you can make [2D, 3D, VR] projects. This folders for 2D not set completely; this needs to change,
not delete but add.
Objects: some things can move, only one sprite and infinity scripts you can add.
Sprites: some images. You can edit them in engine. The edit learning in this app will come in YouTube channel after creating it.
Fonts: in the script writing we have draw_text(x,y,string,color,xscale,yscale,angle); for writing text in game. So here set_font(font); is used for making text better.
Paths: some ways the enemy or something else (but not player) can use to move with set_path(path,speed,loop); so this is good.
TileSets: something used for making 2D games like wall, door, ways, and other edit the place or location of the place. Looks like you can make home.
Scripts: I know you know what it is, but somebodies don't know. Some codes control the game. You can code: if left button hold, x -= 3; with speed 3
it moves to left, or you can use vars:

## work in start of script in some object
now_{
var xspd = 0;
var yspd = 0;

var move_spd = 3;
}

## main always plays again to check buttons
main_{
var left = keyboard_hold(char("A") or bt_left);
var right = keyboard_hold(char("D") or bt_right);
var up = keyboard_hold(char("W") or bt_up);
var down = keyboard_hold(char("S") or bt_down);

xspd = left - right * move_spd;
yspd = up - down * move_spd;
}

It can be changed because script is not created yet, and its looks like GML and its kind of copy so its gonna change so it can be changed.
These codes I say are only for 2D. The 3D is bigger than this, so wait.

Thank you.
-MJGstudio2026
