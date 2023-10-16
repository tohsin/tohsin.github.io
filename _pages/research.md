---
layout: archive
permalink: /research/
classes: wide
title: "Research Projects and Regular Projects"
author_profile: true

---
<div>
  <h2>DexCatch: Learning to Catch Arbitrary Objects with Dexterous Hands</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/dex.gif" alt="image-left" style="width: 200; height: 200px; margin-right: 10px;">
    <p>Achieving human-like dexterous manipulation re- mains a crucial area of research in robotics. Compared with static grasping, dynamic dexterous manipulation can achieve more efficient task execution. For example, the throw-catching behavior has the potential to increase picking speed without transporting objects to their destination. However, it poses a major challenge for stable control due to a large number of dynamic contacts. In this paper, we propose a Stability- Constrained Reinforcement Learning (SCRL) algorithm to learn to catch diverse objects with the hands facing upward and sideward. The SGRL algorithm outperforms baselines by a large margin, and the learned policies show strong zero- shot transfer performance on unseen objects. Remarkably, even though the object in a hand facing sideward is extremely unstable due to the lack of support from the palm, our method can still achieve a high level of success, 52.58%, in the most challenging task.
    </p>
  </div>
</div>
<div>
  <h2>NightMare Dreamer ( Releasing Soon )</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/eval_video_goal.gif" alt="image-left" style="width: 200; height: 200px; margin-right: 10px;">
    <p><strong>Abstract</strong>:We present a <strong>Model-based safe reinforcement learning (RL) algorithm </strong>that builds on the Dreamer work. Our approach to the problem involves <strong>multi-agent and hierarchical planning</strong>. We train two policies: a control agent whose objective is to solve the goal, and a safe agent that aims to mimic the control policy but limits the cost constraint. Both policies are learned purely from imagination. During environment interaction, the agent looks ahead and decides if it should switch to a safe policy under the control policy, leading to a safety guarantee. <strong>Top right Corner: Green is the Control Policy, Red is the time step agent detects violation and switches to Safe Policy</strong>
    </p>
  </div>
</div>

<div>
  <h2>Active Graph Slam and Exploration ( Currently Ongoing ) </h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="assets/images/pose graph.png" alt="image-left" style="width: 200; height: 200px; margin-right: 10px;">
    <p>
    Modern RL + Active SLAM methods don't attempt to solve the problem for modern SLAM techniques that use Graph SLAM. To address this and provide a framework for future agents to explore and reason about the world, we aim to leverage the graph structure itself as a reward signal. For example, the number of spanning trees in a graph is related to the entropy of the 'map uncertainty,' and the graph's Lagrangian can be used as an optimality criterion. We divide the task between a global and local actor to circumvent the issues that arise from RL applications in this domain, which tend to memorize the maps, making generalization difficult. One agent finds the best position to explore and other agent navigates to the point.
    Note: Finishing the work is challenging due to limited access to resources in Nigeria.
    </p>
  </div>
</div>

<div>
  <h2>SafeNeuroEvolution ( Currently Ongoing )</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/neuroevolution.png" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p><strong>Abstract</strong> We present a <strong>NeuroEvolution algorithm</strong> that leverages <strong>parallel computing</strong> and <strong>evolution strategies</strong> to pretrain safe agents without gradient descent.
    </p>
  </div>
</div>

<div>
  <h2>ALAC : Constrained Model-Free Reinforcement Learning with Finite-Time Stability Guarantee</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/Lyapunov.png" alt="image-left" style="width: 300px; height: 200px; margin-right: 10px;">
    <p><strong>Abstract</strong>: Model-based control methods have achieved impressive performance 
        on a large variety robotic tasks over the past few decades. Then recently,
        due to eliminating the difficulty of modeling and parameter-tuning, 
        model-free reinforcement learning (RL) methods perform better under some complex scenarios.
        However, the lack of stability guarantee, which affects the interpretability of the contorl system,
        remains a significant difference in contrast to traditional methods.
        Therefore, we propose a Lyapunov-based actor-critic method that guarantees the stability 
        of control system. Interestingly, we introduce the data-driven stability condition that meets 
        the demand of finite-time stability convergence. Furthermore, the Lyapunov critic function is
        conducted by a constrained neural network, thus making some necessary conditions satisfied naturally. 
        Experimental results demonstrate our approach achieves lower cost and faster convergence rate
        compared with previous studies.
    </p>
  </div>
