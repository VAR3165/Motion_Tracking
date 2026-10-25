# Motion Tracking

A Python-based motion detection system that monitors video footage or a live camera feed and triggers an audible beep when movement is detected.

## Features

- Detects motion in video frames using OpenCV.
- Supports real-time camera input(Can use IP webcam)
- Triggers an audible alarm when motion is detected.
- Uses Python threading to manage the alarm.

## Technologies Used

- Python
- OpenCV
- NumPy
- `threading`
- `winsound` (Windows only)

## Project Structure

```text
Motion_Tracking/
├── Motion_Tracking.py
├── README.md
├── LICENSE
└── requirements.txt
```

## Installation

1. Clone the repository:

   ```bash
   git clone <YOUR_REPOSITORY_URL>
   cd Motion_Tracking
   ```

2. Create and activate a virtual environment (optional but recommended).

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the main Python script:

```bash
python Motion_Tracking.py
```

Ensure your camera is connected and accessible if you're using a live camera feed.

## How It Works

1. Captures frames from a camera or video source.
2. Converts frames to grayscale.
3. Compares frames to identify movement.
4. Activates the alarm when motion is detected.

## Limitations

- The `winsound` module is Windows-specific.
- Detection accuracy depends on lighting, camera movement, and the chosen detection threshold.

## Future Improvements

- Add adjustable motion sensitivity.
- Reduce false detections caused by lighting changes.
- Add motion tracking visualizations.
- Support configurable alarm settings.

## License

See the [LICENSE](LICENSE) file for licensing information.