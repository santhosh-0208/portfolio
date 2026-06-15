# Adaptive Assembly

This project started from a question I kept running into while working with industrial robots: how do you make a robot reliably complete an assembly task when the world is never exactly as expected?

Traditional industrial automation works brilliantly when everything is fixtured and repeatable. But even small position errors can cause insertion tasks to fail. Humans naturally compensate using vision and touch; robots need to learn to do the same.

I wanted to explore how vision and force sensing could be combined to create more robust assembly behavior.

The system consisted of three main components. First, an image-based visual servoing pipeline continuously estimated alignment errors using camera feedback. Second, a virtual force-torque sensor estimated interaction forces from joint torque sensor measurements. Finally, a sensor fusion layer combined both sources of information to generate a more reliable estimate of the assembly state.

One of the biggest lessons from this project was understanding the tradeoffs between sensing modalities. Vision provides rich information but can be noisy and delayed. Force feedback is immediate and highly informative during contact but tells you very little before contact occurs. Getting both systems to complement each other required thinking carefully about timing, confidence, and failure modes.

This project also introduced me to a recurring theme in robotics: the best solution is often not choosing between two approaches, but finding a way for them to work together.

Looking back, this project was my first serious exploration into the intersection of perception, control, and robot learning. It pushed me to think beyond individual algorithms and start designing complete robotic systems.
