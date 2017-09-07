# DeepSense
Tensorflow 1.1 implementation for the paper:

Yao, Shuochao, et al. "Deepsense: A unified deep learning framework for time-series mobile sensing data processing." Proceedings of the 26th International Conference on World Wide Web. International World Wide Web Conferences Steering Committee, 2017.
	
## The preprocessed dataset of HHAR task
https://www.dropbox.com/s/z7zpnwh2ndthd2n/sepHARData_a.tar.gz?dl=0

------

## Updated by zhezh(2017-09-07):

This modified version boosts training speed over 10 times by using a tfrecord file (stored in SSD partition) instead of seperate files.

### Changes:
- Changed data input pipeline to use tfrecord instead of seperate files. This saves storage and improve IO effiency.

### Data preprocessing:
- Download the dataset provided by original developer and unzip the archive file.
- Modify lines tagged 'todo' to your data folder path
- Run 'har_tfrecord_util.py' to generate tfrecord
- Run 'deepSense_HHAR_tf.py' to train

