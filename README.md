# Academic English : 논문에서 나온 표현을 정리해보자

# Reference Table

1. ResNet strikes back : An improved training procedure in timm  
2. Self-Attention With Relative Position Representations
3. Rethinking and Improving Relative Position Encoding for Vision Transformer
4. Person Re-Identification with a Locally Aware Transformer
5. Stronger Baseline for Person Re-identification
6. Self-Supervised Pre-Training for Transformer-Based person Re-identification
7. TransReID : Transformer-based Object Re-Identification
8. UniformFace : Learning Deep Equidistributed Representation for Face Recognition
# Groups

## *Abstract*

1. The influential Residual Networks remain the gold-standard architecture in numerous scientific publications.[1]
    - 기존의 네트워크가 다양한 분야에서 매우 좋은 표준이 되어왔음을 표현  
    - 동사 Remain과 함께 gold-standard 라는 표현을 사용
2. They typically serve as the default architecture in studies, or as baselines when new architectures are proposed.[1]
    - 여러 연구의 baseline이 되어왔다  
    - serve as the default architecture
3. Yet there has been significant progress on ~[1]
    - 지금까지 ~에 매우 많은 발전이 있었음을 표시 
    - Yet을 이렇게도 쓴다
4. ~ have increased the effectiveness of the training recipes.[1]
    - Training recipe (Hyperparameter, method의 setting)의 효율을 증가
    - 무언가의 효율을 증가시켰다는 표현을 쓸때 have increased the effectiveness of ~
5. We share competitive training setting and pre-trained models[1]
    - 성능이 우수한 setting과 model을 open한다  
    - 동사 share, 형용사 competitive 로 의미를 전달
6. With the hope that they will serve as better baselines for future work[1]
    - 공개된 model들이 후속 연구에 더 좋은 baseline으로 쓰이길 바라면서~   
    - With the hope that, serve as
7. Relying entirely on an attention mechanism, ~[2]
    - Transformer가 attention mechanism 만으로 학습이 이루어짐을 entirely rely O 로 표현
8. General efficacy has been proven in natural language processing.[3]
    - General efficacy has been proven
        - 특정 영역에서 일반적인 효용성이 입증됨을 표현
9. However, in computer vision, its efficacy is not well studied and even remains controversial, e.g whether relative position encoding can work equally well as absolute position?[3]
    - not well studied and even remains controversial
        - 잘 연구되어지지 않았음을 remains controversial 이란 표현을 사용
    - work equally well 
        - "제 역할을 동등하게 수행하는가?" 의 뉘앙스를 사용
10. S can be easily plugged into O[3]
    - S(method)가 O(모델)에 쉽게 추가될 수 있음을 표현
11. Experiments demonstrate that solely due to the proposed encoding methods, DeiT and DETR obtain up to 1.5%(top-1 Acc) and 1.3%(mAP) stable improvements over their original versions on ImageNet and COCO respectively, without tuning any extra hyperparameters such as learning rate and weight decay.[3]
    - Hyperparameters의 변경 없이 오직 method의 변경만으로 실험 성능을 높였음을 표현할 때
    - Solely due to
         - 전적으로 ~에 의해
12. Our ablation and analysis also yield interesting findings, some of which run counter to previous understanding[3]
    - yield 
        - ~을 알아냈음을 나타낼 때 (find의 대체어)
    - run counter to
        - ~에 반대하여
13. Extracting robust feature representation is one of the key challenges in object re-identification(Re-ID).[7]
## *Introduction*

1. We have witnessed significant advances in image classification, as reflected by ~[1]
    - ~의 영향을 받아 image classification task에 매우 큰 발전이 있어왔음을 표현  
    - We have witnessed, significant advances, as reflected by~
2. Several good practices exist to mitigate N, like measuing the standard deviation with different seeds, ~[1]
    - 후술할 내용들을 위해 기존에 수행되었던 몇가지 방법들을 열거하는 방식  
    - Several good practices exist to ~
