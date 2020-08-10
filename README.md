# uilib
Expression 2 UI Library for Gmod (Garry's Mod)

# Readme:
Save as "ui/" folder inside expression2.
  
# Usage:
## Initialization
>In the newest version youll have to call EGP:initUI() before everything, this ensures the latest customizations are loaded.
## Buttons  
>EGP:createbutton(Position:vector2, Size:vector2, Text:string, Text Size:number)  
## Text Fields  
>EGP:createtextfield(Position:vector2, Size:vector2, Text:string, Text Size:number)  
## Progress Bars
>EGP:createprogressbar(Position:vector2,Size:vector2)  
>EGP:updateprogress(Bar,Progress)  
## Theming
You can use its Theming capabilities to customize your uilib instance!  
## Specifying a theme  
Specify it in uilib.txt via #include "your/path/to/theme.txt"  
## Modding a theme
There are several themes already for you to toy around with, go ahead, just modify some of them!  
Keep in mind, that some textures cannot be rendered in EGP and will break the Theme doing so.  
## Useful stuff
Check out the examples too! (togglebtn, singlebtn and keypad)  
  
Theme support has been added as of this repo creation.  
  
P.S: Shoutout to TSCM, i was banned ages ago but LINK, YOU ROCK!  
