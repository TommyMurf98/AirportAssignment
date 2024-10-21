This was a universtiy assignemnt/project for the Advanced Programming module that processes and analyzes data related to airports and their communication frequencies. The core functionalities of the code involve loading data, calculating averages, generating graphs, and filtering data based on user input. Here’s a breakdown of the key components:

### 1. **Data Loading**:
   - The code reads two CSV files: `airports.csv` and `airport-frequencies.csv`.
   - These datasets are joined on the airport identifier (`ident`), which combines the airport details with their corresponding frequencies.

### 2. **Calculating Statistics**:
   - The function `get_average_text()` calculates statistics on airport frequencies, specifically focusing on large airports. It calculates:
     - The mean, median, and mode of the frequency (in MHz) for large airports.
     - The same statistics for frequencies above 100 MHz.
   - The results are formatted into a string that can be displayed to the user.

### 3. **Graph Generation**:
   - The function `generate_frequency_graph()` creates a frequency graph for a specific airport type (e.g., large airports). It sorts the frequencies and plots them using `matplotlib`.
   
### 4. **Data Filtering**:
   - The program allows users to input a frequency range (minimum and maximum), and the dataset is filtered accordingly. Frequencies outside this range are removed from the dataset.

### 5. **Saving and Loading Prepared Data**:
   - The prepared dataset can be saved as an Excel file (`Prepared.xlsx`) and reloaded later for further analysis.

### 6. **User Interface**:
   - The notebook includes a simple GUI using `Tkinter` for interacting with the user. Buttons are provided for loading data, showing averages, filtering frequencies, generating graphs, and saving the prepared data.

### Key Functions:
   - **`load_raw_data()`**: Loads and joins the raw datasets.
   - **`get_average_text()`**: Calculates statistical information about airport frequencies.
   - **`generate_frequency_graph(airport_type)`**: Generates a plot of frequencies for a specific airport type.
   - **`filter_frequencies()`**: Filters the dataset based on user-specified frequency limits.
   - **`save_prepared()`**: Saves the current dataset to an Excel file.
   - **`load_prepared()`**: Loads the saved dataset.

### Project Summary:
This project is a data analysis tool for airport communication frequencies, focusing on loading and visualizing the data, filtering it based on user input, and providing statistical insights such as mean, median, and mode frequencies. The Tkinter interface allows users to interact with the data easil
