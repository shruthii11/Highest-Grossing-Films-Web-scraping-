## Highest Grossing Films Web scraping
Certainly! Here's a README content template providing information about the provided code and its functionality:

---

## Web Scraping High-Grossing Films Data

### Overview
This Python script allows users to scrape data from a webpage containing tables of high-grossing films. Specifically, it targets the third table from the page and extracts information like the year of release, film title, worldwide gross, and budget.

### Dependencies
- **Python 3.x**
- **Beautiful Soup 4**: Used for parsing HTML content
- **Requests**: Used to make HTTP requests
- **CSV**: Python's built-in module for handling CSV files

### Usage
1. **Installation:**
    - Ensure you have Python installed.
    - Install required dependencies:
        ```bash
        pip install beautifulsoup4 requests
        ```
2. **Running the Script:**
    - Set the URL of the webpage in the `url` variable inside the script.
    - Run the script in a Python environment.

### Functionality
1. The script fetches the webpage using the provided URL.
2. It searches for tables with a specific class (`wikitable plainrowheaders`).
3. If at least three tables are found, it selects the third table.
4. The script then scrapes data from each row in the table, extracting the year, film title, worldwide gross, and budget.
5. The extracted data is written to a CSV file named `Highest_Grossing_Films.csv`.

### CSV File Structure
The generated CSV file contains the following columns:
- **Year**: The release year of the film
- **Title**: The title of the film
- **Worldwide gross**: The worldwide gross earnings of the film
- **Budget**: The budget of the film (if available)

### Notes
- Ensure the provided URL is accessible and contains the expected table structure.
- Check the generated CSV file for extracted data.

### Example Output (CSV)
```
Year    Title                    Worldwide gross                                      Budget
1915    The Birth of a Nation    $50,000,000â€“100,000,000$20,000,000+R($5,200,000)R    $110,000
1916    Intolerance              $1,750,000RIN                                        $385,907
1917    Cleopatra                $500,000*R                                            $300,000
```

---

