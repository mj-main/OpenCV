# OpenCV

## 1. Overview
- OpenCV 패키지의 사용법을 파이썬 코드로 정리한 내용입니다.

## 2. 순서
- Introduction
  - AI는 computer science의 한 분야이며, computer vision은 대표적인 AI 기술의 활용 사례입니다.
  - 이미지는 2차원 행렬로 표현되며, 각 성분은 이미지의 픽셀을 의미합니다.
  - 이미지의 픽셀은 RGB 3가지의 요소값을 갖습니다.
  
- Image&Video Display
  - OpenCV는 많이 사용되는 컴퓨터 비전 패키지입니다.
  - OpenCV를 통해 이미지와 비디오 파일을 읽고 디스플레이합니다.

- Image Manipulation
  - 일부 픽셀에 접근하여 값을 수정합니다.
  - 노이즈 이미지를 필터링합니다.
  - 이미지를 평행이동, 회전이동, 스캐일링(resize)합니다.
  - Image segmentation과 Line detection을 할 수 있습니다.
  
- Image Feature
  - Image의 가장 기본적인 feature는 point feature이다.
  - Templete matching을 통해 Object Detection을 수행합니다.
  - 픽셀값의 변화율이 최대인 지점을 계산하여 Corner Detection을 수행합니다.
  - SIFT 또는 이를 보완한 ORB를 통해 interesting point를 찾을 수 있습니다.
  
- Object Tracking
  - Object Tracking은 3step: Object Detection, Classification, Tracking 순서로 진행됩니다.
    - Object Detection: Knn method를 통한 Backgroudn subtraction과 Lucas-Kanade method를 통한 Optical flow 등
    - Object Classification: 코드를 따로 정리하지는 않았습니다.
    - Object Tracking: Bounding box의 크기가 일정한 Meanshift Method과 물체에 따라 크기가 조절이 되는 CAM(Continuosly  Adaptive Meanshift)
