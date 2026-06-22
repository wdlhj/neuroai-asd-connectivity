# NeuroAI ASD Connectivity

This project uses functional connectivity features derived from the ABIDE I dataset to classify autism spectrum disorder (ASD) versus control subjects with a Random Forest model.

## Dataset

The train and test splits in this repository come from the ABIDE I dataset.

Data is organized as:

- `data/train/X_train.npy`
- `data/train/y_train.npy`
- `data/test/X_test.npy`
- `data/test/y_test.npy`

## Requirements

import/install the Python packages listed in `requirements.txt`:

```bash
!pip install nilearn
```

## How To Run

1. Open `rfModel.ipynb` in Jupyter Notebook or upload to google colab.
2. Make sure the data paths in the notebook point to a relative path.
3. Run the notebook from top to bottom.

The notebook uses SHAP analysis to rank the most important connectivity features.

## Outputs

- `rf_feature_importances.npy`
- `rf_cv_results.csv`
- `shap_values_asd.npy`
- `top_shap_features.csv`
- `glass_brain_ortho.png`

These outputs summarize model performance and highlight the most influential brain connections for the ASD classification task.

## Notes

- The notebook was originally written with a Colab-style `/content` data path, so you may need to update file paths for local use.

## License

This project is open source and available under the MIT License.