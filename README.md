# SEED-VC Voice Conversion SERVER

This project provides a server implementation for voice conversion using the SEED-VC (Style-Embedded Encoder-Decoder for Voice Conversion) model. It allows developers to convert voice samples through a simple POST request, utilizing zero-shot voice conversion capabilities.

## Features

- Zero-shot voice conversion using SEED-VC model
- RESTful API endpoint for voice conversion
- Easy-to-use interface for developers
- Support for various audio formats
- Jupyter Notebook implementation

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.8 or higher
- Jupyter Notebook
- PyTorch
- CUDA (for GPU acceleration, recommended)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/[your-username]/seed-vc-api
cd seed-vc-api
```

2. Create a virtual environment and activate it:
```bash
python -m venv venv
# For Windows
.\venv\Scripts\activate
# For Linux/Mac
source venv/bin/activate
```

3. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Start the Jupyter Notebook server:
```bash
jupyter notebook
```

2. Open the `SEED-VC-L1.ipynb` notebook

3. Run all cells to start the server

4. Upload the reference audio before starting the server

### API Endpoint

Send a POST request to convert voice:

```
POST http://localhost:[port]/convert
```

Request body should be a multipart form-data with:
- `audio_file`: The source audio file to be converted

Example using cURL:
```bash
curl -X POST -F "audio_file=@path/to/your/audio.wav" http://localhost:[port]/convert
```

## Model Details

This implementation uses the SEED-VC model for voice conversion, which offers:
- Zero-shot voice conversion capabilities
- Style embedding for maintaining speech characteristics
- High-quality voice conversion without parallel data
- Efficient processing and conversion

## Technical Details

- Model: SEED-VC (Style-Embedded Encoder-Decoder for Voice Conversion)
- Conversion Method: Zero-shot
- Framework: PyTorch
- Server: Implemented in Jupyter Notebook with REST API endpoint


## Acknowledgments

- SEED-VC model developers and researchers - acces their repository[https://github.com/Plachtaa/seed-vc]
- all the credits should go to the original developers of the SEED-VC model



## Contact

[Thinal Ahugoda/thinalahugoda] - [thinal.ahugoda01@gmail.com]

Project Link: https://github.com/thinalahugoda/seed-vc-Implemented SERVER
