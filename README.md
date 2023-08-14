## Dataset Summary

**E**motionally paired **M**usic and **I**mage Dataset (**EMID**) is a novel dataset designed for the emotional matching of music and images. The EMID dataset contains 10,738 unique music clips, each of which is paired with 3 images in the same emotion category，as well as rich annotations. These musical clips were categorized into the 13 emotional categories proposed by [What music makes us feel: At least 13 dimensions organize subjective experiences associated with music across different cultures](https://pnas.org/doi/full/10.1073/pnas.1910704117), from which we obtained  1836 original music clips . Subsequently, we acquired images labeled with eight Mikel emotions from [Building a Large Scale Dataset for Image Emotion Recognition: The Fine Print and The Benchmark](http://arxiv.org/abs/1605.02677). Through the processing pipeline propose  in our EMID paper, we expanded the original music clips and obtained the final dataset.

Please cite our paper when using the EMID dataset: http://arxiv.org/XXXXX

### Processing Pipeline

![pipeline](./pipeline.jpg)

### Statistics of EMID

| Emotion          |  A   |  B   |  C   |  D   |  E   |  F   |  G   |  H   |  I   |  J   |  K   |  L   |  M   | Total |
| ---------------- | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :---: |
| Before expanding |  45  |  80  |  54  | 131  | 306  | 174  | 367  |  86  |  36  | 124  | 129  | 105  | 199  | 1836  |
| After expanding  | 255  | 545  | 320  | 771  | 1531 | 889  | 1832 | 1036 | 323  | 1014 | 799  | 484  | 939  | 10738 |

## Dataset Download

The published dataset takes the form of a `.csv` file that contains the filenames of music clips and corresponding emotional matched images. In order to use this dataset, your should download the csv file in this repository  as well as the music/image data in the following onedirve address

[music data address](https://1drv.ms/u/s!AqPSEQiEauC1jBSuIYXsnOFlxwJm?e=0EODxr)

[image data address](https://onedrive.live.com/?cid=ab6522e29f6ed9a0&id=AB6522E29F6ED9A0%21101730&authkey=!AH57YMUbsP-qNls)

The usage of the dataset is published under Non Commercial Creative Commons (BY-NC) license which provides free access to the data for non-profit work. We are by no means can guaranty support for its users. This database comes as is with no guaranty of correctness and we are not liable to any damage it might cause. 



## Data Fields

| filed_name       | explanation                                                  | example                                                      |
| ---------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Audio_Filename   | unique Filename of the music clip                            | 106.m4a___172.mp3                                            |
| genre            | Letter A to M, representing one of the 13 emotion category   | K                                                            |
| feeling          | Feelings reported by participants after listening to this music clip and their  proportions | "33% Sad, depressing, 22% Awe-inspiring, amazing, 22% Proud, strong, 22% Triumphant, heroic, 19% Dreamy, 15% Beautiful, 15% Bittersweet, 11% Calm, relaxing, serene, 11% Compassionate, sympathetic, 11% Entrancing, 11% Transcendent, mystical, 7% Eerie, mysterious, 7% Painful, 7% Tender, longing, 4% Energizing, pump-up, 4% Indignant, defiant" |
| emotion          | Ratings of  subjective experiences elicited by the music on eleven emotional dimensions from 1 to 9 | "5,5.3,5,6,3.1,6.1,5.1,3.6,6.2,5.9,5.6"                      |
| Image1_filename  | -                                                            | excitement_0616.jpg                                          |
| Image1_tag       | emotion category of image 1                                  | excitement                                                   |
| Image1_text      | The textual description of Image 1 generated by the GIT model | ['the marching band in the parade']                          |
| Image2_filename  | -                                                            | amusement_2906.jpg                                           |
| Image2_tag       | emotion category of image 2                                  | amusement                                                    |
| Image2_text      | The textual description of Image 2 generated by the GIT model | ['the marching band at disneyland']                          |
| Image3_filename  | -                                                            | amusement_2226.jpg                                           |
| Image3_tag       | emotion category of image 3                                  | amusement                                                    |
| Image3_text      | The textual description of Image 3 generated by the GIT model | ['a marching band in a parade with people watching.']        |
| is_original_clip | If this value is true, the music clip is from the original music dataset, otherwise it is expanded from the original music clip through our processing pipeline. The original music dataset was considered to have a better emotional matching performance | False                                                        |

For more information about feeling and emotion filed, you can refer to  [What music makes us feel: At least 13 dimensions organize subjective experiences associated with music across different cultures](https://pnas.org/doi/full/10.1073/pnas.1910704117) and their visualized interactive [site](https://www.ocf.berkeley.edu/~acowen/music.html#).

