# License Plate Reader Project

## Overview
This project is designed to process vehicle license plate images, extract the license number using an image recognition API, and fetch detailed vehicle information from the national vehicle office in Israel.

---

## Workflow

### 1. **Image Input**
- Users upload an image of a vehicle license plate through the web app.

### 2. **License Plate Recognition**
- The app processes the image using an external API (e.g., OpenCV, AWS Rekognition, or a dedicated license plate recognition service).
- Recognized license number is extracted.

### 3. **Data Retrieval**
- The app sends a request to the national vehicle office API with the extracted license number.
- Returns details like:
  - Vehicle make and model
  - Year of manufacture
  - Owner's information (if authorized).

---

## Features
- **Upload Image**: Accepts license plate images in common formats (e.g., JPG, PNG).
- **License Plate Recognition**: Automatically extracts the license number from images.
- **Vehicle Information Retrieval**: Integrates with the vehicle office's API for vehicle data.

---

## Technologies
- **Frontend**: React.js
- **Backend**: Python (Flask or FastAPI)
- **Database**: PostgreSQL (if required for storing logs or user information).
- **API Integration**: License plate recognition API + national vehicle office API.

---

## Why Python for the Backend?
Python is an excellent choice for this project due to:
1. **Image Processing Capabilities**:
   - Python has libraries like OpenCV, TensorFlow, and PIL, which are well-suited for processing and analyzing images, including license plate recognition.
   
2. **API Integration**:
   - Flask and FastAPI provide simple, fast, and scalable frameworks for building APIs that integrate with third-party services.

3. **Ease of Development**:
   - Python's simplicity allows for quick development, testing, and debugging, especially useful when working with image recognition and HTTP requests.

4. **Community Support**:
   - Python has a large community and abundant resources, making it easier to find solutions for potential issues in the project.

5. **Compatibility with ML/AI Tools**:
   - If the project evolves to include machine learning for plate recognition, Python's ecosystem is ideal for integrating such models.

---

## Next Steps
1. **Research**: 
   - Gerard will explore license plate recognition APIs (e.g., OpenALPR, Google Vision).
2. **Setup**:
   - Itamar will build the basic web app structure using React.
3. **Weekly Meetings**:
   - Plan discussions to track progress and resolve blockers.
4. **API Connection**:
   - Integrate the vehicle office's API for data retrieval.

---

## Contributions
- **Itamar**: Lead frontend development, project coordination, and UI design.
- **Gerard**: Backend development, API research, and server setup.

---

## Getting Started

### 1. Clone the repository
   ```bash
   git clone <repository-url>
   ```

### 2. Install dependencies

#### For Frontend (React):
   ```bash
   npm install
   ```

#### For Backend (Python):
   ```bash
   pip install -r requirements.txt
   ```

### 3. Run the application

#### Start the Frontend:
   ```bash
   npm start
   ```

#### Start the Backend:
   ```bash
   python app.py
   ```

---

## Directory Structure
```plaintext
license-plate-reader/
├── backend/
│   ├── app.py         # Main Python application
│   ├── requirements.txt # Backend dependencies
├── frontend/
│   ├── src/
│   │   ├── App.js     # Main React application file
│   │   ├── components/
│   │   │   ├── UploadImage.js  # Image upload component
│   │   │   ├── PlateData.js    # Display vehicle details
├── README.md           # Project documentation
```

---

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
