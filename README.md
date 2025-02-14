# MyVisualNovelTransTools
Most of them are written by AI<br/>
## AI5WINGccImageTool
To convert .png(must be 32bpp) to Ai5Win .GCC image file(Uniformly use G24m format)<br/>
## AILScriptSimpleToolPlus/AILScriptSimpleTool++
To dump/inject AIL engine Script from v1 to v3<br/>
v3: ????-2001<br/>
v2: 2002-2005<br/>
v1: 2006-????<br/>
## AoiBoxAOIMYTool
To extract/repack Aoi engine AOIMY Unicode format .box script resource Archive<br/>
when repacking pro.box, you need to manually change the index of pro.txt file to the first one in pro.box archive.<br/>
## AosCompressTool
To decompress/compress Lilim engine .scr files to achieve No-packet-read<br/>
## AZsysCompressTool
To decompress/compress AZ system engine ASB sign .asb compressed and encrypted files<br/>
You can find key in system.arc([here](https://github.com/shangjiaxuan/Crass-source/blob/4aff113b98fc39fb85f64501ab47c580df779a3d/cui/AZSystem/AZSystem.cpp) is the method) or 4 known keys in GARbro<br/>
"Clover Heart's": 3786541434<br/>
"Triptych": 501685433<br/>
"Amaenbou": 2938115999<br/>
"Reminiscence Blue": 2849404158<br/>
## AZsysCpbImageTool
To covert AZ system engine .cpb image file to bmp AND .png(must be 32bpp) to cpb file<br/>
## AZsysScriptSimpleTool
To dump/inject decompressed ASB sign .asb script files<br/>
## BGIScriptSimpleTool
To dump/inject BGI engine Script<br/>
Most likely it won't work in very old BGI version<br/>
DO NOT use it to edit config file, especially when it has messy code in the dumped txt file<br/>
## CaramelBox
A series of tools for extract/repack CaramelBox engine arc3 Archive, decompress/fake compress lze files, dump/inject scb script files<br/>
## CswareDL1ArchiveTool
To extract/repack Csware .DL1 Archive<br/>
## CVNSCpz2ArchiveTool
To pack a cpz2 Archive<br/>
have no compress AND md5_compute function in the programm<br/>
so you have to modify game.exe to jump the md5_check(track MessageBox) and decompress_function([here](https://www.bilibili.com/video/BV1cB4y1k7tF/) is the method)<br/>
## EAGLSDecryptTool
To decrypt/encrypt EAGLS .dat script files to achieve No-packet-read.<br/>
## EscudeScriptSimpleTool
Most likely it has no Universality because escude's scriptmode always changes<br/>
Tested on 放課後⇒エデュケーション！～先生とはじめる魅惑のレッスン～<br/>
## EscudeScriptSimpleToolV2
Most likely it has no Universality because escude's scriptmode always changes<br/>
Tested on 彗聖天使プリマヴェールZwei<br/>
## FlyingV3ArchiveTool
To extract/repack Flying ShineV3 .pd Archive<br/>
## FosterFA2ArchiveTool
To extract/repack Foster game engine .FA2 Archive<br/>
It will set all compression flags to 0(no compression) so the repacked archive looks like plaintext<br/>
## FrontWingPacArchiveTool
To extract/repack FrontWing engine LIB_PACKDATA0000 sign .pac(ArcFLT in GARbro) Archive<br/>
## GPK2CompressTool
To decompress/compress GPK2 .scb file to achieve No-packet-read<br/>
## IceArchiveTool
To extract/repack IceSoft .BIN Archive<br/>
## IceCompressTool
To decompress/compress(Actually just add a TPW\x00 sign) IceSoft TPW sign Script files<br/>
## LambdaLapArchiveTool
To extract/repack Lambda engine gsce.lap Archive<br/>
## LambdaLapArchiveSimpleTool && LambdaCompressTool
To extract Lambda engine gevent.lap image archive.<br/>
you need to use archivetool to extract compressed files and use compresstool to decompress files twice.
## LambdaLAXArchiveTool
To extract/repack Lambda engine .lax Archive<br/>
Uniformly use lzss fake compression to repack<br/>
## MajiroScriptSimpleTool
To dump/inject Majiro Script .mjs(decrypted by mjcrypt) file or MajiroOBJV file(need to change file-extend-name to .mjs)<br/>
To change MajiroOBJX to MajiroOBJV You can see [GalgameReverse Project](https://github.com/YuriSizuku/GalgameReverse)<br/>
Initially made to edit script in あの晴れわたる空より高く for there are tips-jump in the game and no tools can deal with it.<br/>
So it ONLY works on new_version majirov3 script<br/>
For v1 use [VNT](https://github.com/arcusmaximus/VNTranslationTools)<br/>
For v2 and old_version v3 use [MajiroTools](https://github.com/AtomCrafty/MajiroTools) or Ineditor<br/>
## MarbleMblArchiveTool
To extract/repack Marble engine mg_data(%d).mbl Archive<br/>
If the game has no key(can be correctly extracted by the default method in GARbro), keep key empty<br/>
Or you can use known keys in GARbro<br/>
![Snipaste_2025-01-30_15-13-54](https://github.com/julixian/MyVisualNovelTransTools/blob/main/images/Snipaste_2025-01-30_15-13-54.png)
You can also manually find the key in game.exe, [here](https://github.com/shangjiaxuan/Crass-source/blob/4aff113b98fc39fb85f64501ab47c580df779a3d/cui/MarbleEngine/MarbleEngine.cpp) exists the method to find key<br/>
For example:<br/>
![Snipaste_2025-01-30_14-25-37](https://github.com/julixian/MyVisualNovelTransTools/blob/main/images/Snipaste_2025-01-30_14-25-37.png)
![Snipaste_2025-01-30_15-21-02](https://github.com/julixian/MyVisualNovelTransTools/blob/main/images/Snipaste_2025-01-30_15-21-02.png)
the key of 彼女が見舞いに来ない理由 is 0x46554A4953415741 and Cafe AQUA is 0x89B482CD97598EF782BE
## MTSPakZArchiveTool
To extract/repack MTS engine .pak or .z Archive<br/>
## MyAdvArchiveTool
To extract/repack MyAdv engine .pac Archive<br/>
when packing, please limit the numbers of the files to pack or delete the config files in the dir ready to pack to prevent replacing the config file in the archive, for the config file use different zlib compress method and if they are recompressed and replace the orgi config file in the archive, game can't run.<br/>
Tested on 彼女達は脅迫に屈する, 猫mata～猫又と兄と私の話～<br/>
## OhgetsuPacArchiveTool
To extract/repack Ohgetsu engine script.pac Archive<br/>
when repacking, the programm will set the compression flag to 0(no compression) in exe<br/>
So do not compress the files back before repacking<br/>
You can also use crass to unpack the archive(using special parameter 『exe="path/to/your/game.exe"』, will decompress the files at the same time)<br/>
## OtemotoCompressTool
To decompress/fake compress the lzss compressed files<br/>
## OtemotoTLZArchiveTool
To extract/repack Otemoto engine .TLZ Archive<br/>
## RiddleArchiveTool
To extract/repack Riddle engine .pac Archive<br/>
## RiddleCompressTool
To decompress/compress Riddle .scp file<br/>
## RiddleScriptSimpleTool
To dump/inject Riddle .scp Script file<br/>
If there are Select jump in a script, from 0x8 it has flags like Select, CngExe and F47<br/>
And 0x24、0x44、0x64…… will store the offset<br/>
So if there are new flags, you can change the offset by hand<br/>
## TailCafArchiveTool
To extract/repack Tail engine .caf Archive<br/>
## TailScriptSimpleTool
To dump/inject Tail .scd Script file<br/>
## TopCatCompressTool
To decompress/compress TopCat engine .TCT Script file<br/>
apply for both v2 and v3<br/>
## TopCatV2ArchiveTool
To extract/repack TopCatV2 .TCD Archive<br/>
## TopCatV3ArchiveTool
To extract/repack TopCatV3 .TCD Archive<br/>
## YaneuraoDatArchiveTool
To extract/repack Yaneurao engine .dat Archive<br/>
## YaneuraoYgaImageTool
To convert .yga image to bmp AND .bmp to yga(no compress) image<br/>
If want to edit the image, convert the image to png first. And before converting to yga, convert the png back to bmp and then convert to yga.<br/>
Or the image will lose Transparent pixel.<br/>
