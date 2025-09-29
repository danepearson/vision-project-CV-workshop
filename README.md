# Computer Vision workshop for Vision Team at UCSC  📷 👨‍💻
This workshop will cover some simple classical single-object and more robust multi-object tracking algorithms.

### What you will need installed: 
- Python 3.11
- NumPy 1.26.x (must be less than 2.0 because pandas + scikit-learn don’t support NumPy 2 yet)
- opencv-python 4.9.0.80 (best with NumPy 1.26)
- ultralytics 8.3.x
- torch 2.5.0
- torchvision 0.20.0
- deep-sort-realtime 1.3.2

Install these as such:
```
python3.11 -m venv workshop-environment
source workshop-environment/bin/activate  (or venv\Scripts\activate on Windows)

pip install "numpy<2" \
            "opencv-python<4.10" \
            "opencv-contrib-python<4.10" \
            ultralytics==8.3.203 \
            torch==2.5.0 torchvision==0.20.0 torchaudio==2.5.0 \
            deep-sort-realtime==1.3.2
```
