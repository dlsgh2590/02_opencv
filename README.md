OpenCV를 활용하여 다양한 이미지 처리 및 영상 처리 기법을 학습하고 실습한 예제 코드들을 모아놓은 프로젝트입니다.

---

## 학습 목표 및 내용 요약

- OpenCV 기본 컬러 공간 변환 이해  
- 히스토그램 평활화와 CLAHE 기법 실습  
- 이미지의 관심 영역(ROI) 선택 및 처리  
- 임계처리(Thresholding)를 통한 이미지 이진화  
- 실시간 영상 캡처 및 처리

---

## 파일별 상세 설명

### 1. bgr2gray.py  
- OpenCV에서 기본 색상 공간인 BGR을 그레이스케일로 변환하는 예제  
- `cv2.cvtColor()` 함수 사용법 이해

### 2. color.py  
- 이미지에서 특정 색상 영역을 추출하거나 색상 변환 실습  
- 컬러 필터링 및 색상 범위 지정 방법 소개

### 3. cropped.jpg  
- 예제에서 사용할 크롭된 이미지 파일

### 4. histo_clahe.py  
- CLAHE (Contrast Limited Adaptive Histogram Equalization) 기법을 적용해 이미지 대비 향상  
- 국소 대비 향상을 통해 어두운 영역 디테일 살리기

### 5. histo_equalize.py  
- 전통적인 히스토그램 평활화 적용 예제  
- 전체 이미지 대비 균일화 및 밝기 조절

### 6. histo_equalize_yuv.py  
- YUV 색 공간에서 밝기 채널(Y)에 히스토그램 평활화 적용  
- 컬러 정보는 유지하면서 밝기만 개선하는 기법

### 7. histo_gray.py  
- 그레이스케일 이미지에 히스토그램 평활화 적용 예제

### 8. histo_noramize.py  
- 이미지 정규화(Normalization)를 통한 픽셀 값 범위 조정  
- `cv2.normalize()` 함수 사용법 소개

### 9. histo_rgb.py  
- RGB 각 채널별로 히스토그램 평활화 적용  
- 채널별 이미지 개선 효과 비교

### 10. roi.py  
- 이미지 내 관심 영역(Region Of Interest, ROI)을 지정하여 처리하는 기본 예제

### 11. roi_copy.py  
- ROI를 복사하여 별도의 이미지로 추출하는 방법 실습

### 12. roi_crop_mouse.py  
- 마우스 이벤트를 이용해 이미지에서 직접 ROI를 선택하는 예제  
- 사용자가 마우스로 드래그하여 관심 영역 지정 가능

### 13. roi_select_img.py  
- ROI 선택 후 선택한 영역에 대해 다양한 이미지 처리 적용 예제

### 14. threshold.py  
- 임계처리(Thresholding)를 활용한 이진화 예제  
- 다양한 임계 처리 방식과 그 효과 설명

### 15. video_cam.py  
- 웹캠을 이용한 실시간 영상 캡처 및 화면 출력  
- OpenCV `VideoCapture`와 `imshow` 활용

---

## 실행 환경 및 준비

- Python 3.x 권장  
- OpenCV 라이브러리 설치 필요:  
  ```bash
  pip install opencv-python
  pip install opencv-contrib-python
