FROM stellargroup/phylanx:devel

RUN apt-get update
RUN apt-get install -y python-pip

WORKDIR /
RUN git clone https://github.com/hdc-arizona/traveler-tree
RUN pip install --upgrade pip
RUN pip install wheel
RUN pip install -U Flask
WORKDIR /traveler-tree
CMD python tree.py static/20180713_als_tree.txt static/20180713_als_perfdata.csv static/als_csv_instrumented.cpp
