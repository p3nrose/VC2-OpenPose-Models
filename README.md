# VC2-OpenPose-Models

OpenPose is a real-time multi-person keypoint detection library that estimates keypoints for the body, face, hands, and feet.

## Notice
The `models/getBaseModels.bat` script is currently non-functional due to server downtime. You can download the pre-trained models and manually copy them to the appropriate folder.

## Compatibility
This has been tested with OpenPose v1.7.0. Here are the recommended downloads based on your system configuration:

- **CPU-only (suitable for laptops):**
  [Download](https://github.com/CMU-Perceptual-Computing-Lab/openpose/releases/download/v1.7.0/openpose-1.7.0-binaries-win64-cpu-python3.7-flir-3d.zip)
- **CUDA-compatible devices:**
  [Download](https://github.com/CMU-Perceptual-Computing-Lab/openpose/releases/download/v1.7.0/openpose-1.7.0-binaries-win64-gpu-python3.7-flir-3d_recommended.zip)

If you encounter any issues with this version, consider using the latest version available:
[Latest OpenPose Releases](https://github.com/CMU-Perceptual-Computing-Lab/openpose/releases)

## Additional Resources
In the OpenPose folder, refer to the `Instructions.txt` file for more information and guides.

The [Quick Start Guide](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/8ca5c1d95a42340b323e9273654d1db98bec779c/doc/quick_start.md) is a good place to begin.

## Quick Start

### Ubuntu and Mac
```bash
./build/examples/openpose/openpose.bin --video examples/media/video.avi
```
#### With face and hands
```bash
./build/examples/openpose/openpose.bin --video examples/media/video.avi --face --hand
```

### Windows - Portable Demo
```bash
bin\OpenPoseDemo.exe --video examples\media\video.avi
```
#### With face and hands
```bash
bin\OpenPoseDemo.exe --video examples\media\video.avi --face --hand
```

### Running on Webcam
Simply run the binary or executable without the `--video` or `--image_dir` parameters.
