# csee4121
If the graphs do not show up, please refer to this link:
https://github.com/siqihe41099/csee4121/blob/main/README.md

### Question 1
The default blocksize used by HFDS is 128 MB.
The default replication factor of HDFS on Dataproc is 3.

### Question 2 <img width="534" alt="Screen Shot 2022-04-30 at 11 39 53 PM" src="https://user-images.githubusercontent.com/92268046/166131201-e543dda5-cdda-4894-8126-109a74df50ac.png">
The completion time of the task is 5 min 5 sec.


### Question 3
<img width="622" alt="Screen Shot 2022-04-30 at 11 41 23 PM" src="https://user-images.githubusercontent.com/92268046/166131236-ffe8409b-8e72-42ae-a200-83a6321b29ce.png">
The completion time of the task is 4 min 9 sec. The performance is getting better in terms of completion time. Since in this question, we applied 3 node cluster (2 worker nodes) instead of a Single Node cluster. It means that more nodes to process at the same time, so it redues the competion time of the task.

### Question 4
<img width="552" alt="Screen Shot 2022-04-30 at 11 49 43 PM" src="https://user-images.githubusercontent.com/92268046/166131431-19847905-3855-40fe-bd2b-7153328b363c.png">
The completion time of the task is 2 min 59 sec. The performance is getting better in terms of completion time. Since in this question, the text file is small so that a comparatively small blocksizr is more suitable for this task. 

### Question 5
<img width="543" alt="Screen Shot 2022-04-30 at 11 52 05 PM" src="https://user-images.githubusercontent.com/92268046/166131486-be94ef11-73bc-414e-9a22-17cc95ec389a.png">
The completion time of the task is 33 min 48 sec.
Then killed one of the worker nodes immediately.
<img width="543" alt="Screen Shot 2022-05-01 at 12 16 58 AM" src="https://user-images.githubusercontent.com/92268046/166131999-abfe0d37-e197-46d8-bf83-ddc6c7290b47.png">
The job is still finished. The completion time of the task is 1 hr 6 min. The performance is getting worse in terms of completion time, becasue one worker node is lost. 


### Question 6
<img width="613" alt="Screen Shot 2022-04-30 at 11 57 18 PM" src="https://user-images.githubusercontent.com/92268046/166131596-05fc8601-91cc-410f-8594-9eb3394deca5.png">
The completion time of the task is 34 min 8 sec. The performance is getting worse in terms of completion time compared to question 5 without killing one work node. In this question, we set dfs.replication from default to 1. Having replication factor of more than 1 results in more parallelization, which means that having multiple copies of data at multiple places and all the machines can simultaneously process data. Therefore, the performance would be better when we have replication factor of more than 1.

### Question 7
<img width="586" alt="Screen Shot 2022-05-01 at 12 56 43 AM" src="https://user-images.githubusercontent.com/92268046/166132776-ae2012e6-ba65-47a6-bf36-9cd2dcae89e3.png">
The completion time of the task is 33 min 38 sec. The performance is getting slightly better in terms of completion time, and its time is 10 sec less than the performance of question 5 without killing one work node. In general, the larger the blocksize, the less the completion time is. However, if the size of a file is small, then smaller blocksize is better. In this question, The file may not be large enough, so 64GB blocksize works well.


