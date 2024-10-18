

# Feed Optimization for Dairy Cows

## Overview
This project demonstrates how to optimize the feed mix for dairy cows using Linear Programming. The goal is to minimize the cost of the feed while ensuring that the nutritional requirements for the cows are met. The project uses real-world nutrient data fetched from the USDA FoodData Central API, and the optimization is done using the `PuLP` library in Python.

### Key Features:
- **Data Source**: Nutrient data for feed ingredients is fetched from the USDA FoodData Central API.
- **Feed Ingredients**: Corn silage, soybean meal, barley, and hay.
- **Nutrient Requirements**: Optimization ensures that the feed meets the minimum requirements for protein, fat, fiber, and energy.
- **Cost Minimization**: The linear programming model is set to minimize the total cost of the feed mix.
- **Visualizations**: Includes pie charts and bar charts to visually represent the optimized feed mix and the nutritional contributions of each ingredient.

---

## Project Structure:
The project consists of the following key components:
- **API Integration**: Fetches real-time nutrient data for each feed ingredient.
- **Linear Programming Model**: Optimizes the feed mix using `PuLP` to meet nutritional requirements at the lowest cost.
- **Data Handling**: Cleans and processes the fetched data, replacing missing values with mean values.
- **Visualizations**: Provides insights into the optimized feed mix and nutritional contributions with clear, easy-to-understand charts.

---

## Visualizations:
- **Pie Chart**: Displays the proportions of each ingredient in the optimized feed mix.
- **Bar Chart**: Shows how each feed ingredient contributes to the total amounts of protein, fat, fiber, and energy.

![Feed Mix Visualization](path-to-your-pie-chart-image.png)

---

## Installation

### Prerequisites:
- Python 3.x
- Jupyter Notebook (optional but recommended)

### Python Libraries:
Make sure to install the necessary Python libraries before running the project. You can install them by running the following command:

```bash
pip install requests pandas pulp matplotlib
```

---

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/feed-optimization.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd feed-optimization
   ```

3. **Run the Jupyter Notebook**:
   Open the `feed_optimization.ipynb` file in Jupyter Notebook or JupyterLab.

4. **Run the Python Script**:
   If you prefer to run the script in a terminal or Python environment, execute the notebook cells sequentially to fetch the data, optimize the feed, and display the visualizations.

---

## Project Walkthrough

### Step 1: Fetching Data from USDA API
We use the USDA FoodData Central API to fetch the nutritional information for four common feed ingredients: **corn silage**, **soybean meal**, **barley**, and **hay**. The nutrient data includes the protein, fat, fiber, and energy content of each feed ingredient.

### Step 2: Data Preprocessing
After fetching the data, we handle missing values by replacing any zeros with the mean value for that nutrient across all feed ingredients.

### Step 3: Feed Optimization Model
We set up a linear programming model using `PuLP` to minimize the cost of the feed while meeting the cows' nutritional requirements for protein, fat, fiber, and energy. Bounds are set to ensure a balanced feed mix, with upper and lower limits for each ingredient.

### Step 4: Visualizing the Results
Once the model is solved, we generate visualizations to showcase the optimized feed mix and how each ingredient contributes to the cows' total nutritional intake.

---

## Example Output

Here’s an example of the optimized feed mix and its visual representation:

- **Feed Mix**:
    - Corn silage: 30%
    - Soybean meal: 5%
    - Barley: 5%
    - Hay: 60%
- **Total Cost**: $14.00 per kg

![Nutritional Contribution Visualization](path-to-your-bar-chart-image.png)

---

## Future Enhancements
- **More Feed Ingredients**: Incorporating additional feed ingredients into the optimization model.
- **Dynamic Nutritional Requirements**: Adding a feature to dynamically change the nutritional requirements based on different cow types or stages of lactation.
- **Interactive Dashboard**: Implementing an interactive dashboard using a tool like `Dash` or `Streamlit` for better user interaction with the optimization results.

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contributing
Feel free to submit issues or pull requests if you want to contribute to improving this feed optimization project.

---

## Contact
For any inquiries or further information, feel free to contact me at:
- **Email**: jebin.jervis2@mail.dcu.ie
- **LinkedIn**: https://www.linkedin.com/in/jebin-larosh-jervis-a52938123/
- **GitHub**: https://github.com/Jebin1999

---

### Acknowledgments:
- Special thanks to the [USDA FoodData Central](https://fdc.nal.usda.gov/) for providing the nutrient data used in this project.
