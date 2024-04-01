# Conditional Generative Adversarial Network (CGAN)
## Example 
<details>
  <summary>Click to expand</summary>
- Do you remember the analogy we used in example of GAN. Let's continue with that Generator Team vs Discriminator Team game analogy. Previously, the Generator Team had to create completely random fake data samples like face images without any additional guidance.

- Now, imagine the teams are given an extra rule - the Generator Team has to create specific types of face images based on certain conditions provided to them.

- For example, they may be told to generate a face image of a smiling young woman with blonde hair. Or an elderly man with a beard and glasses. Or a baby with brown eyes and chubby cheeks.

- So in addition to just creating realistic-looking fake face data, the Generator Team now also has to satisfy the conditional requirements given to them for each image they produce.

- The Discriminator Team is also provided these same condition specifications. Their job remains to determine whether each face image presented to them is real from the actual data or a fake generated one. However, they now also get to verify whether the generated fake images adhered properly to the specified conditions.

- This makes the Discriminator Team's job more challenging as they have to scrutinize the images more thoroughly, but it also gives them an additional reference point to detect flaws in the Generator Team's outputs.

- Just like before, both teams continually get feedback and learn from their mistakes over many rounds. The Generator Team finds better ways to not only produce realistic face images but to precisely control attributes like age, expression, hair style etc. per the condition requirements.

- The Discriminator Team in turn gets better at picking up on even subtle inconsistencies between the conditions and the generated fake images.

- What makes cGANs powerful is this ability to generate specific controlled outputs based on the provided conditions, rather than just random data samples. This conditional generation allows for lots of interesting applications.

- For example, a cGAN could be trained on product images and specifications, and then used to generate realistic product images on-demand based on whatever specs are provided like material, color, size etc. This eliminates the need for physical photography in certain cases.

- cGANs could be used to generate synthetic images of human faces matching particular descriptions, which is helpful for fields like security, law enforcement and data privacy protection.

- Overall, by adding conditional control, cGANs take the powerful generative modeling capabilities of standard GANs and make the outputs more specific, controllable and applicable across many domains.
<details>
