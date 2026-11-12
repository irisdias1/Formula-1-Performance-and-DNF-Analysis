# Formula 1 Performance and DNF Analysis

This study uses a historical Formula 1 dataset (F1 DNF Dataset) to evaluate the performance, consistency, and behavior of competitors across several world championship seasons. The main goal is to identify patterns and trends considering the number of completed races, finishing positions, and the distribution of nationalities, as well as to understand the impact of technical evolution on car reliability.

## Data Structure

The project uses the `dataset.txt` file, which contains variables based on F1 classification database records. The main information explored includes:
* **Identification and Context**: Race year (`year`), driver identification (`driverRef`), and circuit.
* **Performance**: Finishing position (`positionOrder`) and points scored (`points`).
* **Reliability**: Race completion indicator (`target_finish`), which shows whether the driver finished the race or suffered a DNF (Did Not Finish).

## Analyses and Visualizations Performed

The project's Jupyter notebooks document the cleaning, organization, and graphical visualization of the data:
* **Lewis Hamilton's Wins**: Pie chart detailing the percentage of races where the driver finished in 1st place, grouped by year.
* **Geographic and Nationality Distribution**: Bar chart showing the top 10 countries that hosted the most races, and a pie chart illustrating the top 10 most frequent driver nationalities.
* **Position Distribution**: Histogram illustrating the finishing positions only for successfully completed races.
* **Reliability Evolution**: Dual-axis line chart comparing the total number of DNFs against the total number of finished races per year.
* **Points vs. Average Position**: Line chart mapping the historical relationship between average points scored and average finishing positions per season.

## Technologies and Libraries

The analysis was developed in Python 3 using the Jupyter ecosystem. The dependencies listed in `requirements.txt` include:
* `pandas` (DataFrame manipulation and data cleaning)
* `matplotlib` (Chart and graph generation)
* `numpy` (Auxiliary numerical operations)
* `sqlalchemy` and `pymysql` (Database integration, if applicable)
* `notebook` and `ipykernel` (Interactive computing environment)
* `mypy` (Static typing)

## How to Run

1. Make sure you have Python installed.
2. Clone this repository and navigate to the project folder.
3. Install the required dependencies by running the following command:
   ```bash
   pip install -r requirements.txt
