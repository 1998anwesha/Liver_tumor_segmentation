# Liver_tumor_segmentation
Using ResUnet to segment liver tumors from CT scan images.

We have used Google Colab pro for this project. The training code can also work on normal Colab using T4 GPU and memory space of less than 30 GB. 

## File and dataset extraction
First, extract the file content onto one folder "imageprocessing" in google drive "MyDrive". Now, this folder should have multiple folders and Colab files  
Download dataset Liver segmentation [3D-IRCADb-01](https://www.ircad.fr/research/data-sets/liver-segmentation-3d-ircadb-01/).  This is a zip file of size 806 MB.
Create a new folder called "Dataset" in "imageprocessing" and place this zip file there.

Next, open dataset_generation.ipynb in Google Colab. Follow the instructions in it. 
On running this, "train" folder will be created in “imageprocessing”. Total time taken for data extraction will be around 2 hours.

## Training Liver and Tumor segmentation models
Now open liver_segmentation.ipynb file and run it. It will generate the models folder. There are already three pre-trained models trained on 25%, 50% and 100% data in the models folder. We get following epochs.

Run Liver_segmentation_results to view the final outputs. Run models in models folder or using your trained version. We see results and metric information there

Then run tumor_segmentation file for 25% dataset. This gives following results:

Run Tumor_segmentation_result to view final output. Run the model in models folder or your own.

Run on 25% data for speed. Run tumor_segmentation on 100 epochs for better results.

