# DataMate 🤖

DataMate is an interactive chatbot application designed to help users query and retrieve information from CSV files. Leveraging Google Generative AI, FAISS, and LangChain, DataMate ensures accurate, context-aware responses to your data-related questions.

## Features

- **CSV File Support**: Seamlessly upload and process multiple CSV files.
- **Conversational Interface**: Query your data through an intuitive chat interface.
- **Data Embeddings**: Efficiently stores and retrieves data using FAISS.
- **Google Generative AI**: Provides precise, natural language responses.
- **User-Friendly UI**: Built with Streamlit for a clean and responsive interface.

---

## Prerequisites

- Python 3.8 or higher
- Google API key for Generative AI
- Internet connection

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repository/datamate.git
   cd datamate
   ```

2. Install dependencies:

   ```bash
   pip install -r req.txt
   ```

3. Configure your environment:

   - Create a `.env` file in the project root directory with your Google API key:

     ```env
     GOOGLE_API_KEY=your-google-api-key
     ```

---

## Usage

1. Run the application:

   ```bash
   streamlit run main.py
   ```

2. Open the application in your browser (default: `http://localhost:8501`).

3. Upload CSV files using the sidebar and click "Submit & Process."

4. Start chatting and querying your data interactively.

---

## How It Works

1. **Data Parsing**: Extracts structured data from uploaded CSV files.
2. **Text Chunking**: Breaks large datasets into manageable text chunks.
3. **Embedding Storage**: Generates embeddings using Google Generative AI and stores them in FAISS for efficient searches.
4. **Question Answering**: Uses a conversational chain model to provide relevant responses based on your questions.

---

## File Structure

- `main.py`: Main application script for DataMate.
- `req.txt`: Contains the list of required Python libraries.
- `.env`: Environment configuration file (user-provided).
- `faiss_index/`: Stores FAISS vector indexes (created during runtime).

---

## Future Enhancements

- Support for additional data formats like Excel and JSON.
- Improved conversational AI for more complex queries.
- Integration with visualization tools for better data insights.

---

## Contributing

We welcome contributions! Feel free to open issues or submit pull requests to improve DataMate.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.