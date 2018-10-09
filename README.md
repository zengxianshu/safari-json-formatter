# JSON Formatter

A Safari extension which makes valid JSON documents human-readable.

### Before:
![Before][i1]
### After:
![After][i2]

## Installation
[Download the extension][1] and open it with Safari 5.

### Usage
Once installed, load any valid JSON document. [This project's most recent
commit][2] makes a good example.

#### Version History

### 1.1
* Added folding of arrays, objects and long strings
* Added setting for auto-folding of long strings (default: on)
* Added setting for "long string" threshold (default 512 bytes)
* Added a "toggle formatting" button to switch between formatted and original JSON
* Bug Fixes

#### Caveats
The extension aims to produce the same JSON string that's been loaded as input,
but because the original JSON has actually been parsed, some transformation may
occur. In other words, the formatted JSON will always be equivalent to the
original JSON, but in rare circumstances it may not match exactly. The only
known example of this is kind of discrepancy is between number formats -- if the
original JSON contains the numeric value 1e2, for example, the formatted JSON
will display the value 100.

[1]: http://github.com/rfletcher/safari-json-formatter/downloads
[2]: http://github.com/rfletcher/safari-json-formatter/commit/HEAD.json
[i1]: https://github.com/rfletcher/safari-json-formatter/raw/HEAD/etc/images/before.png
[i2]: https://github.com/rfletcher/safari-json-formatter/raw/HEAD/etc/images/after.png

#### 给Safari安装第三方扩展
起因
某天在用Safari的时候想用Markdown-Here这个插件，但是下载之后发现不能像Chrome那样直接拖放进浏览器实现安装。于是网上搜了一下——都是在说怎么在Safari自带的扩展商店下载和安装插件，对于不在商店里的插件则没有人说怎么办？官方扩展商店还用你教？
怎么办呢？在V2EX上有一个帖子，我顺着他的思路做好了，想着肯定会有别人也遇到这样的问题，索性把过程写下来，方便其他和我一样的小白用户。本操作指南是在 Safari 版本 9.1.1 (11601.6.17)环境下进行的。
教程
1. 点开偏好设置，勾选在菜单栏中显示”开发“菜单。
2. 点击开发菜单，进入”显示扩展创建器“选项。
3. 把下载的后缀为safariextz的文件解压缩，在”显示扩展创建器“页面点击”添加扩展“，找到并选中解压缩的文件夹。
4. 点击右上角的”安装“，会弹出一个提示，点击安装，会继续弹出一个权限窗口，输入本机用户的密码，即可完成该插件的安装。
