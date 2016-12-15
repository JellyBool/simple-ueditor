## Ueditor 的简化版本

> 声明：本项目的代码来源于百度的 ueditor 项目，本人只是做了一些微小的工作。

##效果

![simple-ueditor](https://cloud.githubusercontent.com/assets/6011686/21228553/38bf2fdc-c319-11e6-9b6d-5de223bc9989.png)

## 使用
1. clone 代码
```git
git clone https://github.com/JellyBool/simple-ueditor.git
```
2.用此项目的 `ueditor` 目录替换原来的 `ueditor` 目录

3.实例化编辑器的时候配置 `toolbar` ，主要是 `toolbar` 的配置
```javascript
var ue = UE.getEditor('editor', {
    toolbars: [
            ['bold', 'italic', 'underline', 'strikethrough', 'blockquote', 'insertunorderedlist', 'insertorderedlist', 'justifyleft','justifycenter', 'justifyright',  'link', 'insertimage', 'fullscreen']
        ],
    elementPathEnabled: false,
    enableContextMenu: false,
    autoClearEmptyNode:true,
    wordCount:false,
    imagePopup:false,
    autotypeset:{ indent: true,imageBlockLine: 'center' }
});
```
