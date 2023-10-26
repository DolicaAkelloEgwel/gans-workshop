---
marp: true
---

# GANs with Python

---

# Setup

1. Go to this link: **bit.ly/45svhk0**
2. Log in to your Google account

If you got some of your own files then...
1. Create a folder called `gans-workshop-files` in the top level of your Google Drive folder
2. Within that folder create another folder for your images. This can be named cats/trees/flowers/etc.

---

# What are GANs?

- Generative Adversarial Networks (GANs)
- Two neural networks trained simultaneously
- A Generator ("the criminal") is trying to learn to create fake images
- A Discriminator ("the detective") is trying to tell real images from the fake images
- They help make the other better at their job

---

<style>
img[alt~="center"] {
  display: block;
  margin: 0 auto;
}
</style>

![w:900 center](./presentation-images/generator-discriminator.png)

<!--
- The Criminal starts with "random data." This would be like drawing random images on a piece of paper while blindfolded.
- The Detective is presented with a real bank note and a fake note, and has to say which one it thinks is real.
- If the Detective can tell that they money is fake then the Criminal goes away and tries to get better at making fake money. The Detective got it right, so it doesn't change its behaviour.
- If the Detective can't tell that the counterfeit money is fake, then it tries to get better at spotting fake money. The Criminal doesn't change its behaviour because it was successful.
- After enough repetitions of this, we obtain "convergence" when the Criminal's fake money becomes so convincing that the Detective gives up on trying to tell what's what. All it can do is say there's a 50/50 chance because it's stumped.
 -->

---

# MNIST Dataset

![w:500 center](./presentation-images/mnist.gif)

---

# This Person Does Not Exist

![w:500 center](./presentation-images/doesnt-exist.jpg)

---

# This Person Should Not Exist

![h:350 center](./presentation-images/should-not-exist.png)

---
# Loss Functions

Our loss functions allows us to see how well the Generator and Discriminator are doing.

$D(x)$ measures how confident the Discriminator is that a real image is authentic.
$D(G(z))$ measures how confidence the Discriminator is that a fake image is authentic.

|   | $D(x)$  | $D(G(z))$  |
|---|---|---|
| The Discriminator wants this value to approach...  | 1  | 0 |
| The Generator wants this value to approach...  |   | 1  |

---
# Mathematical Optimisation

GANs are based on the maths of optimisation. The objective of optimisation is to find the best solution to problem.

![h:350 center](./presentation-images/optimisation.png)

Our aim here is to