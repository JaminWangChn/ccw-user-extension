[TOC]
# What for
This repo is for CCW Creator who wants make and test their own extension.
# How to jump in
There are two ways to develop and test your extension
## Normal remote extension (for anyone)
You can build your blocks and test it, you can use all javascript capacity to do what you want, there only have one limit that normal remote extension will be running in a sandbox and unable to access vm or runtime utility.
## CCW approved extension (for CCW collaborator)
Become CCW collaborator then your can push code into this repo. extensions in this repo will have full access to vm and runtime allow you build highly functional block for all CCW Creator.
When your complete testing,you can apply publish extension to CCW Extension Library, and all CCW Creator can use it in their project.
## Apply for CCW collaborator
// TODO email address
// TODO apply form
# How to develop 

## Define a extension
### normal remote extension
checkout example file [.example/normal-ext.js](https://github.com/CCW-Site/ccw-user-extension/blob/main/example/normal-ext.js)

### CCW approved extension
checkout example file [.example/ccw-approved-ext.js](https://github.com/CCW-Site/ccw-user-extension/blob/main/example/ccw-approved-ext.js)
## Test your extension
### normal remote extension
if your work on a normal remote extension, you can upload your extension js file to any http server and make sure it can be accessed in open network.

when complete above moves, use below url in browser(recommend Chrome)
```
https://www.ccw.site/creator?extension=${your_file_url}
```
for example
```
https://www.ccw.site/creator?extension=https://ccw-user-extension.ccw.site/example/normal-ext.js
```
extension will be added in bottom of block menu if your code has no errors.
### CCW approved extension

Commit&push code to this repo and a bot will deploy your extension to CCW test server automatically.

The automatic deploy url format is like below
```
https://ccw-user-extension.ccw.site/${your_folder}/${jsFile}
```

when complete above moves, use below url in browser(recommend Chrome)
```
https://www.ccw.site/creator?ext=https://ccw-user-extension.ccw.site/${your_folder}/${jsFile}
```
for example
```
https://www.ccw.site/creator?ext=https://ccw-user-extension.ccw.site/example/ccw-approved-ext.js
```
extension will be registed in Extension Library.you must add it by hand before you use it.
## Asset standard
extension cover
type: png/jpg/svg
size: 600 × 372 px

extension block icon
type: svg
size: 80 x 80 px

extension menu icon
type: svg
size: 80 x 80 px

