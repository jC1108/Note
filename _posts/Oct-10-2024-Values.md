
## Functions
### Trig funs
#### sin(x)
$$ D= [ -\frac{\pi}{2} , \frac{\pi}{2} ] $$ $$ sin(0^\circ) = 0 \;; sin(90^\circ)= 1 $$
#### cos(x)
$$ D= [ {0} , {\pi} ] $$
$$ cos(0^\circ) = 1 \;; cos(90^\circ)= 0 $$
#### tan(x)
$$ D= [ -\frac{\pi}{2} , \frac{\pi}{2} ] $$
$$ tan(0^\circ) = 0 \;; tan(90^\circ)= Undefined $$

#### cot(x)
$$ D= [ {0} , {\pi} ] $$
#### csc(x) -- 1/sin(x)
$$ D= [ -\frac{\pi}{2} , 0) \cup (0,\frac{\pi}{2} ] $$

#### sec(x) -- 1/cos(x)
$$ D= [0,\frac{\pi}{2}) \cup (\frac{\pi}{2},\pi] $$

### Trigh
def:  hyperbolic functions
#### sinh(x)
$$ \sinh(x) = \frac{e^x - e^{-x}}{2} $$

#### cosh(x)
$$ \sinh(x) = \frac{e^x + e^{-x}}{2}$$
#### tanh(x)
$$ \tanh(x) = \frac{\sinh(x)}{\cosh(x)} = \frac{e^x - e^{-x}}{e^x + e^{-x}} $$


### Logarithm
#### log
**log(x), x should be a positive number,** D=(0,∞) 
- log(0): undefined
- log(1): 0
- log(10): 1
- log(100): 2
<br>
#### ln
**log(x), x should be a positive number,** D=(0,∞) 
- ln(0): undefined
- ln(1): 0
- ln(e): 1

## Limits

### Rules

$$ \begin{align*} &\textbf{1. Limit of a Constant:} && \lim_{x \to c} k = k \\ &\textbf{2. Limit of Identity Function:} && \lim_{x \to c} x = c \\ &\textbf{3. Limit of a Sum:} && \lim_{x \to c} [f(x) + g(x)] = \lim_{x \to c} f(x) + \lim_{x \to c} g(x) \\ &\textbf{4. Limit of a Difference:} && \lim_{x \to c} [f(x) - g(x)] = \lim_{x \to c} f(x) - \lim_{x \to c} g(x) \\ &\textbf{5. Limit of a Product:} && \lim_{x \to c} [f(x) \cdot g(x)] = \left( \lim_{x \to c} f(x) \right) \cdot \left( \lim_{x \to c} g(x) \right) \\ &\textbf{6. Limit of a Quotient:} && \lim_{x \to c} \frac{f(x)}{g(x)} = \frac{\lim_{x \to c} f(x)}{\lim_{x \to c} g(x)}, \quad \text{if } \lim_{x \to c} g(x) \neq 0 \\ &\textbf{7. Limit of a Constant Multiple:} && \lim_{x \to c} [k \cdot f(x)] = k \cdot \lim_{x \to c} f(x) \\ &\textbf{8. Limit of a Power:} && \lim_{x \to c} [f(x)]^n = \left( \lim_{x \to c} f(x) \right)^n, \quad \text{for } n \in \mathbb{N} \\ &\textbf{9. Limit of a Root:} && \lim_{x \to c} \sqrt[n]{f(x)} = \sqrt[n]{\lim_{x \to c} f(x)}, \quad \text{if } n \in \mathbb{N} \text{ and } \lim_{x \to c} f(x) \geq 0 \text{ when } n \text{ is even} \end{align*} $$
### Trig Theorem
$$ \begin{align*} &\textbf{1. Limit of } \frac{\sin(x)}{x} \textbf{ as } x \to 0: && \lim_{x \to 0} \frac{\sin(x)}{x} = 1 \\ &\textbf{2. Limit of } \frac{1 - \cos(x)}{x^2} \textbf{ as } x \to 0: && \lim_{x \to 0} \frac{1 - \cos(x)}{x^2} = \frac{1}{2} \\ &\textbf{3. Limit of } \frac{\tan(x)}{x} \textbf{ as } x \to 0: && \lim_{x \to 0} \frac{\tan(x)}{x} = 1 \\ &\textbf{4. Limit of } \frac{\sin(kx)}{x} \textbf{ as } x \to 0: && \lim_{x \to 0} \frac{\sin(kx)}{x} = k \\ &\textbf{5. Limit of } \frac{\sin(x)}{\sin(kx)} \textbf{ as } x \to 0: && \lim_{x \to 0} \frac{\sin(x)}{\sin(kx)} = \frac{1}{k} \end{align*} $$

### Infinity
![[Pasted image 20241004030409.png]]


### Types of Discontinuities

#### 1. Point Discontinuity (Removable Discontinuity)
A function \(f(x)\) has a point discontinuity at \(x = c\) if:
- \(f(c)\) is not defined, or
- $$\lim_{x \to c} f(x)$$ exists, but $$\lim_{x \to c} f(x) \neq f(c)$$.

This type of discontinuity can be "removed" by redefining \(f(c)\) to be equal to $$\lim_{x \to c} f(x)$$.  
**Example:** $$f(x) = \frac{x^2 - 1}{x - 1}$$ at $$x = 1$$

---

#### 2. Jump Discontinuity
A function \(f(x)\) has a jump discontinuity at \(x = c\) if:
- $$\lim_{x \to c^-} f(x) \neq \lim_{x \to c^+} f(x)$$.

This means that the left-hand limit and the right-hand limit exist but are not equal, causing the function to "jump" from one value to another.  
**Example:**
$$
f(x) = 
\begin{cases} 
2 & \text{if } x < 1 \\
3 & \text{if } x \geq 1 
\end{cases}
$$

---

#### 3. Infinite Discontinuity
A function \(f(x)\) has an infinite discontinuity at \(x = c\) if:
- $$\lim_{x \to c} f(x) = \infty$$ or $$\lim_{x \to c} f(x) = -\infty$$.

This type of discontinuity occurs when the function approaches infinity as $$x$$ approaches $$c$$.  
**Example:** $$f(x) = \frac{1}{x}$$ at $$x = 0$$

---

#### 4. Essential Discontinuity
A function \(f(x)\) has an essential discontinuity at \(x = c\) if:
- Neither the left-hand limit nor the right-hand limit exists, or both limits approach different values.

This discontinuity is more complicated and cannot be
