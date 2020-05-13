# Cross Modal Compression: towards human-comprehensible semantic compression

<table width="100%" cellpadding="0" cellspacing="0" border='0'>
 <tr><td align="center">
<img src="./fig/CNNRNN_with_Attn.jpg" width="95%" align="canter">
  </td></tr>
</table>
![framework](./fig/CNNRNN_with_Attn.jpg？raw=true)
(coming soon)

# Cite us
If you use this code or part of it, please cite us!  
*anonymous, "Cross Modal Compression: towards human-comprehensiblesemantic compression"* [arxiv](coming soon)


# Prerequisites
 - linux
 - python 3.5 (not test on other versions)
 - pytorch 1.3+
 - torchaudio 0.3
 - librosa, pysoundfile
 - json, tqdm, logging



## data preparing
### download dataset and pretrained model
 - you can download CUB-200-2011 dataset and MS COCO 2014 from the offficial site
 - download our json file for MS COCO from [here](link)
 - download our pretrained models from [here](link)

## training the CMC
### training the DAMSM model
### training the ImageText model
### training the TextImage model

## eval the CMC
1. write the pretrained models' paths in cfg/bird_eval.yml for CUB-200-2011 dataset or cfg/coco_eval.yml for MS COCO dataset
2. run
```
python ./ImageText/end_to_end_test.py --cfg cfg/coco_eval.yml --data_dir COCO_PATH --output_dir ./output/end_to_end_coco_test
```
for MS COCO or 
```
python ./ImageText/end_to_end_test.py --cfg cfg/coco_eval.yml --data_dir CUB_PATH --output_dir ./output/end_to_end_bird_test
```


# project home page(coming soon)
our results, data, pretrained model can be found on our [speaker-recognition-attacker]() project main page.

# Acknowledgement
Thanks to the valuable discussion with Junlong Gao. Besides, thanks to the open source of [COCO API](https://github.com/cocodataset/cocoapi), [AttnGAN](https://github.com/taoxugit/AttnGAN), [a-PyTorch-Tutorial-to-Image-Captioning](https://github.com/sgrvinod/a-PyTorch-Tutorial-to-Image-Captioning).

 **Note that this work is only for research. Please do not use it for illegal purposes.**

