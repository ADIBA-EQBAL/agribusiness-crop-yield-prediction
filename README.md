Agribusiness Crop Yield Prediction — Week 2
Project goal
Design and demonstrate a machine-learning workflow that predicts crop yield (tonnes per hectare) from weather, soil, crop, season, fertilizer, and irrigation features.
Files
- crop_yield_model.py — runnable example comparing Linear Regression and Random Forest.
- Week_2_Model_Design_Report.docx — detailed design report.
Run
Install Python 3.10+ and dependencies:
pip install numpy pandas scikit-learn
python crop_yield_model.py
The script intentionally uses synthetic data to make the example self-contained. Its metrics must not be presented as real agricultural performance. For a real project, replace make_demo_dataset() with a vetted dataset, document the source and units, and evaluate on held-out years/regions.
Suggested real-data workflow
1. Identify a trustworthy crop-yield dataset and document licensing, geography, years, and units.
2. Join yield records with weather, soil, irrigation, and input data using consistent location and season identifiers.
3. Audit missingness, outliers, duplicates, and possible target leakage.
4. Use chronological or region-based validation where appropriate.
5. Compare a simple baseline with tree-based models and report MAE, RMSE, and R².
6. Record model limitations and monitor performance across seasons and locations.
