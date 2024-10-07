### Project: Information Retrieval System using Probabilistic Binary Independence Model (BIM)

#### Description:
This project is an **Information Retrieval System** built using the **Probabilistic Binary Independence Model (BIM)**. The system allows users to search a collection of text documents using a query, and ranks the documents based on their relevance to the query. The project is implemented in **Python** using the **Flask** web framework for creating the user interface.

#### Key Features:
- **Document Preprocessing**: Text documents are preprocessed by converting to lowercase and splitting into words. 
- **Term Frequency and Document Frequency Calculation**: The system computes both **Term Frequency (TF)** and **Document Frequency (DF)** for each word in the corpus, which are essential for ranking documents.
- **BIM Ranking Model**: The **Binary Independence Model (BIM)** is used to compute relevance probabilities for each document based on the query terms. The model assumes that terms occur independently and ranks documents accordingly.
- **Laplace Smoothing**: The system applies **Laplace (add-one) smoothing** to handle the zero-frequency problem, ensuring no term has zero probability of occurring, even if it does not appear in a particular document.
- **User Interface**: A simple and user-friendly web interface that allows users to input search queries, and displays the top 3 relevant documents along with their scores.
  
#### Structure:
- **Flask-based Web App**: A lightweight web interface built using Flask.
- **Search Logic**: Implemented in Python, leveraging BIM for probabilistic ranking of documents.
- **Data Handling**: Text documents are stored in a folder, and the system processes and ranks them dynamically based on user queries.

#### How to Use:
1. Place your text documents inside the `data/` folder.
2. Run the Flask app by executing `python app.py`.
3. Navigate to `localhost:5000` in your web browser.
4. Enter a query in the search bar and view the ranked results of the top 3 documents.

#### Installation:
1. Clone this repository.
   ```bash
   git clone https://github.com/your-username/your-repository.git
   ```
2. Install the required dependencies.
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Flask application.
   ```bash
   python app.py
   ```

#### Future Improvements:
- Implementing more sophisticated ranking models, such as TF-IDF or BM25.
- Enhancing the user interface with advanced filtering and sorting options.
- Expanding the system to handle different file formats (e.g., PDF, Word).
  
#### License:
This project is licensed under the MIT License.

---

This is a lightweight yet powerful information retrieval system suited for educational purposes or as a foundation for more advanced search systems.
