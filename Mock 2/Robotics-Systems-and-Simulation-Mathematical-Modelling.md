# Full Exam Method – Mathematical Modelling (Mock 2)

# Universal Method

For these modelling questions, use the same repeatable exam method every time.

---

# Step 1: Identify Input and Output

Write:

```text
Input = applied force / voltage / current
Output = required variable, e.g. x(t), vR(t), vc(t)
```

---

# Step 2: Identify the System Type

## Mechanical Systems

Usually contains:

```text
Mass = M
Damper = B
Spring = K
Input force = F(t)
Output displacement = x(t)
```

---

## Electrical Systems

Usually contains:

```text
Resistor = R
Capacitor = C
Inductor = L
Input = voltage/current source
Output = required voltage/current
```

---

# Mechanical Modelling Example

For a mass-spring-damper system:

```text
Input force = F(t)
Output displacement = x(t)
```

Use Newton's Second Law:

```text
Sum of forces = Mass × acceleration
```

---

# Mechanical Component Equations

## Spring Force

```text
Kx(t)
```

---

## Damper Force

```text
B d/dt(x(t))
```

---

## Mass Force

```text
M d/dt(d/dt(x(t)))
```

---

# Add All Forces Together

```text
F(t) = M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t)
```

Final Answer:

```text
M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t) = F(t)
```

---

# Transfer Function Version

Take Laplace Transform:

```text
Ms²X(s) + BsX(s) + KX(s) = F(s)
```

Factor out X(s):

```text
X(s)(Ms² + Bs + K) = F(s)
```

Transfer Function:

```text
X(s)/F(s) = 1 / (Ms² + Bs + K)
```

---

# Electrical Modelling Method

Use these component equations.

---

# Resistor

```text
vR(t) = R i(t)
```

---

# Capacitor

```text
i(t) = C d/dt(v(t))
```

---

# Inductor

```text
v(t) = L d/dt(i(t))
```

---

# Series Circuit Method

Use KVL:

```text
Input voltage = sum of voltages across components
```

Example for series RC (no inductor):

```text
V(t) = vR(t) + vC(t)
```

---

# Capacitor Current

```text
i(t) = C d/dt(vC(t))
```

---

# Resistor Voltage

```text
vR(t) = R i(t)
```

Substitute current:

```text
vR(t) = RC d/dt(vC(t))
```

---

# When Output is vR(t) — Extra Step

Because the output is vR(t) not vC(t), you need to eliminate vC(t).

Rearrange KVL to get vC(t):

```text
vC(t) = V(t) - vR(t)
```

Then substitute into the resistor equation:

```text
vR(t) = RC d/dt(V(t) - vR(t))
```

Expand:

```text
vR(t) = RC d/dt(V(t)) - RC d/dt(vR(t))
```

Rearrange:

```text
RC d/dt(vR(t)) + vR(t) = RC d/dt(V(t))
```

---

# Final Model (Series RC, Output = vR(t))

```text
RC d/dt(vR(t)) + vR(t) = RC d/dt(V(t))
```

---

# Transfer Function

Take Laplace Transform:

```text
RCsVR(s) + VR(s) = RCsV(s)
```

Factor out VR(s):

```text
VR(s)(RCs + 1) = RCsV(s)
```

Transfer Function:

```text
VR(s)/V(s) = RCs / (RCs + 1)
```

---

# Easy Exam Structure to Copy

## Mechanical System

```text
Let the output be x(t).

Using Newton's Second Law:

Sum of forces = M d/dt(d/dt(x(t)))

The spring force is Kx(t)
The damping force is B d/dt(x(t))

Therefore:

F(t) = M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t)

Rearranging:

M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t) = F(t)
```

---

# Electrical System — Series RC, Output = vR(t)

```text
Let the output be vR(t).

Step 1 — Write component equations:

Capacitor:  i(t) = C d/dt(vC(t))
Resistor:   vR(t) = R i(t)

Step 2 — Apply KVL:

V(t) = vR(t) + vC(t)

Step 3 — Substitute capacitor current into resistor equation:

vR(t) = RC d/dt(vC(t))

Step 4 — Express vC(t) from KVL:

vC(t) = V(t) - vR(t)

Step 5 — Substitute into resistor equation:

vR(t) = RC d/dt(V(t) - vR(t))

Step 6 — Expand:

vR(t) = RC d/dt(V(t)) - RC d/dt(vR(t))

Step 7 — Rearrange:

RC d/dt(vR(t)) + vR(t) = RC d/dt(V(t))

Final model:

RC d/dt(vR(t)) + vR(t) = RC d/dt(V(t))
```

---

# Most Important Exam Tip

Even if you cannot fully finish:

ALWAYS write:

```text
- component equations
- Newton's Law / KVL / KCL
- substitutions
```

You still get marks for method.

Leaving it blank gets 0.