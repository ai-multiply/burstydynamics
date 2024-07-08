# Bursty dynamics

bursty_dynamics is a Python package designed to facilitate the analysis of temporal patterns in longitudinal data. It provides functions to calculate the burstiness parameter (BP) and memory coefficient (MC), detect event trains, and visualize results.

credit: 
This package implements the alternate burstiness parameter described in the paper ‘Measuring Burstiness for Finite Event Sequences’ by Kim, Eun-Kyeong, and Hang-Hyun Jo, and memeory coefficient described in ‘Burstiness and Memory in Complex Systems’ by Goh, K.-I., and A.-L. Barabási. 


## Features

- Burstiness Parameter (BP) and Memory Coefficient (MC) Calculation: Calculate BP and MC to quantify the irregularity and memory effects of event timing within longitudinal data.
- Event Train Detection: Detect and label event trains based on user-defined criteria such as maximum inter-event time and minimum burst size.
- Train-Level Analysis: Analyse BP and MC for detected event trains, providing insights into temporal patterns within clusters of events.
- Visualization Tools: Visualise temporal patterns with scatter plots, histograms, kernel density estimates (KDE), and more, facilitating interpretation of analysis results.
- User-Friendly Interface: Designed for ease of use, with clear function parameters and output formats, making it accessible to both novice and experienced users.

## Installation

You can install the bursty_dynamics via pip:
```sh
pip install bursty_dynamics
```

## Usage
Here's a quick overview of how to use the main functionalities of the package:

```sh
from bursty_dynamics.scores import calculate_scores
from bursty_dynamics.trains import train_detection, calculate_train_info, calculate_scores_train

# Load your longitudinal data into a DataFrame
# df = load_data()

# Calculate burst parameters
burst_params = calculate_scores(df, subject_id = 'eid', time_col = 'event_dt')
```

For more example of usage, please take a look at examples.ipynb in the example folder.

## License

bursty_dynamics is licensed under the MIT License. See the LICENSE file for more details.


## Contributing
Contributions are welcome! If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request on GitHub.




