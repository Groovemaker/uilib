# uilib
Expression 2 UI Library for Gmod (Garry's Mod)

# Readme:
Save as "ui/" folder inside expression2.
  
  
# Usage:
## Initialization
In the newest version youll have to call EGP:initUI() before everything, this ensures the latest customizations are loaded.  
## Buttons  
EGP:createbutton(Position:vector2, Size:vector2, Text:string, Text Size:number)  
EGP:createbuttonEx(ID:number, Position:vector2, Size:vector2, Text:string, TextSize:number)  
## Icon Buttons  
EGP:createiconbutton(Position:vector2,Size:vector2,Texture:string,IconSize:vector2)  
EGP:createiconbuttonEx(ID:number,Position:vector2,Size:vector2,Texture:string,IconSize:vector2)  
## Text Fields  
EGP:createtextfield(Position:vector2, Size:vector2, Text:string, Text Size:number)  
## Progress Bars  
EGP:createprogressbar(Position:vector2,Size:vector2)  
EGP:updateprogress(Bar,Progress)
## Popups  
EGP:popup(Title:string, Size:vector2, Text:string, TextSize:number) - returns: Array:CloseBtnID,Size)  
EGP:closepopup(Popup:array)
EGP:movepopup(Popup:array,Pos:vector2)
## Cursor Support  
EGP:cursor()  
(Call it in a loop.)  
## Transforming
EGP:uiSetPos(ID:number,Pos:vector2)  
  
## Theming  
You can use its Theming capabilities to customize your uilib instance!  
## Specifying a Ttheme  
Specify it in uilib.txt via #include "your/path/to/theme.txt"  
## Modding a Theme
There are several themes already for you to toy around with, go ahead, just modify some of them!  
Keep in mind, that some textures cannot be rendered in EGP and will break the Theme doing so.  

## Some Theming Vars with examples
### General
ThemeStyle = "Modern" (This is the Style of the theme, Possible values: "Modern". Omit variable for minimal theme.)  
CursorEnable = 1 (Enables/Disables Cursor)  
BackgroundEnable = 1 (Enables/Disables Background)  
### Design Related
CursorMat = "icon16/cursor.png" (Texture of the Cursor if enabled)  
TxtFont = "DermaDefault" (Font for Text related elements)  
ButtonStyle = "Gradient" (Button Style, Possible values: "Gradient", "Rounded")  
Background = "gui/noicon.png" (Texture of the Background if enabled)  
BtnForeColor = vec(111,11,255) (Theme Palette Color 1)  
Gradient = vec(111,111,255) (Gradient Color if enabled)  
BtnForeColor2 = vec(255) (Theme Palette Color 2)  
BtnAlpha = 155 (Alpha of Elements)  
BtnTextColor = vec(255) (Text Color of all Elements)  
### Feedback Related
BtnPressColor = BtnForeColor * 2 (Button Pressing Color)  
BtnWrongColor = vec(255,0,0) (Button Wrong Color for use with keypads, warnings, etc)  
BtnRightColor = vec(0,255,0) (Button Right Color, ditto)  
PressSnd = "buttons/button16.wav" (Button Press Sound, put "" for quiet)  

# MOUSE SUPPORT!!
uilib now supports mouse!
If you wish to use mouse to operate panels, please enable "MouseEnabled" to 1 in ui/uilib.txt!  
  
## Useful stuff
Check out the examples too! (togglebtn, singlebtn and keypad, etc)  
Theme support has been added as of this repo creation.  
  
P.S: Shoutout to TSCM, i was banned ages ago but LINK, YOU ROCK!  
