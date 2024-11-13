# AI Basics - Climate Data from Berlin Tempelhofer Feld
## Predicting Soil Temperature with Historical Weather Data

This project uses historical temperature, humidity, and precipitation data from Berlin Tempelhofer Feld to predict soil temperature. Data is sourced from Open Meteo's [historical weather API](https://open-meteo.com/en/docs/historical-weather-api) and covers a period from January 1990 to November 2024. The imported data and data split setup are located in the [data folder](https://github.com/Till1983/ai-basics-climate-data/tree/main/data), while different regression models can be found in the [models folder](https://github.com/Till1983/ai-basics-climate-data/tree/main/models).

## Running the Software Locally
### 1. Clone the Repository

```bash
git clone https://github.com/Till1983/ai-basics-climate-data.git
```

### 2. Navigate to the Main Folder

```bash
cd ai-basics-climate-data
```

### 3. Create a Virtual Environment

```bash
python3 -m venv venv
```

### 4. Activate the Virtual Environment

On Linux/macOS:
```bash
source venv/bin/activate
```

On Windows:
```bash
venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

## Running the Models
### 1. Import Data and Save as CSV

Open **data_preparation.ipynb** in the **data** folder, then select **Run All** from the toolbar to execute each cell. When prompted, select the virtual environment for the kernel. This notebook runs the Open Meteo API script, retrieving the data and saving it in CSV format.

### 2. Split Data into Training and Testing Sets

Open **data_split.ipynb** (also in the **data** folder) and click **Run All**. This notebook splits the data into training and testing datasets, saving them as separate files for use in the model notebooks.

### 3. Evaluate the Models

With the data split and saved, open any file in the **models** folder to evaluate various regression models. Each file imports the train and test data at the beginning, allowing you to review model performance directly.