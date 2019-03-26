I have used the CRNN implemented [here](https://github.com/Belval/CRNN) to complete this task. 

To train the model, cd into the CRNN directory and use the following command:

`python run.py --train -ttr <Train-test ratio> -m <The path where the model will be saved> -ex <The path to the file containing the training samples, i.e, generated text images> -bs <Batch size> -it <Iteration count/ Number of epochs>` 

To test the model stored in save directory, cd to the CRNN directory and use the following command:

`python run.py --test -ex <The path to the file containing the testing samples> -bs <Batch size> --save_test_img --restore`

Note: The argument save_text_image enable to save text image with predicted output of CRNN as name of the image. This would be useful for analysis of output. 
