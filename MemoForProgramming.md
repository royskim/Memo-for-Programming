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

