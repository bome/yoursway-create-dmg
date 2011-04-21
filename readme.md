#Creating dmg

This is a small utility design to automatize creation of `.dmg` files for software redistribution on mac using only command line and configuration files. It usses bash and applescript in the background.

## Supported Parameter ##

dmg files on mac are highly customizable, for know not all options are supported but you can set the following for your image

 * Volume Name
 * Window size
 * Window position 
 * Window background
 * Icons size 
 * Icons position

## Example ##
you can refere to the `.sample file`

```bash
./create-dmg   \
	--icon-size 96  \
	--window-pos 413 295  \
	--window-size 770 367  \
	--icon Applications 527 187   \
	--volname "Songbook Client v0.x"   \
	--icon "Songbook-Client.app" 201 187  \
	--background ~/songbook-client/macos_specific/Sbc/.bg/background.png  \
	test2.dmg ~/songbook-client/build/ 
```
