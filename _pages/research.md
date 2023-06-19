---
layout: archive
permalink: /research/
classes: wide
title: "Research Projects and Regular Projects"
author_profile: true

---

<div>
  <h2>ALAC : Constrained Model-Free Reinforcement Learning with Finite-Time Stability Guarantee</h2>
  <hr>
  <div style="display: flex; align-items: center;">
    <img src="/assets/images/Lyapunov.png" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
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
    <img src="/assets/images/push_safe.png" alt="image-left" style="width: 200px; height: 200px; margin-right: 10px;">
    <p>Called turbo not because its fast but because its a mini Pytorch, well sorta.
        Repo was adapted from andrej kaparthy, but modified to solve RL tasks providing an overall
        framework for people to learn both RL and pytorch and how to implement these algorithms,
        It also includes many other features not included in Andrej work like other optimisers
        (ADAM, RMSProp) and detach functions etc. Have fun and dont forget to call Zero_grad before backward.
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
    </p>
  </div>
</div>
