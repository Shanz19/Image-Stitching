# Image Stitching with Key Point Detection

This project focuses on image stitching using key point detection, matching descriptors, RANSAC algorithm, and homography matrix estimation.

## Key Steps in the Code

1. **Detect Key Points**: SIFT algorithm is applied to detect key points in the images.
2. **Match Descriptors**: Descriptors of the key points are matched using a brute force matcher.
3. **RANSAC Algorithm**: RANSAC algorithm is employed to estimate the homography matrix based on matched descriptors.
4. **Apply Warp Transformation**: After obtaining the homography matrix, a warp transformation is applied to stitch images.

## Key Features of the Code

- **SIFT Key Point Detection**: SIFT algorithm is utilized to identify key points.
- **Key Point Statistics**:
  - Image 1: 1354 keypoints
  - Image 2: 2033 keypoints
  - Image 3: 2714 keypoints
- **Brute Force Matching**: Distance between descriptors is computed using a brute force matcher.
- **Robust Matching**: Minimum distances are used to track key points between Image 1 and Image 2.
- **Rotation and Scale Invariance**: The results demonstrate that SIFT operator can robustly match images even under rotation or scale transformations.

