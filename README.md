# Crop Yield Prediction

This project predicts crop yield using machine learning based on environmental and agricultural data. It consists of a Flask web application (`app.py`) and a Jupyter notebook (`Crop Yield Prediction.ipynb`) for exploratory data analysis and model development.

## Features

- **Flask Web App**: User-friendly interface for crop yield prediction.
- **Machine Learning Model**: Uses pre-trained models for yield prediction.
- **Data Preprocessing**: Handles feature transformation for model input.
- **Exploratory Data Analysis**: Jupyter notebook provides insights, visualizations, and data cleaning.

## File Structure

- `app.py`: Flask application for serving predictions.
- `Crop Yield Prediction.ipynb`: Notebook for EDA, feature engineering, and model training.
- `dtr.pkl`: Pickled Decision Tree Regression model.
- `preprocessor.pkl`: Pickled data preprocessor (for feature transformation).
- `templates/index.html`: HTML template for the web UI (not included here).
- `yield_df.csv`: Dataset used for training and evaluation (not included here).

## How to Use

### 1. Setup

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install flask numpy pandas scikit-learn seaborn matplotlib
   ```
3. Ensure `dtr.pkl` and `preprocessor.pkl` are present.
4. Place the dataset (`yield_df.csv`) in the working directory.

### 2. Run the Web App

```bash
python app.py
```
Visit [http://localhost:5000](http://localhost:5000) in your browser.

### 3. Use the Jupyter Notebook

Open `Crop Yield Prediction.ipynb` in Jupyter Lab/Notebook to explore the data, visualizations, and model development steps.

## Data

The dataset contains the following columns:

- `Area`: Country/Region
- `Item`: Crop type
- `Year`: Year
- `hg/ha_yield`: Crop yield (hectogram/hectare)
- `average_rain_fall_mm_per_year`: Average rainfall per year (mm)
- `pesticides_tonnes`: Pesticide usage (tonnes)
- `avg_temp`: Average temperature (°C)

## Prediction

On the web app, input the following features:
- Year
- Average rainfall (mm)
- Pesticides (tonnes)
- Average temperature (°C)
- Area (country/region)
- Item (crop type)

The app returns a predicted crop yield.

## Notebook Highlights

- Data cleaning (missing values, duplicates)
- Statistical analysis (describe/corr)
- Data visualization (country/crop distribution)
- Feature engineering
- Model training and saving

## License

This project is for educational purposes.

For questions or issues, please open an Issue or Pull Request.
