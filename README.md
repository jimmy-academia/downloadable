# downloadable

> This repository is for hosting small datasets or models weights, in order to achieve efficiency, as well as avoiding Google drive download quotas in downloading popular datasets.
> The datasets will be regrouped for the compressed file to be less than 2GB. The files are located in the "releases" sections above.

## Current table of contents:

- ### [CelebA Datasets](https://github.com/jimmy-academia/downloadable/releases/tag/dset.celeba)
    - <b>CelebA.zip</b><br>this file contains <b>Large-scale CelebFaces Attributes (CelebA) Dataset</b>, excluding the img_aligned_celeba.zip<br>[original site link](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html), [original google drive link](https://drive.google.com/drive/folders/1lENOECdd-8is7RnVSGOrlCdamYJ8hyhd)<br>the folder contains:
        - Img
            - img_celeba.7z (may be broken)
            - img_align_celeba_png.7z (may be broken)
        - Eval
            - list_eval_partition.txt (ex: "000001.jpg 0" 0,1,2)
        - Anno
            - list_landmarks_celeba.txt
            - list_landmarks_align_celeba.txt
            - list_bbox_celeba.txt
            - list_attr_celeba.txt
            - identity_CelebA.txt
    - <b>img_align_celeba.zip</b><br>this file contains the <b>aligned and cropped images</b> from the <b>Large-scale CelebFaces Attributes (CelebA) Dataset</b>
    - <b>CelebA-HQ.zip</b><br>this file contains <b>CelebA-HQ dataset</b> along with various attributes from the <b>CelebAMask-HQ</b><br>[original github repo link](https://github.com/switchablenorms/CelebAMask-HQ), [original google drive link](https://drive.google.com/file/d/1badu11NqxGf6qM3PTTooQDJvQbejgbTv/view)<br>the folder contains:
        - CelebA-HQ-img<br>(contains the celebaHQ dataset images from 15000.jpg to 29999.jpg)
        - CelebA-HQ-to-CelebA-mapping.txt<br>(celebaHQ index to original celeba image index)
        - CelebAMask-HQ-attribute-anno.txt<br>(attributes "smiling", "black_hair"...)
        - CelebAMask-HQ-pose-anno.txt<br>(yaw, pitch, raw(roll))
        - README.txt<br>readme file from the original github repo CelebAMask-HQ
    - <b>CelebA-HQ-img2.zip</b><br>(contains the <b>celebaHQ</b> dataset images from 0.jpg to 14999.jpg)
    - <b>CelebAMask-HQ-mask-anno.zip</b><br>this file contains <b>the masks for CelebA-HQ dataset</b> from the <b>CelebAMask-HQ</b> (same as above)<br>the folder contains:
        - subdirectories 0 to 14<br>each containing 14 mask x 2000 images<br>the 14 masks are: cloth, hair, l/r_eye, skin, l/u_lip, mouth, neck, nose, l/r_brow, l/r_ear (if it appears in the image) <br>filename example: `00001_cloth.png`
    


## Usage   
### download commands:   
right click on *.zip and chose "copy link url" to get the `<url>`    
`wget <url>`   

### extraction commands:   
`unzip celeba.zip`   
`7za e img_celeba.7z`   
