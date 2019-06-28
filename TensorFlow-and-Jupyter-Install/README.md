# 텐서플로와 주피터 노트북 설치

1. 우선 파이썬을 설치해야합니다. (윈도우에서는 반드시 파이썬 3.5 이상, 64 비트용 사용)

   https://www.python.org/downloads

2. 터미널 또는 윈도우의 명령 프롬프트에서 텐서플로 설치

   ```
   pip3 install --upgrade tensorflow
   ```

   * NVIDIA GPU를 사용하고 있다면, GPU 가속을 지원하는 텐서플로 설치 가능

     ```bash
     pip3 install --upgrade tensorflow-gpu
     ```

3. 라이브러리 설치

   ```
   pip3 install numpy matplotlib pillow
   ```

   * Numpy : 수치 계산 라이브러리
   * Matplotlib : 그래프 출력 라이브러리
   * pillow : 이미지 처리 라이브러

4. 텐서플로 실행해보기

   ```bash
   C:/> python3 (Enter)
   >>> import tensorflow (Enter)
   ```

5. 주피터 노트북 설치

   ```
   pip3 install jupyter
   ```

6. 주피터 실행

   ```
   jupyter notebook
   ```