# The Daily Prophet — augmented reality on printed images

Point the phone at a printed picture and it starts playing as video, pinned to
the paper — the moving-newspaper effect from Harry Potter, built with ARKit.

This is the first version of the idea. The later, tidier iteration lives in
[`Augmented-Reality-AR-in-Education`](https://github.com/ankurxbatta/Augmented-Reality-AR-in-Education).

## How it works

ARKit image tracking recognises a known picture in the camera feed, reports
where it sits in 3D space, and the app overlays a video node on that exact
plane. The clip stays locked to the page as the phone moves.

## Repository layout

```
The Daily Prophet/
  ViewController.swift    AR session, image detection, video playback
  AppDelegate.swift
  harrypotter.mp4
Assets/                   reference images and the clips they map to
The Daily Prophet.xcodeproj
```

## Running it

Open the Xcode project and run on a **physical iOS device** — ARKit needs a real
camera. Show the app one of the images in `Assets/` and the matching video
plays over it.

## Built with

Swift, ARKit and SceneKit.
