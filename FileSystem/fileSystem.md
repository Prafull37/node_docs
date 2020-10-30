# File System

To use the file system we have to ***import fs*** 
``` javascript
const fs=require('fs');
```

Before starting we will grab some knowledge about ***FILE SYSTEM FLAGS***.

### FILE SYSTEM FLAGS

#### Appending

Flag | Appending | Reading | Create File(if path not exists) | Fails/Exception(if path exists) | open in Synchronous mode
-----|-----------|---------|---------------------------------| ----------------------|--------------------------
```a```|Yes|-|Yes|-|-
```ax```|Yes|-|-|Yes|-
```a+```|Yes|Yes|Yes|-
```ax+```|Yes|Yes|-|Yes|-
```as```|Yes|-|Yes|-|Yes
```as```|Yes|Yes|Yes|-|Yes

#### Reading
Flag | Reading | Writting | Create File(if path not exists) | Fails/Exception(if path does not exists) | open in Synchronous mode
-----|-----------|---------|---------------------------------| ----------------------|--------------------------
```r```|Yes|-|-|Yes|-
```r+```|Yes|Yes|-|Yes|-
```rs+```|Yes|Yes|-|-|Yes

#### Writting
Flag | Writting |  Reading| Create File(if path not exists) | Fails/Exception(if path exists) | Truncate(if file exists)
-----|-----------|---------|---------------------------------| ----------------------|--------------------------
```w```|Yes|-|Yes|-|Yes
```wx```|Yes|-|-|Yes|-
```w+```|Yes|Yes|Yes|-|Yes
```wx+```|Yes|Yes|-|Yes|-
