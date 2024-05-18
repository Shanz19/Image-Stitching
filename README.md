# Image Stitching with Key Point Detection

This project focuses on image stitching using key point detection, matching descriptors, RANSAC algorithm, and homography matrix estimation.

## Key Steps in the Code

1. **Detect Key Points**: SIFT algorithm is applied to detect key points in the images.
2. **Match Descriptors**: Descriptors of the key points are matched using a brute force matcher.
3. **RANSAC Algorithm**: RANSAC algorithm is employed to estimate the homography matrix based on matched descriptors.
4. **Apply Warp Transformation**: After obtaining the homography matrix, a warp transformation is applied to stitch images.

## Key Features of the Code

- **SIFT Key Point Detection**: SIFT algorithm is utilized to identify key points.
- **Key points of image 1 and 2**:
<img width="581" alt="Screenshot 2024-05-18 at 5 19 31 PM" src="https://github.com/Shanz19/Image-Stitching/assets/117365514/d0829011-594c-42fd-acce-2e89f3deee41">

- **Key points of image 2 and 3**:
<img width="633" alt="Screenshot 2024-05-18 at 5 19 42 PM" src="https://github.com/Shanz19/Image-Stitching/assets/117365514/94c80e29-2005-4684-8f16-f66065ef1552">

- **Key Point Statistics**:
  - Image 1: 1354 keypoints
  - Image 2: 2033 keypoints
  - Image 3: 2714 keypoints
- **Brute Force Matching**: Distance between descriptors is computed using a brute force matcher.
- **Robust Matching**: Minimum distances are used to track key points between Image 1 and Image 2.
- **Rotation and Scale Invariance**: The results demonstrate that SIFT operator can robustly match images even under rotation or scale transformations.

## Stitched Image (Output):
<img width="691" alt="Screenshot 2024-05-18 at 5 21 29 PM" src="https://github.com/Shanz19/Image-Stitching/assets/117365514/7b0432db-8cae-4a21-8820-fa3e21dbcc6c">


