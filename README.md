# LGQN

LGQN: LLM-Generated Queries from Narrations




> The task of localizing segments of extensive egocentric videos that correspond to natural language queries (NLQ)
> enables diverse applications in augmented reality and robotics. This approach assists humans in daily tasks by enhancing
> memory and providing answers based on everything an individual has observed. However, the task is technically
> challenging and costly due to the resources required to gather a sufficient number of (video, query, answer-timespan)
> pairs.This paper introduces a novel approach called “LLM-Generated Queries from Narrations” (LGQN), which leverages
> existing narrations to generate corresponding queries using Large Language Models (LLMs). This strategy enhances the
> training dataset with focused queries, thereby improving the overall training process. Additionally, we explore and
> modify the VSLNet
> model,a state-of-the-art model tailored for this task, to identify optimized configurations. Through extensive
> experiments, we demonstrate that pretraining with LGQN performs comparably to using standard narrations. We also
> analyze the impact of different training components on the model’s performance, providing valuable insights into the
> effectiveness of our approach.
> 
![main_struct_v2.drawio.png](..%2F..%2F..%2F..%2FUsers%2Finspi%2FOneDrive%2FDesktop%2Fimages%2Fprocessed%2Fmain_struct_v2.drawio.png)
 The proposed architecture for LGQN involves a data-augmentation strategy where textual narrations and corresponding video
spans are used. Narrations are processed through Llama 3 to generate queries. These queries are then aligned with the corresponding
video segments. Both the video segments and generated queries are passed through a query-guided highlighting model(see left). The
model predicts the temporal windows (see right) where the query-related activity occurs, enhancing the training data and improving model
performance .


