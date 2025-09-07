# Advanced Text Summarizer 🚀

An intelligent, dual-mode text summarization tool designed to deliver both rapid, localized summaries and high-quality, context-aware summaries using Google's Gemini API. This project has evolved from a simple scraper into a versatile tool that handles multiple input sources, including complex web pages and local documents.

The full web application is currently live for testing, providing a seamless user experience for all summarization needs.

## ✨ Features

This tool is packed with advanced features to provide a flexible and powerful summarization experience:

* **Dual Summarization Modes:**
    * **Fast Summary:** Utilizes a high-speed, local frequency-based algorithm for near-instantaneous extractive summaries.
    * **AI Summary:** Leverages the power of the **Google Gemini API** to generate sophisticated, abstractive summaries that understand context and nuance.

* **Multiple Input Sources:**
    * **Web Articles & Pages:** Go beyond Wikipedia! The tool integrates an advanced web scraper (`newspaper3k`) to intelligently extract the main content from news articles, blogs, and other complex web pages.
    * **Local Files:** Directly summarize your documents by uploading `.txt` and `.pdf` files.

* **Full-Fledged Web Application (Live for Testing):**
    * **Guest Access:** Anyone can use the summarization features directly without needing an account.
    * **User Authentication:** Sign up or log in using your email or social accounts (Google, Meta) to unlock personalized features.
    * **Saved History:** Logged-in users can access a history of their previous summaries, making it easy to find and reuse important information.

---
## ⚙️ How the Summarizers Work

### Fast Summary (Frequency-Based Extractive Method)

The "Fast Summary" mode operates entirely locally and is built on a classic NLP extractive summarization technique. It doesn't create new sentences; instead, it intelligently identifies and extracts the most important ones from the original text. The process works as follows:

1.  **Text Pre-processing:** The initial text is cleaned to make it suitable for analysis. This involves removing special characters, digits, and extra spaces.
2.  **Tokenization:** The cleaned text is broken down into individual sentences and words.
3.  **Stopword Removal:** Common words that add little semantic value (like "the", "a", "is") are removed to focus on the core topics.
4.  **Word Frequency Calculation:** The script calculates the frequency of each remaining word in the entire document. The idea is that words used more often are more central to the topic.
5.  **Sentence Scoring:** Each sentence is assigned a score based on the frequency of the words it contains. Sentences with a higher concentration of frequently-used words are considered more important.
6.  **Summarization:** The top-scoring sentences are selected and combined to form the final, concise summary.

This entire process is computationally lightweight, resulting in a summary that is generated almost instantly.

### AI Summary (Abstractive Method via Gemini API)

The "AI Summary" mode uses a modern, abstractive approach. Instead of just extracting sentences, it sends the entire text to Google's Gemini model. The model reads and *understands* the context, main points, and nuances of the document. It then generates a brand new, coherent summary in its own words, much like a human would. This results in a higher-quality, more readable summary but requires an internet connection and an API key.

---

## 🛠️ Installation

To set up the project locally, follow these steps:

1.  **Clone the repository:**
    ```
    git clone [https://github.com/Rishav03Raj/Automated_text_summarization.git](https://github.com/Rishav03Raj/Automated_text_summarization.git)
    ```
2.  **Navigate to the project directory:**
    ```
    cd Automated_text_summarization
    ```
3.  **Install the required dependencies:**
    ```
    pip install -r requirements.txt
    ```

## 💻 Usage

To use the summarization tool, run the main script from your terminal:
he script will guide you through the process, allowing you to choose your input source (URL or file) and summarization type (Fast or AI).

## 🚀 Future Roadmap

This project is under active development with many exciting features planned for the near future:

* **Enhanced Dashboard:** A more intuitive user dashboard for managing saved summaries.
* **Team Collaboration:** Features for sharing summaries and collaborating within teams.
* **Expanded File Support:** Adding support for more document types like `.docx` and `.pptx`.
* **Browser Extension:** A planned browser extension for summarizing web pages with a single click.

## 🤝 Contributing

Contributions are welcome! If you'd like to help improve the project, please follow these steps:

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## 📧 Contact

**Project Link:** [https://github.com/Rishav03Raj/Automated_text_summarization](https://github.com/Rishav03Raj/Automated_text_summarization)
