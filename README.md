# fancytext
Goal of this project is to provide a replacement for Garry's Mod RichText vgui panel which supports more scriptability and non-text elements (images etc.).

Final goal is to make it possible to only change vgui.Create("RichText") to vgui.Create("DFancyText") without editing anything else.

[A quick how-to use can be found on the wiki](https://github.com/Herover/fancytext/wiki).

## What implemented
From [the gmod wiki](http://wiki.garrysmod.com/page/Category:RichText) (strike means not implemented yet, italic means partially/not as RichText):
* AppendText
* ~~GetNumLines~~
* GotoTextEnd _seems to require more calls than RichText_
* ~~GotoTextStart~~
* ~~InsertClickableTextEnd~~
* ~~InsertClickableTextStart~~
* InsertColorChange
* ~~InsertFade~~
* ~~ResetAllFades~~
* SetFontInternal _overrideable_
* ~~SetToFullHeight~~
* _SetVerticalScrollbarEnabled_ (resets scroll)

Additionally fancytext also supports following functions
* AppendImage {w, h, mat}
* InsertFontChange fontname _SetFontInternal uses this function, you can change font at any time_
* AppendFunc fn(h) -> {w, h, panel}

Full documentation to-be-made.

## License
Contents of this repository is licensed under [GNU Lesser General Public License v3](http://www.gnu.org/licenses/lgpl-3.0.html) ([tl;dr](https://tldrlegal.com/license/gnu-lesser-general-public-license-v3-%28lgpl-3%29)).
You are allowed to use and include it in code using other licenses, commercial and free, but fancytext itself must remain under LGPL and any changes done to fancytext must be made public under LGPL.
