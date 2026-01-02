# Robotics Learning Path Curriculum

This curriculum is designed to be hands-on, starting from system setup and moving towards complex visual robotics tasks.

## Timeline & Pacing
**Pace**: 2.5 - 3 hours/week.
**Total Estimated Duration**: ~12 Weeks (3 Months).
**Adjustment**: accelerated specifically for an experienced C++/Python developer.

## Module 1: Foundation & Toolchain (1 Week)
**Goal**: Quick verification of the RPi environment and Rust setup.
*   **Week 1**: OS Config, Toolchain verification (C++ CMake/Rust Cargo), Cross-compilation test.
*   **1.1 OS Setup**: Headless setup, SSH, Network config.
*   **1.2 Development Environment**: VS Code Remote SSH, Vim/NeoVim on device.
*   **1.3 The "Hello World" Trinity**: Python, C++, and Rust (focus on Rust if new).

## Module 2: The Networked Eye (IP Camera) (3 Weeks)
**Goal**: Master video ingestion over the network (RTSP/H.265).
*   **Week 2**: **Concept Study** - Video Codecs (H.264/H.265), RTSP/RTP protocols.
*   **Week 3**: Python (OpenCV) & C++ (GStreamer/FFmpeg) implementation.
*   **Week 4**: Rust Implementation (FFI safety & crate selection).
*   **2.1 The Protocol (RTSP)**: RTSP/RTP URLs, `vlc`/`ffprobe` verification.
*   **2.2 Python Stream Ingestion**: `opencv-python` with GStreamer/FFmpeg.
*   **2.3 C++ High-Performance Decoding**: robust RTSP client using `GStreamer` or `FFmpeg`.
*   **2.4 Rust & Media**: `gstreamer-rs` or `ffmpeg-next`.

## Module 3: Visual Intelligence & Optimization (3 Weeks)
**Goal**: Process visual data efficiently.
*   **Week 5**: Latency analysis & Basic Algorithms (Motion/Color).
*   **Week 6**: Advanced: Aruco Marker math & Pose Estimation.
*   **Week 7**: Profiling & Optimization (Glass-to-Glass latency).
*   **3.1 Latency Analysis**: Measuring "Glass-to-Glass" latency. Optimizing buffers.
*   **3.2 Basic Image Processing**: Motion detection, resizing, and color space conversion.
*   **3.3 Aruco Markers**: Robust pose estimation from the decoded stream.

## Module 4: Concurrency & Real-time Systems (2 Weeks)
**Goal**: Application of system programming concepts to Robotics.
*   **Week 8**: The Main Loop & Python/C++ Concurrency patterns (applying what you know).
*   **Week 9**: Rust Concurrency (The Borrow Checker in multi-threaded contexts).
*   **4.1 The Loop**: creating a non-blocking main loop.
*   **4.2 Multithreading/Multiprocessing**:
    *   **Python**: `threading` vs `multiprocessing`.
    *   **C++**: `std::thread`, mutexes.
    *   **Rust**: Ownership transfer, Channels.
*   **4.3 Latency Analysis**: Capture -> Process -> Output analysis.

## Module 5: Introduction to modern Robotics Middleware (ROS 2) (3 Weeks)
**Goal**: Step up to professional-grade tools.
*   **Week 10**: ROS 2 Concepts, Architecture & Setup.
*   **Week 11**: Porting Camera/CV nodes to ROS 2 (Python/C++).
*   **Week 12**: Experimental Rust in ROS 2.
*   **5.1 ROS 2 Concepts**: Nodes, Topics, Publishers, Subscribers.
*   **5.2 Setup**: Installing ROS 2 (Jazzy/Humble) on RPi.
*   **5.3 Integration**: Porting our Camera/CV nodes to ROS 2.
