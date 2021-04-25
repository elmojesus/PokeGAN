# PokeGAN
A 512x512 [stylegan2-ada](https://github.com/NVlabs/stylegan2-ada) model trained on pokemon images

# Dataset
The dataset was taken from this [kaggle](https://www.kaggle.com/brilja/pokemon-mugshots-from-super-mystery-dungeon)Pokemon Mugshots dataset

The datset contained 64x64 images of pokemonm, which is a little too small

I used [waifu2x-chainer](https://github.com/tsurumeso/waifu2x-chainer), to upscale the mugshots to 512x512

![smol](smd/0_01.png)
![big](w2x/0_01.png)

# Training
Originally wanted to train on free GCP TPU's provided by [TRC](https://sites.research.google/trc/), but porting stylegan2-ada to work on TPUs proved to be a challenge.
Instead, I used Google Colab Pro and trained StyleGan2-ada on Tesla V100s for a few days
