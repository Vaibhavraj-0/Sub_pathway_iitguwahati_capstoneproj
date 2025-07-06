# Sub_pathway_iitguwahati_capstoneproj
# Dynamic Pricing for Urban Parking Lots

## Overview
Urban parking spaces are scarce and static pricing leads to inefficiency.  
This project implements a real-time, data-driven dynamic pricing engine for 14 parking lots, using demand, queue, vehicle type, traffic, and competition to optimize prices.

## Tech Stack
- Python 3.x
- Pandas
- Numpy
- Pathway (for real-time data processing)
- Bokeh (for visualization)
- Mermaid (for architecture diagram)

## Architecture Diagram

flowchart TD
A[Raw CSV Data] --> B[Preprocessing (Pandas)]
B --> C[Pathway Data Ingestion]
C --> D[Dynamic Pricing Logic]
D --> E[Output CSV (Predicted Prices)]
E --> F[Bokeh Visualization]


## Project Architecture & Workflow

1. **Data Preprocessing:**  
   - Combine date and time columns into ISO 8601 timestamp  
   - Map categorical variables (traffic, vehicle type) to numeric codes  
   - Save as `dataset_processed.csv`

2. **Real-Time Simulation (Pathway):**  
   - Ingest processed CSV as a real-time stream  
   - Apply dynamic pricing models (baseline, demand-based, competitive)  
   - Output price predictions per lot and time

3. **Visualization:**  
   - Plot real-time price trajectories for each parking lot using Bokeh

## How to Run

1. Clone this repo and open the notebook in Google Colab.
2. Upload your dataset as `dataset.csv`.
3. Run all cells in the notebook.
4. View generated visualizations and output files.

## Files

- `dynamic_pricing.ipynb`: Main notebook with code and explanations
- `dataset_processed.csv`: Preprocessed data (not included; generate from notebook)
- `output_priced.csv`: Model output
- `report.pdf`: (Optional) Detailed project report

## Documentation

- All code is commented and sections are explained in the notebook.
- See the report for methodology, assumptions, and results.

## License

MIT License

---

**For questions or collaboration, please contact me @Vaibhav_2311res77@iitp.ac.in or open an issue.**

