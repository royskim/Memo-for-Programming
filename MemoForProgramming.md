# Xcode tips

###Really Clean

Instead of manually deleting the DerivedData folder, get Xcode to do it.

Hold down the option key, pull down the Product menu, and choose Clean Build Folder…

Normally that menu item is Clean…, but with the option key it’s really clean.

Keyboard shortcut: option-shift-cmd-K.

### Callers

In that bar right above the source code, at top left, is a little icon made up of four rectangles. Click it to pull down a menu that includes a Callers submenu.

Put the cursor on any method name. Pull down the menu and see where it gets called.

(Note, however, that it won’t detect performWithSelector-style calls. So the Callers submenu could miss instances.)

###The Find pasteboard

To search for some text, select it and hit cmd-E. The text will then appear in the find and search text fields.

No need to select the text, copy it, and then paste it into a text field.


# CocoaPods Trouble Shooting

## Fail to build

>diff: /../Podfile.lock: No such file or directory
diff: Manifest.lock: No such file or directory error: 
The sandbox is not in sync with the Podfile.lock. Run 'pod install' or update your CocoaPods installation.`

### Summary : 
Delete projectName.xcworkspace and install pods again using below command;

```
$ pod install
```

### Reference
[http://stackoverflow.com/questions/17072396/cocoapods-errors-on-project-build](http://stackoverflow.com/questions/17072396/cocoapods-errors-on-project-build)

## Predefined Comments
- #pragma mark
- #pragma mark -
- MARK:
- TODO:
- FIXME:
- !!!:
- ???:

```objc
//TODO: Some comments
```