</div>


<div>
  <h2>TURBOGrad</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/torch_image.jpeg" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p>Called turbo not because its fast but because its a mini Pytorch, well sorta.
        Repo was adapted from andrej kaparthy, but modified to solve RL tasks providing an overall
        framework for people to learn both RL and pytorch and how to implement these algorithms,
        It also includes many other features not included in Andrej work like other optimisers
        (ADAM, RMSProp) and detach functions etc. Have fun and dont forget to call `zero_grad()` before backward.
    </p>
  </div>
</div>


<div>
  <h2>SAFE PANDA GYM</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/push_safe.png" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p><strong>Abstract</strong>: A modification to the original Panda Gym environment for the development
        and experimentation of Safe-RL algorithms by adding more complex tasks and Constraints 
        to the environment for agents to learn both safe and optimal policies by minimizing cost functions.
        <a href="https://github.com/tohsin/Safe-panda-gym.git">Github Link</a>
    </p>
  </div>
</div>

<div>
  <h2>SpaceRobotEnv (Tsinghua-Space-Robot-Learning-Group)</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/ral.png" alt="image-left" style="width: 300px; height: 200px; margin-right: 10px;">
    <div>
      <p>SpaceRobotEnv is an open-sourced environment for trajectory planning of free-floating space robots.
        Different from the traditional robot, the free-floating space robot is a dynamic coupling
        system because of the non-actuated base.
        Therefore, model-based trajectory planning methods encounter many difficulties in modeling 
        and computing.
      </p>
      <p>Contributions include:</p>
      <ul>
        <li>SpaceRobotEnvPointCloud-V0: an environment version of SpaceRobotEnv with point cloud used as the observation.</li>
        <li>Reinforcement learning algorithms implementation and experimentations on different models and performance comparisons (PPO, SAC, DDPG, TRPO)<a href="https://github.com/Tsinghua-Space-Robot-Learning-Group/SpaceRobotEnv.git">Github Link</a></li>
      </ul>
    </div>
  </div>
</div>


<div>
  <h2>2D Localisation and SLAM</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/2dslam.png" alt="image-left" style="width: 300px; height: 200px; margin-right: 10px;">
    <div>
      <p>My implementation of probabilistic robotics algorithms and assignments from introduction to mobile robotics
        project includes algorithms for localization and SLAM like Particle Filter, Kalman Filter, EKF, and 
        a capstone implementation of graph SLAM in a 2d Pygame simulator.
      </p>
      <ul>
        <li>Backend optimizes a pose graph generated from moving the robot in the simulator using Gauss Netwon with Schur trick for optimization.</li>
        <li>Frontend Implements an Iterative closest point for the simulated point cloud and the user has to guide robot to the start point for loop closure<a href="https://github.com/tohsin/Localisation_and_Slam_algorithms_implimentation.git">Github Link</a></li>
      </ul>
    </div>
  </div>
</div>


<div>
  <h2>Visual Slam and Visual Slam Python</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/vslam.png" alt="image-left" style="width: 300px; height: 150px; margin-right: 10px;">
    <p>Implemented several concepts in Visual SLAM using Lie algebra and Lie groups (SE3),
        including visual odometry, optical flow, bundle adjustment, pose graph, loop closure,
        sliding window, and dense reconstruction using Gauss-Newton or g2o for optimization. 
        The Visual SLAM Python repository serves as a prototype for Visual SLAM concepts using Python wrappers for g2o,
        pangolin, etc. <a href="https://github.com/tohsin/visual-slam-python.git">Visual slam Python</a> 
        <a href="https://github.com/tohsin/visual-slam.git">Visual slam C++</a> </p>
  </div>
</div>

