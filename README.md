<p align="center">
  <img src="icon_text.png" height=100>
</p>

## <div align="center"><b><a href="README.md">English</a> | <a href="README_CN.md">简体中文</a></b></div>

<div align="center">

[![download](https://img.shields.io/github/downloads/xinntao/HandyView/total)](https://github.com/xinntao/HandyView/releases)
![visitors](https://visitor-badge.glitch.me/badge?page_id=xinntao/HandyView)
[![PyPI](https://img.shields.io/pypi/v/handyview)](https://pypi.org/project/handyview/)
[![license](https://img.shields.io/github/license/xinntao/HandyView)](https://github.com/xinntao/HandyView/blob/master/LICENSE)
[![python lint](https://github.com/xinntao/HandyView/actions/workflows/pylint.yml/badge.svg)](https://github.com/xinntao/HandyView/blob/master/.github/workflows/pylint.yml)
[![Publish-pip](https://github.com/xinntao/HandyView/actions/workflows/publish-pip.yml/badge.svg)](https://github.com/xinntao/HandyView/blob/master/.github/workflows/publish-pip.yml)
[![Release](https://github.com/xinntao/HandyView/actions/workflows/release.yml/badge.svg)](https://github.com/xinntao/HandyView/blob/master/.github/workflows/release.yml)

 </div>

<div align="center">

  🔻[**Executable files**](https://github.com/xinntao/HandyView/releases) **|** 🔧[**Installation**](#-Installation)  **|** 📕[**使用说明**](docs)
 </div>

HandyView is a **handy image viewer** for convenient viewing and comparing. It is developed with PyQt5.

---

```Handy``` *Series*: &emsp;&emsp;
<img src="https://github.com/xinntao/HandyView/blob/master/icon.png" alt="HandyView Icon" width="36" height="36"> [HandyView](https://github.com/xinntao/HandyView) &emsp; <img src="https://github.com/xinntao/HandyFigure/blob/master/icon.png" alt="HandyFigure Icon" width="36" height="36"> [HandyFigure](https://github.com/xinntao/HandyFigure) &emsp; <img src="https://github.com/xinntao/HandyCrawler/blob/master/icon.png" alt="HandyCrawler Icon" width="36" height="36"> [HandyCrawler](https://github.com/xinntao/HandyCrawler)
&emsp; <img src="https://github.com/xinntao/HandyWriting/blob/master/icon.png" alt="HandyWriting Icon" width="36" height="36"> [HandyWriting](https://github.com/xinntao/HandyWriting)


## 🔧 Installation

### <img src="https://upload.wikimedia.org/wikipedia/commons/8/8d/Windows_darkblue_2012.svg" alt="Windows" height="28">

1. Download the pre-compiled executable zip file from the release page ([Github](https://github.com/xinntao/HandyView/releases).
2. Unzip the file
3. Set HandyView as the default image viewer, so that you can **double-click the image to open** HandyView.

### <img src="https://user-images.githubusercontent.com/11482921/171234862-5a54e430-7c07-4976-9ac8-ce8dbf520a17.png" alt="MacOS" height="24">

1. Download the handyviewer.dmg from the release page ([Github](https://github.com/xinntao/HandyView/releases) and install.
2. If you fail to install the app, you may first need to [disable gatekeeper](https://disable-gatekeeper.github.io/) first. You should be aware of the risk of [disabling gatekeeper](https://disable-gatekeeper.github.io/).
3. Set HandyView as the default image viewer (use `cmd+i`), so that you can **double-click the image to open** HandyView.

### <img src="https://upload.wikimedia.org/wikipedia/commons/3/3a/Logo-ubuntu_no%28r%29-black_orange-hex.svg" alt="Ubuntu" height="24">

I used the early version of HandyView on Ubuntu. The current version is not tested on Ubuntu and may be out-of-date.

1. Clone this repo `git clone https://github.com/xinntao/HandyView.git`
1. How to double click to open an image
    1. Modify the HandyView.desktop file - *Exec & Icon*
    1. Copy the .desktop file to `/usr/share/applications`
1. How to change the default image viewer
    1. Right click an image
    1. Go to `Properties` -> `Open With`
    1. Choose *HandyView*

### <img src="https://user-images.githubusercontent.com/11482921/171239036-858e2c00-835f-4278-afb4-5b8ac3fe2b65.png" alt="Ubuntu" height="38">

For python user, you can also launch HandyView from the command line:

1. Clone repo and install dependent packages

    ```bash
    git clone https://github.com/xinntao/HandyView.git
    cd HandyView
    pip install -r requirements.txt
    ```

2. Run

    ```bash
    python -m handyview.handyviewer [image_path]
    ```

## :sparkles: Features

- Switch among images **with fixed zoom ration**, which is useful when comparing image details. (Unfortunately, I cannot find such a image viewer and this is the initial motivation to develop HandyView).
- Various comparison modes.
- Show basic image information, *e.g.*, image path, shape, size, color type, zoom ration, etc.
- Show the position and color in the current mouse cursor.
- Draw rectangles on images and show the start and end position.

## :eyes: Screenshot

- Current screenshot

<p align="center">
  <img src="assets/screenshot.png" height="400">
</p>

- Switch among images with **fixed zoom ratio**

<p align="center">
  <img src="assets/hv_switch.gif" height="400">
</p>

- Compare images in two-column or three-column modes

<p align="center">
  <img src="assets/hv_cmp.gif" height="400">
</p>

- Show the position and color of the current mouse cursor

<p align="center">
  <img src="assets/hv_mousemove.gif" height="400">
</p>

- Draw rectangles and show the start and end positions

<p align="center">
  <img src="assets/hv_rect.gif" height="400">
</p>

## Compile to executable program

For Windows and MacOS users, you can find the instructions of compiling the executable program from [how-to-build](how_to_build.md).

## :book: Document (On the way)

The basic operation (such as shortcut keys) could be found in the *Help* button in the toolbar.

## :hourglass_flowing_sand: TODO list

- [ ] preview mode
- [ ] show zoom info for each folder (store in database)
- [ ] drag together in the multi-view comparison mode

### Editing operation

- [ ] Simple image edit: crop, resize, color conversion, etc
- [ ] Draw rectangular and enlarged the area
- [ ] Make GIF easily

## :books: References

- [Qt5 doc](https://doc.qt.io/qt-5/)
- [PyQt5 doc](https://doc.qt.io/qtforpython/api.html)
- [Qt Key](https://doc.qt.io/archives/qtjambi-4.5.2_01/com/trolltech/qt/core/Qt.Key.html)

## :scroll: License and Acknowledgement

This project is released under the [MIT license](./LICENSE).

### Icons

I have used the icons from [flaticon](www.flaticon.com). The following are the source links.

| Icon | Link | Icon | Link | Icon |Link|
| :--- | :---:        |     :---      | :---: | :---        |     :---:      |
| <img src="icons/open.png" height="32" alt="Open">  | [Open](https://www.flaticon.com/free-icon/open_3143203?term=file%20open&page=1&position=1) | <img src="icons/history.png" height="32" alt="History">|[History](https://www.flaticon.com/free-icon/timer_2921268) | <img src="icons/refresh.png" height="32" alt="Refresh"> |[Refresh](https://www.flaticon.com/free-icon/reuse_3299869?term=refresh&page=1&position=16) |
| <img src="icons/index.png" height="32" alt="Index">  | [Index](https://www.flaticon.com/free-icon/index_2807595?term=index&page=1&position=8) | <img src="icons/include.png" height="32" alt="Include"> |[Include](https://www.flaticon.com/free-icon/add_2921226) | <img src="icons/exclude.png" height="32" alt="Exclude">|[Exclude](https://www.flaticon.com/free-icon/remove_2921203) |
| <img src="icons/compare.png" height="32" alt="Compare">  | [Compare](https://www.flaticon.com/free-icon/file_748614?term=compare&page=1&position=17) | <img src="icons/clear_comparison.png" height="32" alt="Clear comparison"> |[Clear comparison](https://www.flaticon.com/free-icon/eraser_3277337?term=clear&page=1&position=5) |<img src="icons/instructions.png" height="32" alt="Help">  |[Help](https://www.flaticon.com/free-icon/information-point_4231321?term=help&page=1&position=87&page=1&position=87)|
| <img src="icons/main_canvas.png" height="32" alt="Main canvas">  | [Main canvas](https://www.flaticon.com/free-icon/image_3603103) | <img src="icons/compare_canvas.png" height="32" alt="Compare canvas"> |[Compare canvas](https://www.flaticon.com/free-icon/portraits_3603402) |  <img src="icons/preview_canvas.png" height="32" alt="Preview canvas">  |[Preview canvas](https://www.flaticon.com/free-icon/pieces_3603403)|
| <img src="icons/fingerprint.png" height="32" alt="Fingerprint">  | [Fingerprint](https://www.flaticon.com/free-icon/fingerprint_2313448?term=fingerprint&page=1&position=7) | <img src="icons/auto_zoom.png" height="32" alt="auto zoom"> | [Auto Zoom](https://www.flaticon.com/premium-icon/target_4723850?term=target%20lens&page=1&position=5&page=1&position=5&related_id=4723850&origin=search)  |  | |

(pip install pyqt5 -i <http://mirrors.xxx.com/pypi/simple/> --trusted-host mirrors.xxx.com)

## :e-mail: Contact

If you have any question, please open an issue or email `xintao.wang@outlook.com`.
