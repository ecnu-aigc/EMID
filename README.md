## Dataset Summary

**E**motionally paired **M**usic and **I**mage Dataset (**EMID**) is a novel dataset designed for the emotional matching of music and images. The EMID dataset contains 10738 unique music clips, each of which is paired with 3 images in the same emotion state，as well as rich annotations. These musical clips were categorized into the 13 emotional categories proposed by [What music makes us feel: At least 13 dimensions organize subjective experiences associated with music across different cultures](https://pnas.org/doi/full/10.1073/pnas.1910704117), from which we obtained  1836 original music clips . Subsequently, we acquired images labeled with eight Mikel emotions from this [Building a Large Scale Dataset for Image Emotion Recognition: The Fine Print and The Benchmark](http://arxiv.org/abs/1605.02677). Through the processing pipeline propose  in our EMID paper, we expanded the original dataset and obtained the final dataset.

Please cite the our EMID paper, when using this dataset: http://arxiv.org/XXXXX

### Processing Pipeline

![pipeline](./pipeline.jpg)



### Statistics of EMID

|     Emotion      | A    | B    | C    | D    | E    | F    | G    | H    | I    | J    | K    | L    | M    | Total |
| :--------------: | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----- |
| Before expanding | 45   | 80   | 54   | 131  | 306  | 174  | 367  | 86   | 36   | 124  | 129  | 105  | 199  | 1836  |
| After expanding  | 255  | 545  | 320  | 771  | 1531 | 889  | 1832 | 1036 | 323  | 1014 | 799  | 484  | 939  | 10738 |

## Dataset Usage

The published dataset takes the form of a `.csv` file that contains the filenames of music clips and corresponding emotional matched images. In order to use this dataset, your should download the music data and csv file in this repository  as well as the image data in this [address](https://onedrive.live.com/?cid=ab6522e29f6ed9a0&id=AB6522E29F6ED9A0%21101730&authkey=!AH57YMUbsP-qNls)

The usage of the dataset is published under Non Commercial Creative Commons (BY-NC) license which provides free access to the data for non-profit work. We are by no means can guaranty support for its users. This database comes as is with no guaranty of correctness and we are not liable to any damage it might cause. 



## Data Fields

