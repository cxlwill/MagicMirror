本文档为 Home Assistant 夜间模式，以适配魔镜背景。

HA 在最新版本 49.0 中推出了主题模式，但尚无法实现全局 CSS 自定义。因此本方法采用 HTML + 主题修改方法，后续随 HA 不断完善，将最终转为纯主题设置。

md5: 766d2e2ac7bfa269edf7abe30b3797a6

使用`front.html`及`front.html.gz`替换`www_static`文件夹内相同文件，同时使用` version.py`替换上层文件夹内同名文件。

**注意：文件替换直接修改了原UI，在下次更新后将失效**

在`configuaration.yaml`添加主题设置：
```
frontend:
  themes:
    night:
      dark-primary-color: black
      backgroud-color: black
      primary-background-color: black
      primary-text-color: white
      primary-color: black
      paper-card-background-color: black
      paper-listbox-background-color: black
      divider-color: black
      paper-slider-container-color: black
      text-primary-color: black
      paper-grey-200: black
      disabled-text-color: black
```




若想保持永久更新，请打开 Home Assistant 开发者模式，添加 Custom UI,详见[官方教程](https://home-assistant.io/developers/frontend_creating_custom_ui/)


