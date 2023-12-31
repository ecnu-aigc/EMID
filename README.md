## Dataset Summary

**E**motionally paired **M**usic and **I**mage Dataset (**EMID**) is a novel dataset designed for the emotional matching of music and images. The EMID dataset contains 10,738 unique music clips, each of which is paired with 3 images in the same emotional category，as well as rich annotations. These musical clips are categorized into the 13 emotional categories proposed by [What music makes us feel: At least 13 dimensions organize subjective experiences associated with music across different cultures](https://pnas.org/doi/full/10.1073/pnas.1910704117), from which we obtain 1,836 original music clips. Subsequently, we acquire images labeled with Mikels' eight emotions from [Building a Large Scale Dataset for Image Emotion Recognition: The Fine Print and The Benchmark](http://arxiv.org/abs/1605.02677). Through the processing pipeline proposed in our paper, we expanded the original music clips and obtain the final dataset.

Please cite our paper when using the EMID dataset: https://arxiv.org/abs/2308.07622

### Processing Pipeline

![pipeline](./pipeline.jpg)

### Statistics of EMID

| Emotion          |  A   |  B   |  C   |  D   |  E   |  F   |  G   |  H   |  I   |  J   |  K   |  L   |  M   | Total |
| ---------------- | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :---: |
| Before expanding |  45  |  80  |  54  | 131  | 306  | 174  | 367  |  86  |  36  | 124  | 129  | 105  | 199  | 1836  |
| After expanding  | 255  | 545  | 320  | 771  | 1531 | 889  | 1832 | 1036 | 323  | 1014 | 799  | 484  | 939  | 10738 |

## Dataset Download

The published dataset takes the form of a `.csv` file that contains the filenames of music clips and corresponding emotional matched images. In order to use this dataset, your should download the csv file as well as the music/image data in the this [huggingface address](https://huggingface.co/datasets/ecnu-aigc/EMID) .



<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>,which provides free access to the data for non-profit work. We are by no means can guaranty support for its users. This database comes as is with no guaranty of correctness and we are not liable to any damage it might cause.





## Data Fields

| filed_name       | explanation                                                  | example                                                      |
| ---------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Audio_Filename   | unique Filename of the music clip                            | 106.m4a___172.mp3                                            |
| genre            | Letter A to M, representing one of the 13 emotional category   | K                                                            |
| feeling          | Feelings reported by participants after listening to this music clip and their proportions | "33% Sad, depressing, 22% Awe-inspiring, amazing, 22% Proud, strong, 22% Triumphant, heroic, 19% Dreamy, 15% Beautiful, 15% Bittersweet, 11% Calm, relaxing, serene, 11% Compassionate, sympathetic, 11% Entrancing, 11% Transcendent, mystical, 7% Eerie, mysterious, 7% Painful, 7% Tender, longing, 4% Energizing, pump-up, 4% Indignant, defiant" |
| emotion          | Ratings of subjective experiences elicited by the music on 11 emotional dimensions, ranging from 1 to 9 | "5,5.3,5,6,3.1,6.1,5.1,3.6,6.2,5.9,5.6"                      |
| Image1_filename  | -                                                            | excitement_0616.jpg                                          |
| Image1_tag       | emotional category of image 1                                  | excitement                                                   |
| Image1_text      | The textual description of Image 1 generated by the GIT model | ['the marching band in the parade']                          |
| Image2_filename  | -                                                            | amusement_2906.jpg                                           |
| Image2_tag       | emotional category of image 2                                  | amusement                                                    |
| Image2_text      | The textual description of Image 2 generated by the GIT model | ['the marching band at disneyland']                          |
| Image3_filename  | -                                                            | amusement_2226.jpg                                           |
| Image3_tag       | emotional category of image 3                                  | amusement                                                    |
| Image3_text      | The textual description of Image 3 generated by the GIT model | ['a marching band in a parade with people watching.']        |
| is_original_clip | If this value is true, the music clip is from the original music dataset, otherwise it is expanded from the original music clip through our processing pipeline. The original music clips are considered to provide a better emotional matching performance | False                                                        |

For more information about feeling and emotion filed, you can refer to  [What music makes us feel: At least 13 dimensions organize subjective experiences associated with music across different cultures](https://pnas.org/doi/full/10.1073/pnas.1910704117) and their visualized interactive [site](https://www.ocf.berkeley.edu/~acowen/music.html#).

