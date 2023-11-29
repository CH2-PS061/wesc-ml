## Dataset and Data Preparation

The dataset we use for this model is our own collective dataset, [Edible Plants Indonesia](https://www.kaggle.com/datasets/amzadin/edible-plants-indonesia). This dataset contains 826 images of 12 kinds of edible wild plants in Indonesia. We use information from [this](https://www.kompas.tv/feature/215481/5-tumbuhan-liar-yang-bisa-dikonsumsi-saat-tersesat-di-hutan?page=all) and [this](https://blog.eigeradventure.com/tanaman-liar-yang-bisa-dimakan/) website.

We split the dataset into two directories: Training and Testing, with 5 images for each kinds for Testing, and the rest for Training. When modeling, We split the Training images into train and validation with ratio 8:2. Then, we rescale the dataset by 1/255, resize it to 300x300, and apply image augmentation by [Chris Deotte](https://www.kaggle.com/code/cdeotte/rotation-augmentation-gpu-tpu-0-96#Data-Augmentation) that utilize GPU, making the process faster.

Here are some images from the dataset and their labels we use on this model.

![An old rock in the desert](/media/dataset_overview.png "Shiprock, New Mexico by Beau Rogers")
