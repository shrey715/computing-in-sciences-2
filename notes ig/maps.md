# Maps

## Introduction

Maps are essentially this relation

$$ x_{n+1} = f(x_{n}) $$

we try and understand the sequence, and its behaviour.

So say the sequence is such that,

$$ x_{n+1} = f(x_{n}) = x_{n}^{2} + c $$

where $c$ is a constant. Let $x_{0}$ be the initial value = 0.

Then the sequence comes out to be,

$$ c, c^{2} + c, (c^{2} + c)^{2} + c, \ldots $$

## Analysis

We study the behaviour of the sequence, as it approaches infinity for example and try to understand if it's asymptotic.

# Logistic Map

The logistic map is a more general form of the above map, where the function is given by

$$ x_{n+1} = f(x_{n}) = rx_{n}(1 - x_{n}) $$

where $r$ is a constant. The sequence is given by,

$$ x_{0}, rx_{0}(1 - x_{0}), r^{2}x_{0}(1 - x_{0})^{2}, \ldots $$

**HOMEWORK:** Show all quadratic maps where ax^2 + bx + c, behave exactly like the logistic map.

