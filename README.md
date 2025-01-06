# Django Sign Language to Text Converter

## Overview
The Django Sign Language to Text Converter is a web application that translates sign language gestures into readable text. It leverages machine learning models for gesture recognition and provides an intuitive interface for real-time or uploaded video processing.

## Features
- **Real-time Gesture Recognition**: Translates live sign language gestures into text using a webcam.
- **Video Upload Support**: Converts pre-recorded videos of sign language gestures into text.
- **History Tracking**: Allows users to save and view their past translations.

## Requirements

### Software Requirements
- **Python**: 3.8+
- **Django**: 4.0+
- **OpenCV**: 4.5+
- **TensorFlow/Keras**: 2.0+
- **Other Dependencies**: Listed in `requirements.txt`

### Hardware Requirements
- **Webcam**: For real-time gesture recognition.
- **GPU (Optional)**: For faster model inference.

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/django-sign-language-text-converter.git
   cd django-sign-language-text-converter
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```
   Access the application at `http://127.0.0.1:8000`.

## Usage
1. **Real-time Translation**:
   - Navigate to the "Real-time Translation" page and allow access to your webcam.
   - Perform sign language gestures in front of the camera to see the corresponding text in real time.

2. **Video Upload**:
   - Go to the "Upload Video" page and upload a video file.
   - The application will process the video and display the translated text.

3. **View Translation History**:
   - Access the "History" page to see your past translations.

## Project Structure
```
project/
├── app/                # Main Django app
├── static/             # Static files (CSS, JS, images)
├── templates/          # HTML templates
├── media/              # Uploaded files (e.g., videos)
├── models/             # Pre-trained ML models
├── requirements.txt    # Dependencies
└── manage.py           # Django management script
```

## Key Components
- **Machine Learning Models**: Pre-trained models for gesture recognition are stored in the `models/` directory.
- **Real-time Processing**: OpenCV is used to capture video frames and preprocess them for model inference.
- **User Interface**: Built with Django templates and Bootstrap for responsive design.


## Contributing
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit changes: `git commit -m 'Add feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.



## Acknowledgments
- TensorFlow for model training and inference.
- OpenCV for video processing.
- Bootstrap for responsive UI design.

## Contact
For questions or support, contact [Ujwal] at [ujwalsai16@gmail.com].

