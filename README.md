# DSTC8-AVSD Official
DSTC8-AVSD: Sentence generation task for Audio Visual Scene-aware Dialog 

## NEWS

You can evaluate your results using the following evaluation tool:

AVSD@DSTC8

https://drive.google.com/file/d/1EKfPtrNBQ5ciKRl6XggImweGRP84XuPi/view?usp=sharing


AVSD@DSTC7

https://drive.google.com/open?id=1nz9Pu9YIfuZHzowhASXERajRXqE6DBQx


April 1st, 2020: All data is now publicly available.

To let you submit a full paper (8 pages + citation) of your experiments to CVPR2020, we will accept an AVSD@DSTC8 workshop paper (2-3 pages + citation) which is a subset of the full paper for CVPR2020.

```
The submission of your system description to DSTC8@AAAI2020 is mandatory.
If you will not submit your paper to the DSTC8 workshop, 
you cannot submit any papers using the AVSD@DSTC8 data set until April 1st in 2020. 
```

### 1.  AVSD@DSTC8 Workshop paper (2-3 pages system description + 1page for citation):

Please use the following AAAI Author Kit:                     

https://www.google.com/urlq=https%3A%2F%2Fwww.aaai.org%2FPublications%2FTemplates%2FAuthorKit20.zip&sa=D&sntz=1&usg=AFQjCNHXkMmYCW9vh4GO1hHKCp12KAf-oA)

Please submit your paper to the following site:                     

https://www.google.com/urlq=https%3A%2F%2Fcmt3.research.microsoft.com%2FDSTC82020%2FSubmission%2FIndex&sa=D&sntz=1&usg=AFQjCNFX_OkwQGd5g2J8B9_6dGxPk8slUQ

### 2.  CVPR2020 paper (Full paper including 1 and more experiments and analysis)

Please use the following CVPR Author Kit:                    

http://cvpr2020.thecvf.com/sites/default/files/2019-09/cvpr2020AuthorKit.zip

Please submit your paper to the following link:                    

https://cmt3.research.microsoft.com/User/Login?ReturnUrl=%2FCVPR2020  


## Evaluation Resutls
The evaluation toolkit for AVSD@DSTC is now releasing to the challenge participants.
The human evaluation was done by 5 humans.
The objective evaluation was done and the results were released to the participants 10/21/2019 !

The data sets for AVSD@DSTC8 is only limited used by the participants who submitted the results to the official challenge.
If you got the data but not submitted your results to the challenge,
please hold your publishing your number for AVSD@DSTC8 until the data will be publicly available on April 1st, 2020.
Submission site is now open:

https://docs.google.com/forms/d/e/1FAIpQLSdZizy9H143VQ2nGihha38ncJVLLMMSP55zCT7ls5aeBNSy1A/viewform

Test sets are now Releasing!!! 

Submission format

Please fill your answers into __UNDISCLOSED__ below:

```
-----------------------------------------------------------------------------------------------------------
  "dialog" : [
              {
                 "answer" : "no and it is a window that he is standing in front of .",
                 "question" : "hello . did someone come to the door ?"
              },
              {
                 "answer" : "__UNDISCLOSED__",
                 "question" : "is he looking at something outside the window ?"
              }
           ]
----------------------------------------------------------------------------------------------------------
```

###
1. Please register the challenge from the following link:

   https://docs.google.com/forms/d/e/1FAIpQLScbTSq9P3d_o_2aK2IKvFmrEJ3-xdORspxNyt3NcQ3oiuA8Bw/viewform

2. You can find the test sets here: 

   https://drive.google.com/file/d/1IYAoCuaKDwzRJURArHh9MHU4HPRYdewo/view?usp=sharing

3. Please note that we cannot use the DSTC7 test sets for any purposes for DSTC8.

4. When you will submit the systems, please clarify training with or without the summary and caption.


###

"Any features" extracted from the given videos can be used at DSTC7 and DSTC8.

The multiple references for the DSTC7 AVSD test set in the following file:
https://drive.google.com/file/d/1nz9Pu9YIfuZHzowhASXERajRXqE6DBQx/view?usp=sharing


dstc7avsd_eval.tgz 

## - Track Description
Welcome to the follow-up challenge for Audio Visual Scene-Aware Dialog (AVSD) using Natural Language Generation (NLG) technologies of the successor of DSTC7-AVSD. This challenge is one of the track for the **8th Dialog System Technology Challenges (DSTC8) workshop.**
The task is to build a system that generates responses in a dialog about an input **video**.

### - Tasks

In this challenge, systems are required to generate responses to user input in the context of a given dialog.  
This context consists of a dialog history (previous utterances between both user and system) in addition to video and audio information that comprise the scene. 
The quality of a system response automatically generated will be evaluated using objective measures to see how good the generated responses are in terms of the naturalness and informativeness.

#### 1. Task 1: Video and Text 
    a. Use the video and text training data provided but no external data sources, 
       other than publicly available pre-trained feature extraction models.

       There are two options: with or without using the summary generated by the questioners after holding 10 QAs.

    b. External data may also be used for training.

#### 2. Task 2: Text Only 
    a. Do not use the input videos for training or testing. 
       Use only the text training data (dialogs and video descriptions) provided. 
    b. Any publicly available text data may also be used for training.
    
    
#### Validation data set:

Please train models using the training data set only.
You can tune the parameters using the validation set and confirm the performance of your systems using the DSTC7 test sets.
Notes: The official challenge doesn't allow you to use the DSTC7 test set to tune your models.

|               |    Training    |  Validation   |   DSTC7 Test  |
| ------------- | -------------- | ------------- | ------------- |
| # of Dialogs  |       7,659    |      1,787    |      1,710    |   
| # of Turns    |     153,180    |     35,740    |     13,490    |
| # of Words    |   1,450,754    |    339,006    |    110,252    |

*The number of turns for the test set is smaller than the validation
because they are not always full dialogs.

You can download the full official data set and the references for AVSD@DSTC7 from here:
https://drive.google.com/drive/folders/1SlZTySJAk_2tiMG5F8ivxCfOl_OWwd_Q?usp=sharing

1. **Text files:**
     - train_set4DSTC7-AVSD.json
     - valid_set4DSTC7-AVSD.json
     - test_set4DSTC7-AVSD.json

2. **Audio feature files:**
   - Training and validation data sets
     - vggish.tgz 
   - DSTC7 test set:
     - vggish_testset.tgz: 

3. **Visual feature files:**
   - Training and validation data sets:
     - i3d_flow.tgz 
     - i3d_rgb.tgz
   - DSTC7 test set:
     - i3d_flow_testset.tgz
     - i3d_rgb_testset.tgz

4. **DSTC7 evaluation setup**
   - dstc7avsd_eval.tgz


Although a new baseline system will be released soon, the old one is available from the following link:
https://github.com/dialogtekgeek/AudioVisualSceneAwareDialog

You can find more information in the following DSTC7-AVSD overview paper:
http://workshop.colips.org/dstc7/papers/DSTC7_Task_3_overview_paper.pdf

### - Contact Information
chori@merl.com

-- 
Chiori Hori
