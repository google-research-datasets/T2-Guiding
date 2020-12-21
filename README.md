# T2-Guiding

T2 Guiding is a dataset of 1000 images, each with six image labels. Three labels are Visual Genome objects extracted from the image using an FRCNN. The other three labels are extracted from the image using the Google Cloud Vision API. This dataset is used as the test set in the paper: "Understanding Guided Image Captioning Performance across Domains".

More details are available in this <a href="https://arxiv.org/abs/2012.02339">paper</a> (please cite the paper if you use or discuss this dataset in your work):
<div class="highlight highlight-source-shell"><pre>
@article{ng2020understanding,
  title={Understanding Guided Image Captioning Performance across Domains},
  author={Edwin G. Ng and Bo Pang and Piyush Sharma and Radu Soricut},
  journal={arXiv preprint arXiv:2012.02339},
  year={2020}
}
</pre></div>

# Data Format

The released data is provided as a TSV (tab-separated values) text file with the following columns:

<p align='center'>Table 1: Columns in TSV files.</p>

| Column   | Description                                                                                               |
| -------- | --------------------------------------------------------------------------------------------------------- |
| 1        | Image key. A unique identifier for the image (a hexadecimal number. e.g., 0000d67245642c5f)               |
| 2        | Visual Genome objects. Three objects detected from the image using a FRCNN model trained on Visual Genome |	
| 3        | Image labels. Three labels extracted from the image using the Google Cloud Vision API                     |	

# Downloads

The dataset is available for download <a href="https://storage.cloud.google.com/t2-guiding/t2_guiding_set.tsv?_ga=2.140996917.-665667375.1608176209">here</a>. The mapping from the image key to the image URL can be found in the  cvpr2019.tsv.meta file of the original <a href="https://www.conceptualcaptions.com/winners-and-data">T2 dataset</a> download link.
