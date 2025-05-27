# AI Virtual Mouse Using Hand Gesture

This project implements a virtual mouse system using hand gesture recognition. Using computer vision and artificial intelligence, users can control the mouse pointer and perform mouse clicks with hand gestures, without the need for a physical mouse.

## Features

- Control mouse cursor with hand movements
- Recognize gestures to perform left click, right click, and drag
- Supports both bare hand and gloved hand tracking
- Real-time webcam feed with gesture overlay

## Project Structure

```
AI-VIRTUAL-MOUSE-USING-HAND-GESTURE-main/
├── app.py                         # Main script to launch virtual mouse
├── Gesture_Controller.py          # Handles hand gesture recognition (bare hand)
├── Gesture_Controller_Gloved.py   # Gesture recognition for gloved hands
├── Proton.py                      # Helper functions
├── requirements.txt               # List of Python dependencies
├── LICENSE                        # MIT License file
├── CODE_OF_CONDUCT.md             # Code of conduct for contributors
├── .gitignore                     # Git ignored files
```

## Requirements

Install the required packages with:

```bash
pip install -r requirements.txt
```

Key Python libraries:

- OpenCV (`cv2`)
- Mediapipe
- PyAutoGUI
- NumPy

## How to Run

1. Make sure your webcam is connected and working.
2. Run the main application script:

```bash
python app.py
```

3. A window will appear with the webcam feed. Use your hand gestures to control the mouse.

## Gesture Controls

- **Move Cursor**: Move your index finger in front of the camera
- **Left Click**: Touch thumb and index fingertips together
- **Right Click**: Touch index and middle fingertips together
- **Drag**: Pinch gesture and move hand

*Note:* These gestures may vary slightly depending on the implementation in `Gesture_Controller.py`.

## Tips

- Ensure proper lighting for better accuracy
- Keep background simple to avoid detection errors
- Use `Gesture_Controller_Gloved.py` if using colored gloves for better hand detection

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributors

- Original Author(s): *[Placeholder - Add Names Here]*

## Acknowledgments

- Mediapipe for hand tracking
- OpenCV for computer vision tools
- PyAutoGUI for simulating mouse actions