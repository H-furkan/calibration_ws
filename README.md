# calibration_ws

Calibration workspace for multisensor systems: Stereo Camera, Event Camera, LIDAR, IMU

## Project Structure

```
calibration_ws/
├── data/                # Calibration datasets (rosbags, images, pointclouds)
├── scripts/             # Calibration scripts & utilities
├── configs/             # Config files for calibration tools
├── results/             # Output (calibration parameters, plots, logs)
└── README.md            # Project documentation
```

## Overview

This workspace provides tools, scripts, and documentation to calibrate and synchronize multiple sensor modalities in robotics and computer vision applications. It is designed to help users align sensor frames and timestamps for accurate sensor fusion.

### Supported sensors

- Stereo Camera
- Event Camera
- LIDAR
- IMU

## Directory Details

- **data/**: Store your calibration datasets here. Supported formats include ROS bag files (`.bag`), images, and pointcloud data (`.pcd`, `.ply`).
- **scripts/**: Contains calibration routines, utilities, and helper scripts (Python, bash, or ROS launch files).
- **configs/**: Configuration files for each sensor or calibration tool. Example: YAML files for ROS nodes, camera intrinsics/extrinsics.
- **results/**: After running calibration, find output files here: transformation matrices, calibration parameters, plots, diagnostic logs.
- **README.md**: You’re reading it! Documentation and usage instructions.

## Getting Started

1. **Clone repository**
   ```bash
   git clone https://github.com/H-furkan/calibration_ws.git
   cd calibration_ws
   ```
2. **Prepare your data**
   - Place sensor recordings and calibration targets in `data/`.
3. **Edit configs**
   - Update configuration files in `configs/` to match your sensor setup.
4. **Run calibration**
   - Use scripts from `scripts/` to perform calibration.
5. **Check results**
   - Find calibration outputs in `results/`.

## Results

- Calibration parameters (extrinsics, intrinsics)
- Plots of calibration accuracy
- Log files for diagnostics
- Example output files available in `results/`

## To Do

- [ ] Add sample calibration datasets to `data/`
- [ ] Provide example configuration files for common hardware
- [ ] Document recommended calibration targets and procedures
- [ ] Add visualization scripts for results
- [ ] Integrate additional sensor types (e.g., GNSS, thermal cameras)
- [ ] Expand troubleshooting and FAQ section

## References

- [ROS Calibration Toolbox](http://wiki.ros.org/camera_calibration)
- [Kalibr: IMU-Camera Calibration](https://github.com/ethz-asl/kalibr)
- [LIDAR-Camera Calibration](https://github.com/ankitdhall/lidar_camera_calibration)
- [Event Camera Calibration Resources](https://rpg.ifi.uzh.ch/docs/EventCameraCalibration.pdf)
- [Sensor Fusion and Calibration Survey](https://www.mdpi.com/1424-8220/20/3/713)
- [Stereo Camera Calibration (OpenCV)](https://docs.opencv.org/master/d9/d0c/group__calib3d.html)

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## Contact

For questions, issues, or contributions, please open an issue or contact [@H-furkan](https://github.com/H-furkan).
