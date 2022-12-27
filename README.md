# bpy_smsk_new_link
Imports models into Blender with the extension .lzs or .bum from a mobile game called

シノビマスター 閃乱カグラ NEW LINK
(Shinobi Master Senran Kagura New Link)

The game is by Honey & Paradise Games: www.hpgames.jp/shinomas/

Request came to me from Lugana-Rysniq via the Xentax community discord:
discord.gg/zWxdRZK

The request was to fix TGE’s maxscript that was failing to import certain meshes
https://www.vg-resource.com/thread-34712.html

I took the opportunity to practice creating a recursive read function in 3dsmax’s maxscript

Part of that process can be seen in this 3hour youtube video stream here:
youtu.be/QbuwFSxtTek

Same rando dude messaged me a few times through out the years barking about script stability.
So I've ported the maxscript over to python and the blender python API, while doing a code review.

The BUM format is a rat's nest, and I truly don't know what's going on in there, but I fixed a few 
bugs from the maxscript.

Also I should mention that chrrox originally reversed engineered the BUM format before TGI, and myself.
As well chrrox created the solution with quickBMS to decompress the lzs files which the game files are packed with.
https://forum.xentax.com/viewtopic.php?f=10&t=16027

For convenience I wrote a lzs decoder in the script so that I didn't have to be dependant on quickBMS.

The lzs decoding algo was adapted from C code shared by Haruhiko Okumura for LZS (Lempel–Ziv–Stac) here:
http://justsolve.archiveteam.org/wiki/LZSS_(Haruhiko_Okumura)


- Have Fun!
