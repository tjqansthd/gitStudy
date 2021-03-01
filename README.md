**3. Dense g.t dataset**  
   We take an inpainting method from [DenseDepth](https://github.com/ialhashim/DenseDepth) to get dense g.t for gradient loss.  
   (You can train our model using only data loss without gradient loss, then you don't need dense g.t)  
   Corresponding inpainted results from **'`./datasets/KITTI/data_depth_annotated/2011_xx_xx_drive_xxxx_sync/proj_depth/groundtruth/image_02`'** are should be saved in **'`./datasets/KITTI/data_depth_annotated/2011_xx_xx_drive_xxxx_sync/dense_gt/image_02`'**.

* KITTI data structures are should be organized as below:
          |-- datasets
                         |-- KITTI
            |-- data_depth_annotated  
               |-- 2011_xx_xx_drive_xxxx_sync
                  |-- proj_depth  
                       |-- groundtruth			# official G.T folder  
               |-- ... (all drives of all days in the raw KITTI)  
           |-- 2011_09_26			               # raw RGB data folder  
               |-- 2011_09_26_drive_xxxx_sync  
           |-- 2011_09_29  
           |-- ... (all days in the raw KITTI)  
