# PigaScribe API Foundation

This repository contains the foundational implementation of the PigaScribe API, built using FastAPI. The API provides a basic structure to manage audio recordings, file uploads, transcription, and interaction with external services like Fabric for meeting report generation.

## Features

- **Start/Stop Recording**: Placeholder endpoints to simulate starting and stopping audio recording.
- **File Upload**: Upload audio files to the server for processing.
- **Transcription**: Simulated transcription endpoint for converting audio files into text.
- **Fabric Integration**: Placeholder endpoint to process transcriptions with Fabric and retrieve meeting reports.
- **File Management**:
  - List all uploaded files.
  - Delete specific files from the server.

## Technologies Used

- **Backend Framework**: [FastAPI](https://fastapi.tiangolo.com/)
- **Language**: Python 3.9+
- **Server**: Uvicorn (ASGI server)

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/pigascribe-api.git
   cd pigascribe-api
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install fastapi uvicorn
   ```

4. Run the server:
   ```bash
   uvicorn main:app --reload
   ```

5. Access the API:
   - Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
   - ReDoc: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

## Endpoints

### Recording
- `POST /record/start` - Start recording (simulated).
- `POST /record/stop` - Stop recording (simulated).

### File Management
- `POST /upload` - Upload an audio file.
- `GET /files` - List all uploaded files.
- `DELETE /files/{file_name}` - Delete a specific file.

### Transcription
- `POST /transcribe` - Simulate transcription of an uploaded audio file.

### Fabric Integration
- `POST /fabric` - Simulate processing transcription with Fabric.

## Directory Structure
```
.
├── main.py        # Main API code
├── uploads/       # Directory for uploaded files
├── README.md      # Project documentation
└── requirements.txt  # Python dependencies (optional)
```

## Next Steps

- Implement actual audio recording functionality.
- Integrate a transcription library or external API.
- Add logic to send transcription data to Fabric and process responses.
- Enhance error handling and input validation.

## Contribution

Feel free to fork this repository and submit pull requests for improvements or new features. Contributions are always welcome!

## License

This project is licensed under the MIT License. See the LICENSE file for details.
