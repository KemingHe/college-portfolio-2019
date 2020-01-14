---
layout: post
title:  "My CS Toolkit Ep.1: Bounding w/ Integrals"
date:   2020-01-14 12:00:00 -0400
categories: projects
---

<style type="text/css">
.image-right {
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}

.image-left {
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: left;
}

img.shrinked{
	height: 90%;
	width: 90%;
}
</style>

In computer science, we might use [summation notation](https://everythingcomputerscience.com/discrete_mathematics/Summations.html) to represent the [runtime complexity](https://www.geeksforgeeks.org/understanding-time-complexity-simple-examples/) of certain algorithms. Moreover, we might need to bound such summations from above (to obtain [Big-O](https://www.khanacademy.org/computing/computer-science/algorithms/asymptotic-notation/a/big-o-notation)) and below (to obtain [Big-Omega](https://www.khanacademy.org/computing/computer-science/algorithms/asymptotic-notation/a/big-big-omega-notation)).

### Method

<p align="left">
  Given that
  <img alt="Def_of_f(x)" src="../../../../assets/mycsetoolkit_ep1/1. Constraint on f - pt1.png" height="15%" width="15%">
  is monotonically increasing <b>AND</b> integrable on <img alt="Domain_of_f(x)" src="../../../../assets/mycsetoolkit_ep1/1. Constraint on f - pt2.png" height="6%" width="6%">.
  <br><br>
  Suppose we wish to bound…
</p>

<p align="center">
  <img alt="Original_Summation" src="../../../../assets/mycsetoolkit_ep1/2. Ori Summation.png" height="12%" width="12%">
</p>

We’d like to say… (for <b>Big-O</b>)

<p align="center">
  <img alt="Desired_BigO" src="../../../../assets/mycsetoolkit_ep1/3. Desired Big-O.png" height="35%" width="35%">
</p>

…as well as… (for <b>Big-Omega</b>)

<p align="center">
  <img alt="Desired_BigOmega" src="../../../../assets/mycsetoolkit_ep1/4. Desired Big-Omega.png" height="35%" width="35%">
</p>

-- and here’s how we prove that we can bound it in this way.

### Proof

First, we want to prove the following inequality:

<p align="center">
  <img alt="Desired_Inequality" src="../../../../assets/mycsetoolkit_ep1/5. Inequality.png" height="70%" width="70%">
</p>

The math is really confusing, so let’s represent each part geometrically and compare the areas:

<p align="center">
  <img alt="AreaFirst_Second" src="../../../../assets/mycsetoolkit_ep1/Area 1 and 2.png" height="70%" width="70%">
  <br><br>
  <img alt="AreaThird_Fourth" src="../../../../assets/mycsetoolkit_ep1/Area 3 and 4.png" height="70%" width="70%">
</p>

Hope that now you can easily see:

<p align="center">
  <img alt="ProofbyArea" src="../../../../assets/mycsetoolkit_ep1/6. Proof of Inequality.png" height="70%" width="70%">
</p>

Now that we’ve proven the inequality through geometry, time for some simple math!

The left part of the inequality gives us bounding from <b>above</b> (Big-O) using the integral:

<p align="center">
  <img alt="ProofofBigO" src="../../../../assets/mycsetoolkit_ep1/7. Proof of Big-O.png" height="40%" width="40%">
</p>

The right part of the inequality gives us bounding from <b>below</b> (Big-Omega) using the integral:

<p align="center">
  <img alt="ProofofBigOmega" src="../../../../assets/mycsetoolkit_ep1/8. Proof of Big_Omega.png" height="47%" width="47%">
</p>

This concludes our proof of the **Bounding-by-Integral** method.

### Forward

Now that you've understood how to use integrals to bound summations, you might also need tools to help you solve such integrals.

* **Integration by Parts**: _Paul's Online Notes_ has a wonderful turotial on solving integrals such as integrating (x*e^x): [http://tutorial.math.lamar.edu/Classes/CalcII/IntegrationByParts.aspx](http://tutorial.math.lamar.edu/Classes/CalcII/IntegrationByParts.aspx)

* **Integration by Substitution**: _Khan Academy_ has another great article (with practice problems) explaining the u-sub method of solving integrals: [https://www.khanacademy.org/math/ap-calculus-ab/ab-integration-new/ab-6-9/a/review-applying-u-substitution](https://www.khanacademy.org/math/ap-calculus-ab/ab-integration-new/ab-6-9/a/review-applying-u-substitution)

And before we go, welcome to My CS Toolkit! This is my latest blog series, focused on the important skills and tools in **Math** and **Computer Science**. Feel free to connect and comment via my email [he.1537@osu.edu](he.1537@osu.edu), and I'll see you in the next episode!
