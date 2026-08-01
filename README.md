# Aviation Accident Analysis


## Project Overview

This project examines aviation accident records from the National Transportation Safety Board (NTSB) between **1983 and 2023** to evaluate the safety performance of different aircraft manufacturers and models.

The analysis was carried out from the perspective of a consulting firm advising an airline or aviation insurance company. The goal was to identify aircraft with stronger historical safety records by considering two important indicators:

* The likelihood of an aircraft being completely destroyed in an accident.
* The likelihood of occupants sustaining fatal or serious injuries.

Recommendations are presented separately for small aircraft and larger commercial aircraft to provide more meaningful comparisons.

---

## Dataset

The project uses the **Aviation Accident Database** obtained from Kaggle, which contains aviation accident records from **1948 to 2023**.

To focus on aircraft that are more representative of modern aviation, only accidents occurring from **1983 onwards** were included in the analysis, assuming an approximate aircraft service life of 40 years.

---

## Data Preparation

Before analysis, the dataset was cleaned and transformed using **Pandas**. The preparation process involved:

* Selecting accident records from 1983 onwards.
* Excluding amateur-built aircraft.
* Retaining only professionally manufactured airplanes.
* Addressing missing values.
* Standardizing aircraft manufacturer and model names.
* Creating a unique aircraft identifier.
* Generating additional variables, including:

  * Total occupants
  * Total fatal and serious injuries
  * Fatal/serious injury rate
  * Aircraft destruction status
* Removing variables with a high proportion of missing data.

---

## Exploratory Analysis

Aircraft safety was assessed using two main indicators:

* Average fatal/serious injury rate
* Average aircraft destruction rate

The aircraft were grouped into two categories:

* **Small aircraft:** fewer than 20 occupants
* **Large aircraft:** 20 or more occupants

The analysis also explored how accident outcomes varied according to:

* Weather conditions
* Engine type

Data visualizations were produced using **Matplotlib** and **Seaborn** to highlight trends and comparisons.

---

## Main Findings

### Manufacturer Performance

For smaller aircraft, manufacturers such as **Airbus, Boeing, Bombardier, Bombardier Inc.,** and **Maule** generally recorded lower injury and aircraft destruction rates.

Among larger passenger aircraft, **Airbus, Boeing, Bombardier, Bombardier Inc.,** and **McDonnell Douglas** consistently showed stronger safety performance across both evaluation measures.

---

### Model Performance

Several aircraft models manufactured by **Boeing** and **Airbus** ranked among those with the lowest average fatal and serious injury rates. Models produced by **Bombardier** and **Embraer** also demonstrated favorable results within the large-aircraft category.

---

### Additional Factors

#### Weather

Accidents that occurred under **Instrument Meteorological Conditions (IMC)** were associated with considerably higher rates of severe injuries and aircraft destruction than accidents that occurred in **Visual Meteorological Conditions (VMC)**.

#### Engine Type

Aircraft powered by **Turbo Fan** engines generally experienced the most favorable safety outcomes, while **Turbo Prop** aircraft tended to have comparatively higher injury and destruction rates.

---

## Conclusion

The findings show that aircraft safety is best evaluated using more than one performance measure. Considering both injury severity and aircraft destruction provides a more complete understanding of accident outcomes.

Overall, **Airbus, Boeing, Bombardier, Bombardier Inc.,** and **McDonnell Douglas** consistently performed well across multiple analyses, making them the strongest recommendations based on the historical accident data.

---

## Repository Structure

```text
.
├── data/
│   ├── AviationData.csv
│   └── AviationData_Clean.csv
├── Aviation_Accidents_Cleaning.ipynb
├── Aviation_Accidents_Data_Analysis.ipynb
├── README.md
└── LICENSE
```

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

