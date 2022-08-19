# caffe
## caffe object classification from webcam with go

 What it does:

 This example uses the Caffe (http://caffe.berkeleyvision.org/) deep learning framework
 to classify whatever is in front of the camera.

 Download the Caffe model file from:
 http://dl.caffe.berkeleyvision.org/bvlc_googlenet.caffemodel

 Also, you will need the prototxt file:
 https://raw.githubusercontent.com/opencv/opencv_extra/master/testdata/dnn/bvlc_googlenet.prototxt

 And the words text file with the descriptions:
 https://raw.githubusercontent.com/opencv/opencv/master/samples/data/dnn/classification_classes_ILSVRC2012.txt

 How to run:

 		go run ./cmd/caffe-classifier/main.go 0 ~/Downloads/bvlc_googlenet.caffemodel ~/Downloads/bvlc_googlenet.prototxt ~/Downloads/classification_classes_ILSVRC2012.txt

		(~shift+end (if downloaded files are in the same folder as main.go))
		go run main.go 0 bvlc_googlenet.caffemodel bvlc_googlenet.prototxt classification_classes_ILSVRC2012.txt opencv cpu    


 You can also use this sample with the Intel OpenVINO Inference Engine, if you have it installed.

 		go run ./cmd/caffe-classifier/main.go 0 ~/Downloads/bvlc_googlenet.caffemodel ~/Downloads/bvlc_googlenet.prototxt ~/Downloads/classification_classes_ILSVRC2012.txt openvino fp16


![Clipboard02](https://user-images.githubusercontent.com/38920548/185664650-2bb51fdf-bd11-4e59-b1a8-369ff9c70a66.png)
![Clipboard01](https://user-images.githubusercontent.com/38920548/185664657-74d418db-404c-4ade-bcd4-f7103abd0f15.png)
