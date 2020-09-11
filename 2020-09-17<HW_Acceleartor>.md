# Intro(밑밥)
- 2020.07 ~ 2020.08
- [유민수 교수님 연구실](https://sites.google.com/view/kaist-via), 이윤재 조교님
- 매주 1회 줌미팅
- 딥러닝(중에서도 특히 CNN) 공부 1달
  - cs231n
- 나머지 논문 읽기 1달

<br>

# Papers
다 읽은 건 아니구, vDNN이랑 TensorDIMM정도는 열심히 읽었습니다! 나머지는 다른 설명 자료들 참고하는 정도...??
- ### **vDNN**: Virtualized Deep Neural Networks for Scalable, Memory-Efficient Neural Network Design
  - https://arxiv.org/abs/1602.08124
- ### **TensorDIMM**: A Practical Near-Memory Processing Architecture for Embeddings and Tensor Operations in Deep Learning
  - https://arxiv.org/abs/1908.03072
- ### **DianNao**: a small-footprint high-throughput accelerator for ubiquitous machine-learning
  - 가속기 논문의 시발점이라 할 수 있다고 하네요!
  - http://novel.ict.ac.cn/ychen/pdf/DianNao.pdf
  - 읽기는 어렵습니다 ^^
- ### **Eyeriss**: An Energy-Efficient Reconfigurable Accelerator for Deep Convolutional Neural Networks
  - https://ieeexplore.ieee.org/document/7738524
  - v1, v2
  - Would be better to refer:
    - https://eyeriss.mit.edu/
    - https://www.youtube.com/watch?v=brhOo-_7NS4
  - Reference가 가장 많았던 논문 
- ### **EIE**: Efficient Inference Engine on Compressed Deep Neural Network
  - https://arxiv.org/abs/1602.01528
  - Song Han 교수님 => 시리즈물인듯?
- ### 느낀점:
  - **Memory Access** is important....!!!!

<br>
<br>

# Other Useful Resources
- Hardware for Machine Learning: Challenges and Opportunities
  - https://arxiv.org/pdf/1612.07625.pdf
- Youtube channel; EEMS Group - PI:Vivienne Sze
  - https://www.youtube.com/channel/UC8cviSAQrtD8IpzXdE6dyug
  - 
- IC Design Education Center - IDEC
  - 김주영 교수님, 머신러닝을 위한 하드웨어 가속 (1~3)
    - 이번 저널클럽 준비의 MVP!!!
  - 1편: 딥러닝에 관한 소개
    - https://www.youtube.com/watch?v=tDxA3VT5kzY
  - 2편: DianNao, Eyeriss, EIE, Unpu
    - https://www.youtube.com/watch?v=95gxMOotYRc
  - 3편: TPU, GPU 등등... (아직 안 봐서 모르겠어요오)
    - https://www.youtube.com/watch?v=z1gBnr6NdoQ&t=156s
- 읽어야지~ 했던거
  - [White Paper on AI Chip
Technologies](https://www.080910t.com/downloads/AI%20Chip%202018%20EN.pdf)
      - 2018년꺼라 요즘 트렌드랑 맞는지는 모르겠네요
- 논문 읽는 법 몰랐을 때 노션에 정리하면서 읽던거
  - [Hardware for Machine Learning: Challenges and Opportunities](https://www.notion.so/woojinnn/Hardware-for-Machine-Learning-Challenges-and-Opportunities-e96d7b4f20214c9da7c2a2a50aa1bc6c)
  - [vDNN](https://www.notion.so/woojinnn/vDNN-Virtualized-Deep-Neural-Networks-for-Scalable-Memory-Efficient-Neural-Network-Design-0fce5cbb1945424895db7517bc842fb5)
  - [TensorDIMM](https://www.notion.so/woojinnn/TensorDIMM-A-Practical-Near-Memory-Processing-Architecture-for-Embeddings-and-Tensor-Operations-in--b720b103624143a5813e256953c7947d)
<br>
<br>
# Discussion
- CNN 말고 다른것들...??
  - 찬연님이랑 얘기했을 때, RL, GNN 등등...
  - 위에 논문들 대부분 AlexNet, VGG 이런애들로 테스트 하길래 다른 분야에서도 잘 먹히는 것인가???
  - 다른 분야에서는 어떤 부분이 Bottleneck? How?
  - 주제는 어떻게 찾는 건가요???