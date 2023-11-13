# THUHITSZ_Coop-MMAC
THUHITSZ_Coop Team for MICCAI MMAC 2023 - Myopic Maculopathy Analysis Challenge



##### Data Augmentation

`python train_diffusion.py`



##### Inference

1. [Download](https://codalab.lisn.upsaclay.fr/competitions/12477#learn_the_details) validation sets

2. [Download](https://drive.google.com/drive/folders/1DRO1SsVxQe_rW3W9CmUBAoxpXzP4Z0L_) *best_model.pth* and *checkpoint.pth*

3. Load model and image

`network =  model.model()`

`network.load(model_path)`

`input_image = cv2.imread(img_path)`

`img = cv2.cvtColor(input_image, cv2.COLOR_BGR2RGB)`

4. Make prediction

`pred_class, attention = network.predict(input_image)`



##### Visualization

`python visualization.py`