3. Putting aside N, measuring progress on A or T poses a challenge as both A and T progress over time.[1]
    - N은 제쳐두고, A 와 T를 진행상황에 따라 측정하는 것에는 어려움이 따른다는 표현  
    - Putting aside ~: 제쳐 두고, poses a challenge : 어려움이 따른다(의미상)
4. When optimizing jointly over (A,T), there is no guarantee that the choice T for a given architecture A remains the best for another model design A2.[1]
    - A와 T를 동시에 최적화 할때 model A에서의 choice T가 다른 모델인 A2에서도 최선의 선택일 것이라는 보장이 없다.  
    - When optimizing jointly over (A,T) : ~을 공동으로 최적화할때 , There is no guarantee that , ~ remains : ~할 것이라는 보장이 없음
5. ~, one may implicitly,favor one model over another[1]
    - 특정 모델이 (암묵적으로) 선호되어질수 있다.  
    - Implicitly favor이 주는 어감을 기억
6. Recent approaches typically leverage O 
    - 최근의 연구들은 전형적으로 O에 집중되어있다.
7. One common approach is to use position encodings which are combined with input elements to expose position information to the model[2]
    - 모델에게 patch의 위치정보를 주는 APE라는 일반적인 방법에 대한 기술
    - summation 대신에 combined with으로 표현
    - Expose 라는 동사로 모델에게 정보를 전달하는 것을 표현
8. Convolutional neural networks inherently capture relative positions within the kernel size of each convolution.[2]
    - Inherently capture 이란 표현으로 model의 nature를 표현
    - capture O within ~ : ~로써 O를 파악
9. For the Transformer, which employs neither convolution nor recurrence, incorpoating explicit representations of position information is an especially important consideration since the model is otherwise entirely invariant to sequence ordering.[2]
    - which employs neither convolution nor recurrence
        - 동사 employ의 사용 : make use of it
    - incorpoating explicit representations of position information
        - incorporate
        - position 에 대한 직접적인 정보를 제공하는 것
    - is an especially important consideration
        - 중요성의 명사화
    - is otherwise entirely invariant to sequence ordering
10. Our approach can be cast as a special case of extending the self-attention mechanism of the Transformer to considering arbitrary relations between any two elements of the input, a direction we plan to explore in future work on modeling labeled, directed graphs.[2]
    - S can be cast as a speical case of ~
        - S 는 ~의 특별한 경우로 여겨질 수 있다.
    - considering arbitrary relations between any two elements of the input 
        - Input의 두 element의 관계를 고려하는~
11. Transformer recently has drawn great attention in computer vision because of its competitive performance and superior capability in capturing long-range dependencies[3]
    - 첫 문장의 impact
    - ~ has drawn great attention in computer vision
        - Computer vision 영역에서 굉장한 관심을 얻었음을 표현
    - competitive performance and superior capability
    - capturing long-range dependencies
12. There are mainly two classes of methods to encode positional representations for transformer.[3]
    - There are mainly two classes of methods to ~
        - 주로 두가지 방법을 사용한다~의 표현
13. The core of transformer is self-attention, which is capable of modeling the relationship of tokens in a sequence.[3]
    - The core of A is B : A의 핵심 아이디어는 B이다.

14. There are mainly two classes of methods to encode positional representations for transformer.[3]
    - There are mainly n classes of methods to~
        - 어떤 주제의 굵직한 접근방식을 나열하기 전에 사용하기 좋음

15. However, in computer vision, the efficacy is still unclear.[3]
    - still unclear
    - remains controversial의 느낌으로 사용

16. There are few recent works shedding light on it, but obtaining controversial conclusions in vision transformers.[3]
    - 몇몇 연구들이 진행되었음을 sense 있게 표현...
    - 이런 표현은 어떻게 쓴거지 진짜

17. For example, ~ observed that the relative position encoding does not bring any gain comparing to the absolute one.[3]

