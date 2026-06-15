# Suspension System Optimization

## Motivation

This project feels very dear to me because this is where it all started.

During COVID, I became fascinated with numerical optimization methods and wanted to apply them to a real engineering problem.

---

## Problem

Designing a suspension involves balancing:

- Ride comfort
- Body roll
- Camber variation
- Stability

The search space is highly coupled and difficult to tune manually.

---

## Approach

I built:

- A double wishbone suspension model
- A dynamic simulation
- A genetic algorithm from scratch
- An objective function combining bounce, roll and camber

![Suspension Model](../images/suspension_model.png)

---

## Challenges

The biggest challenge wasn't coding the genetic algorithm.

It was validating the mathematical model.

Many times the code executed perfectly while the physics was completely wrong.

---

## Results

![Results](../images/ga_results.png)

The optimized design showed significant reductions in:

- Bounce
- Roll
- Vertical acceleration
- Camber variation

---

## Lessons Learned

This project taught me:

- Optimization
- Dynamic simulation
- Debugging mathematical models
- Systems thinking

Most importantly:

You'll never feel fully ready. Learn while building.
