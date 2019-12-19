# downloadable

> This repository is for hosting small datasets or models weights, in order to achieve efficiency in downloading popular datasets
> The datasets will be regrouped for the compressed file to be less than 2GB
> In the "releases" section above, 

Current table of contents:

- celeba Datasets
    - celebA.zip<br>this file contains <b>Large-scale CelebFaces Attributes (CelebA) Dataset</b><br>[original site link](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html), [original google drive link](https://drive.google.com/drive/folders/1lENOECdd-8is7RnVSGOrlCdamYJ8hyhd)<br>the folder contains:
        - Img
            - img_align_celeba.zip
            - img_celeba.7z
            - img_align_celeba_png.7z
        - Eval
            - list_eval_partition.txt (ex: "000001.jpg 0" 0,1,2)
        - Anno
            - list_landmarks_celeba.txt
            - list_landmarks_align_celeba.txt
            - list_bbox_celeba.txt
            - list_attr_celeba.txt
            - identity_CelebA.txt
    - CelebA-HQ.zip<br>this file contains <b>CelebA-HQ dataset</b> along with various attributes<br>[original github repo link](https://github.com/switchablenorms/CelebAMask-HQ), [original google drive link](https://drive.google.com/file/d/1badu11NqxGf6qM3PTTooQDJvQbejgbTv/view)<br>the folder contains:
        - CelebA-HQ-img<br>(contains the celebaHQ dataset images from 0.jpg to 29999.jpg)
        - CelebA-HQ-to-CelebA-mapping.txt<br>(celebaHQ index to original celeba image index)
        - CelebAMask-HQ-attribute-anno.txt
        
    
    




extraction commands:
`unzip celeba.zip`  
`7za e img_celeba.7z`
