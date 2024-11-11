# AI Basics - Climate Data from Berlin Tempelhofer Feld
## Predicting with Historical Weather Data

This project uses temperature, humidity, and precipitation data from Berlin Tempelhofer Feld to predict soil temperature. The data comes from Open Meteo's [historical weather API](https://open-meteo.com/en/docs/historical-weather-api). You can find the imported data and the setup for the data split in the [data](https://github.com/Till1983/ai-basics-climate-data/tree/main/data) folder. The different regression models can be found in the [models](https://github.com/Till1983/ai-basics-climate-data/tree/main/models) folder.

## How to Run the Software Locally
### 1. Clone the Repository

`git clone https://github.com/Till1983/ai-basics-climate-data.git`

### 2. Move into the Main Folder

`cd ai-basics-climate-data`

### 3. Create a Virtual Environment

`python3 -m venv venv`

### 4. Activate the Virtual Environment

`source venv/bin/activate`

### 5. Install Dependencies from requirements.txt

`pip install -r requirements.txt`

## How to Run the Models
### 1. Import the Data and Save It in a CSV File

Open **data_preparation.ipynb** in the **data** folder and click the **Run All** button above the first cell. You will be prompted to select a virtual environment for the kernel upon clicking. Select the environment of the current repository. The cells will continue to execute after selection. Running all cells will execute the Open Meteo API response script and save the imported data in a CSV file.

### 2. Split Data into Training and Test Sets

Open **data_split.ipynb**, also located in the **data** folder, and click **Run All**. The train and test datasets will be saved in separate files for use in the model notebooks.