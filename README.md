# downloadable

This repository is for hosting small datasets or models weights, in order to achieve efficiency, as well as avoiding Google drive download quotas in downloading popular datasets.
> The datasets will be regrouped for the compressed file to be less than 2GB. The files are located in the "releases" sections above.

## Contents:

- ### [CycleGAN model weights](https://github.com/jimmy-academia/downloadable/releases/tag/weight.cyc)
    - model weights for [LaSGSA repository](https://github.com/jimmy-academia/LaSGSA), ICCV 2021 paper [Attack As the Best Defense: Nullifying Image-to-Image Translation GANs via Limit-Aware Adversarial Attack](https://openaccess.thecvf.com/content/ICCV2021/html/Yeh_Attack_As_the_Best_Defense_Nullifying_Image-to-Image_Translation_GANs_via_ICCV_2021_paper.html)
    - <b>pre.tar.gz</b><br> contains weights for cyclegan (model Blond, Glass and Blue)

- ### [CycleGAN, pix2pix and pix2pixHD model weights](https://github.com/jimmy-academia/downloadable/releases/tag/weight.cyc-pix) 
    - model weights for [Adversarial-Attack-CycleGAN-and-pix2pix repository](https://github.com/jimmy-academia/Adversarial-Attack-CycleGAN-and-pix2pix), WACV 2020 DeepPAB workshop paper [Disrupting Image-Translation-Based DeepFake Algorithms with Adversarial Attacks](https://openaccess.thecvf.com/content_WACVW_2020/html/w4/Yeh_Disrupting_Image-Translation-Based_DeepFake_Algorithms_with_Adversarial_Attacks_WACVW_2020_paper.html)
    - <b>pre.tar.gz</b><br> contains weights for cyclegan and pix2pix (model Smile, Blond, Bald, Glass, Blond-pix)
    - <b>prehd.tar.gz</b><br> prehd.tar.gz contains weights for pix2pixHD (model Blond-HD, trained with image size 256)


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

#### notes on slow downloads:  
We found that wget speeds vary largely from `14MB/s` all the way to `700KB/s` for trials within seconds appart. If the download speed is slow, stop the process and try again. We found that the suggestion in this [reference](https://stackoverflow.com/questions/94074/slow-wget-speeds-when-connecting-to-https-pages) does not work, and the download speed is mainly a matter of luck.

### extraction commands:   
`unzip celeba.zip`   
`7za e img_celeba.7z`   
