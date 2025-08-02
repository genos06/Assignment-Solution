# ML Intern Assignment

This project demonstrates face detection and orientation correction using the RetinaFace model (`resnet50_2020-07-20`). It includes two main notebooks:

- **1_Problem2_a.ipynb**: Detects faces in images, expands bounding boxes, and saves annotated images.
- **2_Problem2_b.ipynb**: Detects faces, estimates face orientation, rotates images to correct orientation, and saves results.
- **3_Problem2_bonus.ipynb**: Detects faces, crops the bounding boxes, estimates face orientation, rotates images to correct orientation, and saves results.

## Setup

1. Install dependencies using pip:

   ```bash
   pip install -r requirements.txt
   ```

2. Place your image zip files (`img-set-1.zip`, `img-set-2.zip`) in the project directory.

## Usage

- Open the notebooks in Jupyter or VS Code.
- Run each cell sequentially.
- Outputs (annotated images, rotated images, CSV files) are saved in respective folders.

## Dependencies

See `requirements.txt` for dependancies.

## Output

- Annotated images with bounding boxes (`boxed_images/`)
- Rotated images with corrected orientation (`rotated_images/`)
- Bonus problem Solution (`rotated_images/{image_name}/`)
- CSV files with detection results (`problem2_a.csv`, `problem2_b.csv`)

## Notes

- The model is device agnostic (uses GPU if available).
- Padding and bounding box expansion are used to improve detection accuracy.