18. It is unclear that : Whether the naive extension from 1D or 2D is suitable for vision models; whether the directional information is important in vision task?[3]
    - 질문형 문장을 이어나가는 방식
    - That 이후 wheter 문을 쓰는 것이 깔끔하게 떨어진다.
## Re-ID Introduction

1. Person Re-identification is an important problem in computer vision-based surveilance applications, in which the same person is attempted to be identified from surveillance in a variety of nearby zones.[4]
    - be attempted to be identified from ~ 
    - in a variety of ~ 
2. Person Re-ID is a predominantly considered as a feature embedding problem[4]
    - predominantly considered as ~ : ~로 간주된다.
3. Person re-identification(re-ID) aims to identify the same person of interest across non-overlapping capturing cameras, which plays an important role in visual surveillance applications and computer vision research areas.[5] 
    - aims to ~ 
    - plays an importabt role
4. It aims at locating and recognizing a person of interest across multiple non-overlapping cameras in various spots.[5]

5. This work targets to mitigate the gap between the pre-training and ReID datasets from the perspective of data and model structure, respectively[6]
    - S targets to mitigate O : S는 O를 통합하는 것을 목적으로 한다.
    - from the perpective of ~ : 의 관점에서 

6. Object re-identification(Re-ID) aims to associate a particular object across different scenes and camera view, such as in the applications of person ReID and vehicle ReID.[7]
    - ~ aims to associate O across different scenes and camera view

7. Extracting robust and discriminative features is a crucial component of ReID, and has been dominated by CNN-based methods for a long time.[7]
    - S is a crucial component of O
    - Has been dominated by O

## Related work

1. The Transformer employs an encoder-decoder structure, consisting of stacked encoder and decoder layers[2]
    - S employs O
        - Model이 어떤 구조를 사용함을 표현할때 
    - ~, consisting of stacked encoder and decoder layers
        - 구조가 어떤 요소들로 이루어졌음을 나타내고자 할때 consisting of~ 
2. Self-attention followed by a position-wise feed-forward layer[2]
    - ~ followed by
        - Layer의 선후관계를 표현하며 설명할 때 사용
3. To form the sublayer output, results from each heads are concatenated and a parameterized linear transformation is applied.[2]
    - MHSA에 대한 설명 방식

4. This property is shared by our relative position representations which, in contrast to absolute position representations, are invariant to the total sequence length[2]
    - is shared by
        - 특성이 공유된다는 말을 통해, 특성이 내재되어있음을 표현
    - ~, are invaraint to the total sequence length
        - sequence 에 대해 total sequence length라는 표현

5. In this fashion, the pairwise positional relation is learned during transformer training.[3]
    - 이런 방식으로, pairwise의 위치관계가 transformer의 학습과정에서 학습된다.
    - In this fashion : 이런 방식으로~ 

## Proposed methods

1. We employ the simultaneous supervision of A-Softmax loss and uniform loss to learn discriminative and equidistributed features as follows[8]
    - Employ the simultaneous supervision of ~ : 제안한 loss를 기존 loss와 통합하여 씀을 이와 같이 표현
## Experiments

## Ablations

1. The experiments include an ablation study to analyse the effectiveness of the ideas introduced in the proposed approach.
    - 깊게 고민하지 말고 ablation study에 대해 명료하게 설명

## Conclusion 

- 요약을 하는것이 아닌 연구의 의미의 전망을 적는것!
- 논문의 Conclusion 부분을 모아 유심히 읽으면 감이 빨리 온다.

- The abundant experiments show that our methods bring a clear improvement on both classification and detection tasks with negligible extra complexity.[3]
    - abundant experimenst
    - our methods bring a clear improvement on ~

- Our method could be easily plugged into the self-attention modules in vision models.[3]
    - could be easily plugged into ~
- In addition, we give comparison of different methods and analysis on relative position encoding with following conclusions.[3]
    - give comparison of different methods~

