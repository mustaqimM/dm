dm.
==============================
A dark theme for [rEFInd][refurl] based on [Dream Machine][theme-author].
----
**Screenshot**
![M](https://github.com/mustaqimM/dm/blob/master/screenshot.png)

Installation
----
```
$root: cp -r ~/dm /boot/efi/EFI/refind/themes
$root: nvim + /boot/efi/EFI/refind/refind.conf # Opens nvim and puts the cursor on the last line
$root: #Append `include themes/dm/theme.conf` to `refind.conf`
```
__NOTE:__

Obviously [rEFInd][refurl] is needed to use this. Install with your package manager `refind-efi`. You many need to run `refind-install` afterwards.

If the `refind` bootloader doesn't show up on boot even after running `refind-install`. Run `efibootmgr` (to see the current boot order), then set the order so it is loaded first, for example: `efibootmgr -o 0002,0003,0001`. You may first need to clear the boot order: `efibootmgr -O` OR delete a specific entry: `efibootmgr -A 0002`

----  
Attributions
----

**Font:** [Dento font]

**Icons:** [Lightness for burg][icons] & [refind-ambience][icons2].

**Reddit:** [rEFInd Theme]

----

<h5 align="center">
	<br>
	<img width="150" src="https://i.imgur.com/hVNigO6.png" alt="awesome">
	<FIGCAPTION><center><a href="bitcoin:1JP6sFRUgrnAjci8ycTdGaVKGB4Y71nQyz">bitcoin:1JP6sFRUgrnAjci8ycTdGaVKGB4Y71nQyz</a></center></FIGCAPTION>
	<br>
	<br>
	<br>
</h5>
[icons]: http://sworiginal.deviantart.com/art/Lightness-for-burg-181461810
[icons2]: https://github.com/lukechilds/refind-ambience
[Dento font]: http://fontmeme.com/freefonts/34867/dento.font
[refurl]: http://www.rodsbooks.com/refind/
[theme-author]: https://github.com/Lindstream/dm-refind-theme
[rEFInd Theme]: https://redd.it/573bdd
