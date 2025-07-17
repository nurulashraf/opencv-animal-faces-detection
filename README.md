# Detecting Animal Faces using OpenCV

A simple project using OpenCV to detect animal faces in images and videos.  
This repo includes basic Haar Cascade XML files and Python scripts to detect specific animal faces or experiment with custom ones.

---

## Project Structure

- **`cascades/`**: Haar Cascade XML files for animal face detection.
- **`notebooks/`**: Jupyter notebooks for data analysis, feature engineering, and model building.
- **`requirements.txt`**: List of required Python packages
- **`LICENSE`**: MIT License file
- **`README.md`**: Project overview and usage instructions.

---

## Features

- Detect cat faces using pre-trained Haar Cascade files.
- Easily swap or add other cascade files to detect other animals.
- Works on static images and video streams.
- Simple and beginner-friendly OpenCV scripts.

---

## Tools & Libraries

- **Python 3.x**
- **OpenCV** (`cv2`)

Install dependencies with:
```bash
pip install -r requirements.txt
````

---

## How to Use

1. **Clone the repo**

   ```bash
   git clone https://github.com/nurulashraf/opencv-animal-faces-detection.git
   cd opencv-animal-faces-detection
   ```

2. **Install requirements**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run detection on an image**

   ```bash
   python detect_image.py --image images/sample.jpg --cascade cascades/haarcascade_frontalcatface.xml
   ```

4. **Run detection on a video**

   ```bash
   python detect_video.py --video videos/sample.mp4 --cascade cascades/haarcascade_frontalcatface.xml
   ```

   Or use your webcam:

   ```bash
   python detect_video.py --cascade cascades/haarcascade_frontalcatface.xml
   ```

5. **Add your own cascades**

   * Download or train other Haar Cascade XML files.
   * Place them in the `cascades/` folder.
   * Update the `--cascade` argument when running the script.

---

## License

This project is licensed under the [MIT License](LICENSE).
