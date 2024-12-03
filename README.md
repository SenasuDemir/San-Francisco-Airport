# San Francisco International Airport (SFO) Clustering Analysis

## Project Overview

This project aims to analyze and cluster passenger activity data from **San Francisco International Airport (SFO)** to uncover meaningful patterns and insights. Using clustering techniques, the analysis categorizes operational activities and highlights trends in terminal usage, boarding areas, and passenger flow. The clustering model's **optimal number of clusters** was determined using the **elbow method**, with the best value being **k=3**. The model achieved a **silhouette score of 0.8286**, reflecting well-defined clusters and high-quality segmentation.

---

## Project Aim

The primary goal of this project is to analyze and cluster passenger activity data to:
- Categorize operational activities, such as passenger flow (**enplaned**, **deplaned**, or **transit**),
- Analyze airline operations and terminal usage,
- Identify trends across different terminals and boarding areas.

This clustering approach provides actionable insights to optimize airport operations, improve resource allocation, and enhance the overall passenger experience.

---

## <font color='gold'>Dataset Column Descriptions

| Column Name                 | Description                                                                                     | Example                |
|-----------------------------|-------------------------------------------------------------------------------------------------|------------------------|
| **Activity Period**         | The time period of the activity in **YYYYMM** format.                                          | `200507` (July 2005)  |
| **Operating Airline**       | The name of the airline operating the flight or activity.                                      | `ATA Airlines`        |
| **Operating Airline IATA Code** | The IATA (International Air Transport Association) code for the operating airline.             | `TZ`, `AC`            |
| **Published Airline**       | The airline under which the flight or activity is marketed or published.                      | `Air Canada`          |
| **Published Airline IATA Code** | The IATA code for the published airline.                                                     | `AC`                  |
| **GEO Summary**             | Indicates whether the activity is **Domestic** or **International**.                          | `Domestic`, `International` |
| **GEO Region**              | Specifies the geographical region associated with the flight or activity.                     | `US`, `Canada`        |
| **Activity Type Code**      | Describes the type of passenger activity: `Deplaned`, `Enplaned`, or `Thru / Transit`.        | `Deplaned`            |
| **Price Category Code**     | Indicates the fare category of the flight or activity.                                        | `Low Fare`, `Other`   |
| **Terminal**                | Specifies the terminal at the airport where the activity occurred.                            | `Terminal 1`          |
| **Boarding Area**           | Represents the boarding area within the specified terminal.                                   | `B`                   |
| **Passenger Count**         | The number of passengers associated with the activity.                                        | `27271`               |

---

## Methodology

1. **Data Preprocessing**:
   - Cleaned and prepared the dataset for clustering.
   - Scaled numerical features to ensure balanced contributions.

2. **Clustering**:
   - Performed clustering using the **KMeans algorithm**.
   - Determined the optimal number of clusters using the **Elbow Method**:
     - The optimal number of clusters was found to be **k=3**.
   - Evaluated clustering performance with the **Silhouette Score**:
     - Achieved a score of **0.8286**, indicating well-separated and cohesive clusters.

3. **Visualization**:
   - Visualized the results using various charts, including:
     - **Sunburst Chart** for hierarchical data relationships.
     - **Bar Charts** and **Heatmaps** to analyze patterns in passenger activity.

---

## Results and Conclusion

The clustering analysis yielded three distinct clusters, revealing significant insights into passenger activities at SFO:
- **Cluster 1**: Characterized by high passenger traffic in certain terminals and boarding areas.
- **Cluster 2**: Highlighted unique patterns in airline operations and regional activity.
- **Cluster 3**: Captured less frequent but critical transit and low-fare passenger activities.

### Key Outcomes:
- Identified trends in terminal and boarding area usage.
- Improved understanding of passenger flow patterns, allowing for more effective airport resource allocation.

With a silhouette score of **0.8286**, the clusters are well-defined and provide actionable insights for decision-making at SFO.


