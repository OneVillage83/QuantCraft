## _Linear Algebra as Risk Geometry_

---

## The Core Idea

Every quantitative model lives in a **space**.

Prices, returns, signals, factors, residuals — all of them are vectors.  
Regression, estimation, and prediction are not algebraic tricks; they are **geometric projections**.

This chapter exists to replace a dangerous misconception:

> _“Linear algebra is about solving equations.”_

In quantitative finance, linear algebra is about:

- **information**
    
- **dimension**
    
- **overlap**
    
- **what cannot be learned from the data**
    

If you misunderstand the geometry, you will misinterpret:

- regression coefficients
    
- factor exposures
    
- diversification
    
- residual risk
    

---

## What a Vector Really Represents

A vector is not “a list of numbers”.

A vector is:

> **a point or direction in an information space**

Examples:

- A return time series → a vector in time space
    
- A factor loading → a direction in risk space
    
- A signal → a projection of data onto a chosen direction
    

When you stack numbers into a vector, you are asserting:

- what dimensions matter
    
- what structure exists
    
- what variation is meaningful
    

This is an assumption — not a fact.

---

## Vector Spaces: The Universe Your Model Lives In

A **vector space** is the set of all combinations you allow.

When you choose:

- features
    
- factors
    
- basis functions
    

you are choosing the **space of explanations** your model is allowed to use.

Anything outside that space:

- cannot be learned
    
- cannot be explained
    
- will appear as noise
    

This is not a limitation of data.  
It is a limitation of **model geometry**.

---

## Basis Choice = Worldview

A basis defines how you describe reality.

Different bases:

- explain the same data
    
- emphasize different structure
    
- hide different risks
    

In finance:

- factor models are basis choices
    
- principal components are basis rotations
    
- signals are hand-crafted basis vectors
    

Changing the basis does not change reality —  
but it changes **what you see**.

---

## Orthogonality: When Things Truly Don’t Interact

Two vectors are orthogonal if they share **no overlap**.

Geometrically:

- orthogonal = independent directions
    
- non-orthogonal = shared information
    

In quant terms:

- orthogonal signals don’t cannibalize each other
    
- non-orthogonal signals double-count risk
    

Most “diversified” strategies are **not orthogonal** —  
they are merely uncorrelated under one regime.

---

## Projection: The Heart of Regression

Projection answers one question:

> _“How much of this vector lies in that space?”_

When you run a regression, you are:

- projecting returns onto a signal space
    
- decomposing outcomes into:
    
    - explained component
        
    - residual component
        

The residual is not “random”.  
It is **everything your model cannot explain**.

Ignoring residual structure is how hidden risk accumulates.

---

## Least Squares as Geometry (Not Optimization)

Least squares does **not** mean:

> “Find coefficients that minimize error.”

Geometrically, it means:

> **Project the data onto the closest point in the model space.**

That space is fixed by:

- your features
    
- your assumptions
    
- your design choices
    

If the space is wrong, the projection will be misleading —  
even if the math is perfect.

---

## Residuals Are Where Risk Lives

The residual vector represents:

- regime effects
    
- nonlinear structure
    
- tail behavior
    
- model misspecification
    

In practice:

- residual variance dominates portfolio risk
    
- residual correlations explode in stress
    
- residuals reveal fragility
    

A model with small residuals in calm markets  
can still fail catastrophically when the space itself is wrong.

---

## Dimensionality: More Is Not Better

Adding dimensions:

- increases flexibility
    
- reduces bias
    
- increases variance
    
- amplifies noise
    

High-dimensional spaces are dangerous because:

- projections become unstable
    
- estimation error dominates signal
    
- geometry becomes ill-conditioned
    

This is why:

- factor models overfit
    
- covariance matrices explode
    
- optimizers behave erratically
    

Dimensionality is **risk**, not capacity.

---

## Information Geometry & Overfitting

Overfitting is not about “too many parameters”.

It is about:

> **projecting onto directions that exist only in noise**

These directions:

- look meaningful in-sample
    
- disappear out-of-sample
    
- reappear as drawdowns
    

Geometrically, you are fitting structure where none exists.

---

## Why This Matters for Portfolios

Portfolios are linear combinations of vectors.

That means:

- diversification is geometric
    
- risk aggregation is geometric
    
- leverage magnifies geometric error
    

If your signals live in overlapping subspaces:

- diversification is an illusion
    
- drawdowns synchronize
    
- correlation spikes surprise you
    

Geometry explains why.

---

## Implementation Notes (Quant Discipline)

When building models:

1. Explicitly define your vector space
    
2. Track basis changes over time
    
3. Monitor residual structure
    
4. Limit dimensionality aggressively
    
5. Treat orthogonality as fragile
    
6. Assume geometry shifts under stress
    

A model that ignores geometry is blind to risk structure.

---

## Common Mistakes

- Treating regression coefficients as causal
    
- Assuming uncorrelated = independent
    
- Adding features without geometric justification
    
- Ignoring residual behavior
    
- Believing “more data fixes geometry”
    

It does not.

---

## Why This Chapter Matters

This chapter reframes linear algebra as:

- **information containment**
    
- **risk structure**
    
- **model limitation**
    

From here forward:

- PCA becomes risk decomposition
    
- covariance becomes geometry
    
- optimization becomes constrained projection
    

This is the lens used on institutional desks — whether they articulate it or not.

---

## Further Reading (Learning Sources)

- MIT OpenCourseWare — 18.06 Linear Algebra
    
- Gilbert Strang — _Introduction to Linear Algebra_
    
- Trefethen & Bau — _Numerical Linear Algebra_
    

(Used for learning and inspiration; content here is original.)

---

## End-of-Chapter Questions (Gate Check)

You should be able to answer:

1. What does a vector represent in a quant system?
    
2. How does a basis choice encode assumptions?
    
3. Why is regression fundamentally a projection?
    
4. Where does risk live after projection?
    
5. Why does higher dimensionality increase fragility?
    

If these answers are unclear, **do not proceed**.