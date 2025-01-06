🎥 Movie Recommendation System
Discover movies you'll love with this Movie Recommendation System! Built with powerful algorithms and an intuitive interface, this project provides personalized recommendations and showcases movie posters for a rich user experience.

🌟 Key Features
🚀 Smart Recommendations
Based on advanced similarity algorithms using movie metadata.

🎨 Dynamic Posters
Fetches high-quality posters from the TMDb API to enhance your movie discovery experience.

⚡ Intuitive UI
Powered by Streamlit for seamless interaction.

🔗 Scalable and Modular
Easily extendable for future enhancements or dataset updates.

🛠️ Technologies Used
Programming Language: Python

Libraries and Frameworks:

pandas: For data manipulation

pickle: For serialized data storage

scikit-learn: For similarity computation

Streamlit: For creating the interactive UI

requests: For API integration

Data Source: The Movie Database (TMDb)

💡 How Does It Work?
1️⃣ Data Preprocessing
1.The system uses the Bag of Words (BoW) model, a popular text representation technique.

Screenshot 2024-12-05 185212

2.CountVectorizer transforms movie descriptions into numerical vectors to capture the importance of words.

2️⃣ Similarity Computation
A Cosine Similarity algorithm is applied to measure the relationship between movies based on their feature vectors.

Screenshot 2024-12-05 223318

The similarity matrix is precomputed and stored in similarities.pkl, allowing the system to quickly retrieve the top matches for any selected movie.

3️⃣ Recommendation Generation
When a user selects a movie:

1.The system identifies its index in the dataset.

2.Similarity scores are retrieved from the matrix.

3.The top 5 most similar movies are selected and returned.

4️⃣ Poster Integration

Posters are dynamically fetched using the TMDb API to create a visually rich experience image

5️⃣ Interactive User Interface

Built with Streamlit, the UI provides:

1.A dropdown menu to select a movie.

2.A "Recommend" button to fetch similar movies.

3.A grid display for movie titles and posters.

Screenshot 2024-12-05 223456

📂 Project Files
streamlit(ap).py:-Main application script

movie_dict.pkl:-Serialized movie dataset

similarities.pkl:-Precomputed similarity matrix

movierecommender.ipynb:-Notebook for data preprocessing and vectorization

🚀 How to Run the Project
1.Clone the Repository

Screenshot 2024-12-05 223939

2.Navigate to the Project Directory

Screenshot 2024-12-05 223947

3.Install Dependencie

Screenshot 2024-12-05 223952

4.Run the Application

Screenshot 2024-12-05 223957

5.Access the App Open the local URL displayed in your terminal (usually http://localhost:8501).

📊 How the Backend Works
1.Input: User selects a movie.

2.Processing:

1.Retrieve the selected movie’s similarity scores.

2.Sort and select the top 5 movies based on scores.

3.Fetch posters dynamically via the TMDb API.

3.Output: Display recommendations with titles and posters.

🎨 Visual Preview
Screenshot 2024-12-03 234944

🌟 Why Choose This Project?
1.Speed: Precomputed similarity matrix ensures fast responses.

2.Scalability: Modular design supports future upgrades and new datasets.

3.Visual Appeal: High-quality posters elevate user experience.

4.Ease of Use: Intuitive interface simplifies navigation.
