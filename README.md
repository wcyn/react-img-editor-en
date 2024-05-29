# react-img-editor-en Image Editor

![](https://img.shields.io/npm/v/react-img-editor-en.svg) ![](https://img.shields.io/npm/dw/react-img-editor-en.svg)

react-img-editor-en is an image editor react component that supports cropping, graffiti, text editing, mosaic processing and other operations on images. It also supports custom plug-ins and flexible style configuration.

![Example](https://s2.ax1x.com/2020/02/16/39gZcD.png)

## ✨ Features

- Supports free brush, rectangle, circle, arrow, text, mosaic drawing
- Support eraser, undo operation, screenshot and image download
- Support custom plugins and toolbar configuration
- Support stretching, dragging and deleting of rectangles, circles, arrows, text and other nodes
- Support multiple components on the same page

## 📦 Download

```
npm install react-img-editor-en -S
```

## 🔨 Import and use

```
import ReactImgEditor from 'react-img-editor-en'
import 'react-img-editor-en/assets/index.css'

<ReactImgEditor src="https://www.w3schools.com/html/img_girl.jpg" />
```

## 🧰 API

| Property          | Description                                                                                                                             | Type                 | Default Value                                                            |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------- | -------------------- | ------------------------------------------------------------------------ |
| src               | image url                                                                                                                               | string               | -                                                                        |
| width             | Artboard width                                                                                                                          | number?              | 700                                                                      |
| height            | Artboard height                                                                                                                         | number?              | 500                                                                      |
| style             | Artboard style                                                                                                                          | React.CSSProperties  | -                                                                        |
| plugins           | Custom plugins                                                                                                                          | Plugin[]             | []                                                                       |
| toolbar           | Toolbar configuration                                                                                                                   | { items: string[] }  | {items: ['pen', 'eraser', 'arrow', 'rect', 'circle', 'mosaic', 'text', ' | ', 'repeal', 'download', 'crop']} |
| getStage          | Get KonvaJS's [Stage](https://konvajs.org/api/Konva.Stage.html) object, which can be used for downloading pictures and other operations | (stage: any) => void |
| defaultPluginName | Default selected plugin name                                                                                                            | string?              | -                                                                        |
| crossOrigin       | Handle cross-origin images                                                                                                              | string?              | -                                                                        |

## 📝 ALL

- [ ] Dynamically load images
- [ ] Download image type configuration
- [ ] Provide plugin configuration item configuration
- [ ] Optimize the free brush writing experience
- [ ] Internationalization support

## 🤝 Contributions

Development

```
npm run start
```

http://127.0.0.1:8012/examples/simple.html

release

```
npm run lint
npm run pub
```
