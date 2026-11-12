# Formula 1 Performance and DNF Analysis

This study uses a historical Formula 1 dataset (F1 DNF Dataset) to evaluate the performance, consistency, and behavior of competitors across several world championship seasons. The main goal is to identify patterns and trends considering the number of completed races, finishing positions, and the distribution of nationalities, as well as to understand the impact of technical evolution on car reliability[cite: 2].

## Data Structure

The project uses the `dataset.txt` file, which contains variables based on F1 classification database records[cite: 1, 2]. The main information explored includes:
* **Identification and Context**: Race year (`year`), driver identification (`driverRef`), and circuit[cite: 2].
* **Performance**: Finishing position (`positionOrder`) and points scored (`points`)[cite: 2].
* **Reliability**: Race completion indicator (`target_finish`), which shows whether the driver finished the race or suffered a DNF (Did Not Finish)[cite: 2].

## Analyses and Visualizations Performed

The project's Jupyter notebooks document the cleaning, organization, and graphical visualization of the data[cite: 2]:
* **Lewis Hamilton's Wins**: Pie chart detailing the percentage of races where the driver finished in 1st place, grouped by year[cite: 2].
* **Geographic and Nationality Distribution**: Bar chart showing the top 10 countries that hosted the most races[cite: 3], and a pie chart illustrating the top 10 most frequent driver nationalities[cite: 5].
* **Position Distribution**: Histogram illustrating the finishing positions only for successfully completed races[cite: 3].
* **Reliability Evolution**: Dual-axis line chart comparing the total number of DNFs against the total number of finished races per year[cite: 4].
* **Points vs. Average Position**: Line chart mapping the historical relationship between average points scored and average finishing positions per season[cite: 6].

## Technologies and Libraries

The analysis was developed in Python 3 using the Jupyter ecosystem[cite: 2, 7]. The dependencies listed in `requirements.txt` include[cite: 7]:
* `pandas` (DataFrame manipulation and data cleaning)[cite: 2, 7]
* `matplotlib` (Chart and graph generation)[cite: 2]
* `numpy` (Auxiliary numerical operations)[cite: 2, 3]
* `sqlalchemy` and `pymysql` (Database integration, if applicable)[cite: 7]
* `notebook` and `ipykernel` (Interactive computing environment)[cite: 7]
* `mypy` (Static typing)[cite: 7]

## How to Run

1. Make sure you have Python installed.
2. Clone this repository and navigate to the project folder.
3. Install the required dependencies by running the following command:
   ```bash
   pip install -r requirements.txt