<div>
  <h2> Tomato harvesting Soft Robotic arm (Research Assistant)</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <div>
      <p>Joined a team of 3 with a graduate student to design and implement a  cost-effective soft robotic arm to be used for 
        harvesting Tomatoes on a farm.
      </p>
      <ul>
        <li>Using a vacuum pump, Cassava, and rubber as the components for the soft arm grabbing actuator.</li>
        <li>Trained YOLO algorithms to identify types of tomatoes as well as assess the state of fruit (Ripe/ Unripe) </li>
        <li>Deploy project on a Raspberry PI with a camera attached and use Serial connection with an Arduino for control of the joints and gripper actuator </li>
        <li>Simulated manipulator forward and inverse kinematic motions using python robotics toolbox.</li>
      </ul>
    </div>
  </div>
</div>


<div>
  <h2>LOUISE - A Medical CHATBOT </h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/rasa1.jpg" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p>Designed and developed a medical chatbot that suggests emergency diagnoses based on symptoms reported by users. 
        Our chatbot uses a unique approach that avoids the need for large datasets of intents for training, 
        making it more efficient and scalable. The chatbot features a backend with two separate models - a support vector machine for 
        categorizing health problems based on symptoms, and a transformer model for detecting symptoms as intents. By using several similarity algorithms,
        we are able to map the right symptoms to the appropriate diagnoses.
        This approach allows us to avoid the time-consuming process of manually writing a large number of intents to map symptoms to diagnoses. <a href="https://github.com/tohsin/rasaSymptomChatBot.git ">Github Link</a>
    </p>
  </div>
</div>

<div>
  <h2>CxrCovidClassify - Double Transfer learning for Covid Prediction on Mobile Devices</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/screens.png" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p>We show the use of Double Transfer learning, The neural Net was first trained on a large dataset of X-rays on pneumonia 
        so neural net learns the structure of Xray images and the finally trained on Covid Xray data set.
        Due to compatibility and optimisation, Mobile net was the pre-trained model to allow easy quantisation to deploy on a 
        mobile device with tensor flow lite. <a href="https://github.com/t-regbs/CxrCovidClassify.git">Github Link</a>
    </p>
  </div>
</div>

<div>
  <h2>Electronic Car Ignition using Face Recongnition </h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <p>Development of a portable device to work with cars for car owners to start engines using face recognition,
        the application comes with a GUI and LCD and is developed to run optimally on a raspberry pi with motors 
        attached to simulate car engine starting. <a href="https://github.com/tohsin/face_recognition_to_start_engine.git">Github Link</a>
    </p>
  </div>
</div>


<div>
  <h2>Car Monitoring OBD2-Mobile</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/obd.jpeg" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p>A portable device working with an OBD device, the OBD is connected to cars providing real-time data and in some cases
        diagnosis to users remotely on their mobile devices. The OBD2 remotely connects to a Raspberry Pi that
        then publishes information to the user website or mobile device.
    </p>
  </div>
</div>

<div>
  <h2>IOT Remote Farm monitoring</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <p>Development of an IoT solution for farmers to monitor some properties of their farms remotely using a collection of 
        sensors suite with real-time connection to a web API that works with an IOS Mobile application and also includes and
        automatic sprinkler if soil humidity drops to a certain threshold.
    </p>
  </div>
</div>

<div>
  <h2>Remote Repogrammable Robotic Arm (Final Year Project)</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/robarm.png" alt="image-left" style="width: 300px; height: 200px; margin-right: 10px;">
    <div>
      <p>Development of a remote solution to programming robot arms. A mobile application that 
        remotely connects to the robotic arm and offers two modes one two directly actuate the arm and 
        one to program and save a sequence of tasks so one robot can be adapted and switched to different
        task easily.
      </p>
      <ul>
        <li>3D Modelling was done with SOLIDWORKS and arm was made of arcylic materials.</li>
        <li>Arm uses Raspberry and an arduino for control and WI-FI connection for remote control.</li>
      </ul>
    </div>
  </div>
</div>


<div>
  <h2>Robot Receptionist Concept Design ( Group Project )</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <p>Concept design for robot receptionist during the Covid 19 period to provide a tour for 
        users visiting the mechanical Engineering building. 
        We explore the CAD design of the robot, the use of active Rfid for localization,
        use pre-recorded audio for conversation with humans and a language model for intent detection.
    </p>
  </div>
</div>
