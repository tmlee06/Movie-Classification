# Movie Classification Project

A comprehensive data analysis and machine learning project that performs movie genre classification using natural language processing and k-nearest neighbors (KNN) algorithms.

## 📋 Project Overview

This project analyzes movie datasets to understand word frequency patterns and correlations, then applies machine learning techniques to classify movies by genre. The analysis includes text preprocessing, stem analysis, correlation studies, and predictive modeling.

## 🚀 Features

### Data Analysis
- **Movie Dataset Processing**: Load and analyze movie data with ratings, genres, and word frequency features
- **Natural Language Processing**: 
  - Word stemming analysis using stem.csv
  - Vocabulary mapping between stemmed and original words
  - Word frequency correlation analysis
- **Statistical Analysis**:
  - Correlation coefficient calculations between word proportions
  - Scatter plot visualizations with regression lines
  - Distribution analysis of word stems

### Machine Learning
- **K-Nearest Neighbors (KNN) Classification**:
  - Euclidean distance calculations for feature comparison
  - Fast distance computation using vectorized operations
  - Genre prediction based on word frequency features
- **Model Evaluation**:
  - Training/testing data split (85% training, 15% testing)
  - Performance analysis on test dataset

## 📊 Dataset Structure

The project works with two main datasets:
- `movies.csv`: Contains movie information including:
  - Title, Genre, Rating
  - Word frequency proportions for various terms
  - Feature columns for machine learning
- `stem.csv`: Contains word stemming mappings:
  - Stem: Root form of words
  - Word: Original word forms

## 🛠️ Setup and Installation

### Prerequisites
- Python 3.7+
- Required Python packages:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn
  ```

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Movie-Classification.git
   cd Movie-Classification
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have the required data files:
   - `movies.csv`
   - `stem.csv`

## 📖 Usage

### Running the Analysis
1. Open the Jupyter notebook:
   ```bash
   jupyter notebook Movie_Classifaction_Project.ipynb
   ```

2. Execute cells sequentially to run the complete analysis pipeline

### Key Analysis Steps

1. **Data Exploration**:
   - Load and examine movie dataset
   - Analyze specific movie ratings and word counts

2. **Text Processing**:
   - Perform stemming analysis
   - Create vocabulary mappings
   - Analyze word distribution patterns

3. **Correlation Analysis**:
   - Calculate correlations between word proportions
   - Visualize relationships with scatter plots
   - Identify highly correlated word pairs

4. **Machine Learning**:
   - Split data into training and testing sets
   - Implement KNN classification
   - Predict movie genres based on word features

## 📈 Results

The project demonstrates:
- **Word Stem Analysis**: 22,594 stems map to single words, showing the effectiveness of stemming
- **Correlation Insights**: Identifies word pairs with significant correlations (e.g., "space" vs "outer" with r=0.319)
- **Classification Performance**: KNN algorithm successfully classifies movies by genre using word frequency features

## 🔬 Technical Implementation

### Key Functions
- `distance_two_features()`: Calculates Euclidean distance between movies
- `fast_distances()`: Vectorized distance computation for efficiency
- `most_common()`: Determines most frequent genre in nearest neighbors
- `classify()`: Main KNN classification function

### Performance Optimizations
- Vectorized operations using NumPy
- Efficient distance calculations
- Memory-optimized data processing

## 📁 Project Structure

```
Movie-Classification/
├── Movie_Classifaction_Project.ipynb  # Main analysis notebook
├── README.md                          # Project documentation
├── movies.csv                         # Movie dataset (required)
├── stem.csv                          # Word stemming data (required)
└── requirements.txt                  # Python dependencies
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- Email: your.email@example.com

## 🙏 Acknowledgments

- Movie dataset sources
- Natural language processing libraries
- Machine learning community resources

---

*This project demonstrates practical applications of data science and machine learning in entertainment industry analysis.*