# Ediky Video Editor | Phase-1 Layout

This is a minimal skeleton project for building our editor using **Qt6 + CMake**. It sets up the basic UI layout so we can extend it feature by feature.

---

## Directory structure

```
ediky-video-editor/
├─ CMakeLists.txt
├─ cmake/
│  └─ QtConfig.cmake
├─ assets/
│  └─ icons/
└─ src/
   ├─ main.cpp
   ├─ MainWindow.h
   ├─ MainWindow.cpp
   ├─ widgets/
   │  ├─ MediaBin.h
   │  ├─ MediaBin.cpp
   │  ├─ Timeline.h
   │  ├─ Timeline.cpp
   │  ├─ Inspector.h
   │  ├─ Inspector.cpp
   │  ├─ Preview.h
   │  └─ Preview.cpp
   └─ utils/
      ├─ Actions.h
      └─ Actions.cpp
```

---

## Features in this starter

* Menu bar (File, Edit, View, Help)
* Toolbar (Import, Play/Pause, Step)
* Media Bin dock (left)
* Timeline dock (bottom)
* Inspector dock (right)
* Preview area (center) with QMediaPlayer + QVideoWidget

---

## Build & Run

```bash
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build -j
./build/ediky_editor
```

On macOS, you can also open the generated `.app` bundle.

---

## Next steps

* Drag-and-drop import into Media Bin
* Double-click item to preview
* Add timeline clips model
* Basic export using FFmpeg

This project is intentionally minimal. Add features one by one to keep it manageable.