- In future works, we plan to extend our method to other attention-based models and scenarios, such as ~[3]
    - plan to extend our method to ~

- In this paper, we invesitgate a pure transformer framework for the object ReID task, and propose two novel modules.[7]

- The final framework TransReID outperforms all other state-of-the-art methods by a large margin on several popular person/vehicle ReID datasets.[7]
    - S outperforms O by a large margin 

- Based on the promising results achieved by TransReID, we believe the transformer has great potential to be further explored for ReID tasks.[7]
    - promising results achieved by ~
    - we believe the ~

- Based on the rich experience gained from CNN-based methods, it is in prospect that more efficient transformer-based networks can be designed with better representation power and less computational cost.[7]
    - rich experience 
    - in prospect that : ~을 예상하여

- In this paper we presented an extension to self-attention that can be used to incorporate relative position information for sequences, which improves performance for machine translation.
    - present an extension to ~ : 개념을 확장하는 의미로 사용

- For future work, we plan to extend this mechanism to consider arbitrary directed, labeled graph inputs to the Transformer.
    - plan to extend this mechanism

- For both of these extensions, a key consideration will be determining efficient implementations.
    - a key consideration : 주요 고려사항
    

## 숙어/기본 문장

1. benefits greatly from : ~로 부터 큰 혜택을 받다.

2. without requiring ~ : ~ 없이도
    - ex) Global feature learning benefits greatly from local feature learning, without requiring extra supervision.

3. introduce sth into ~ : sth을 ~에 반영(영향을 끼치는 상황을 만든다.)
    - ex) Occluded parts of the human body might introduce irrelevant context into the learned feature.

4. To explicitly overcome these drawbacks, ~ : 이러한 결점을 명시적으로 보완하기 위해

5. Recent studies have paid attention to ~ : 최근 연구들은 ~에 집중한다
    - ex) To explicitly overcome these drawbacks, recent studies have paid attention to part-based, local feature learning.

6. prevent A from B : A가 B하는 것을 막다
    - ex) The decoder uses masking in its self-attention to prevent a given output position from incorporating information about future output positions during training

7. However, both issues can be resolved by ~ : 언급된 issue(문제제기)들은 ~에 의해 해결될 수 있다.  
    - ex) However, both issues can be resolved by splitting the computation of equation into two terms.

8. Solely due to ~
    - 전적으로 ~만으로 

9. To alleviate this dilemma, : 이런 문제를 완화하기 위해~

10. To address this challenge, : 이런 문제를 다루기 위해~ (resolve)

11. To overcome these limitations : 이런 한계점을 극복하기 위해~

12. With respect to : ~에 관하여

13. Integrate 과 Incorporate의 차이 (통합하다) : 

    - 어떤 것이 다른 것과 integrate 된다고 할때 온전한 하나로 다시 형성되는 것을 의미
    - Incorporate는 어떤 것이 다른 것에 부분으로 포함되는 것을 의미

15. in order O to V : O가 V할수 있게 하기 위해

16. Adjust, apply , draw conclusion

17. For the sake of ~ : ~때문에, ~를 위해서
    - ~를 돕기 위해서, ~를 좋아해서 의 의미가 강하다.
    - 목적을 가진 뉘앙스로 쓰지는 않는다.

18. "포함"의 의미 
    - include : 전체가 여러개로 구분된 것들을 전체의 일부분으로 포함시키는 것, 상품이나 서비스가 어떠한 구성 요소를 포함하고 있음을 의미
    - contain : 대상 안에 내용물이 함유되어 있음을 의미
    - involve : 수반하다. 관련시키다. 참여시키다. 원인과 결과의 인관관계로 설명하는 뜻으로 제한되어 쓰임

19. "각각"
    - each
    - respective
    - individual

20. with respect to : ~에 대해

21. be equipped with : network가 어떤 구조적 요소들을 포함하고 있을때 자주 쓰인다.