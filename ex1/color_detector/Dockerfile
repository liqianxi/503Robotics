FROM duckietown/dt-duckiebot-interface:daffy-arm64v8

WORKDIR /color_detector_dir

COPY requirements.txt ./

RUN pip install -r requirements.txt
ENV "N_SPLITS" 10
ENV "BINS" 10
ENV "MAX" 5

COPY color_detector.py .

CMD python3 ./color_detector.py