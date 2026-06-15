# Self Balancing Robot
I've always found inverted pendulums fascinating. They are simple enough to understand on paper, but difficult enough to expose every weakness in your model, controller, hardware, and assumptions.

This project began as an attempt to build a two-wheeled self-balancing robot from scratch and use it as a platform to learn controls, embedded systems, and eventually reinforcement learning.

I designed and assembled the hardware, integrated the sensors and motor drivers, and developed the software needed to estimate the robot's state in real time. To understand the system properly, I derived its dynamics and performed frequency response analysis to identify the plant characteristics before designing a controller.

The first balancing attempts were far less graceful than the final result. Small errors in sensor calibration, delays in the control loop, and noise in the measurements would quickly cause the robot to oscillate or fall over. Solving these issues taught me more about practical control systems than any textbook could.

Once a stable PID controller was working, I became curious about how modern learning-based methods would compare against classical control. I trained a reinforcement learning policy and deployed it directly onto the physical hardware, using IMU measurements as inputs and motor commands as outputs.

What made the project interesting was not determining whether PID or reinforcement learning was "better," but understanding the strengths and limitations of each approach. Classical control provided predictability and stability, while learning-based approaches offered flexibility but introduced new challenges around robustness and generalization.

This project became a personal playground for exploring the relationship between physics, control theory, embedded systems, and machine learning. It remains one of the projects that most influenced how I think about robotics today.
