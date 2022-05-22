# 🎛️🎚️ Pixel Alchemist: Semantic image editing in realtime with a multi-parameter interface for StyleCLIP global directions

Open the interactive notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/titusss/PixelAlchemist/blob/main/PixelAlchemist.ipynb)

### FFHQ

![ffhq](https://user-images.githubusercontent.com/26855197/169719959-4ad7a367-b961-4021-85d7-0e84ca520894.gif)

### LSUN Churches

![lsun_churches](https://user-images.githubusercontent.com/26855197/169720012-c0802098-7175-4509-ae19-e4139a6a88e7.gif)

### LSUN Car

![lsun_car](https://user-images.githubusercontent.com/26855197/169719991-a0268e88-533f-4b02-b424-3c8a94441562.gif)


## Setup
Open the Google Colab Notebook, make sure your runtime has a GPU, run all cells, and open the web interface from the last cell. If you run the notebook for the first time, the GUI will ask you to register for a ngrok account to get an [authoken](https://dashboard.ngrok.com/get-started/your-authtoken) that you have to paste in the corresponding cell.

## Using your own model
Refer to the StyleCLIP repository, [here](https://github.com/orpatashnik/StyleCLIP#user-content-editing-via-global-direction), to learn how to preprocess your own StyleGAN model for global directions. You can use your model with the Pixel Alchemist notebook by uploading the "fs3", "W", "S", and "S_mean_std" files from the preprocessing and your .pkl file containing your StyleGAN weights to two different Google Drive folders. Finally, you have to add the two links (which need to be formatted for gdown) to the cell responsible for downloading all models from Google Drive.


## Roadmap
- [x] Initial code release
- [ ] Info note for model bias & ethics
- [ ] Add MIDI control
- [ ] Add more datasets (Imagenet-512 StyleGAN-XL, Conditional WikiArt, StyleGAN-Human)
- [ ] Edit uploaded images with inversion
- [ ] Text-to-image feature


## References
This is a multi-parameter interface for StyleCLIP:
"StyleCLIP: Text-Driven Manipulation of StyleGAN Imagery",
Or Patashnik, Zongze Wu, Eli Shechtman, Daniel Cohen-Or, Dani Lischinski
https://arxiv.org/abs/2103.17249
