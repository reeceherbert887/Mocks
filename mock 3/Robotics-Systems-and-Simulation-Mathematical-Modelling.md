# Full Exam Method – Mathematical Modelling (RLC Circuit)

# Universal Method

For these modelling questions, use the same repeatable exam method every time.

---

# Step 1: Identify Input and Output

Write:

```text
Input = u(t)
Output = v(t) (capacitor voltage)
```

---

# Step 2: Identify the System Type

## Electrical System

We have a **series RLC circuit**:

```text
Resistor = R
Inductor = L
Capacitor = C
Input voltage = u(t)
Output voltage = v(t)
```

---

# Step 3: Write Component Equations

## Resistor

```text
vR(t) = R i(t)
```

## Inductor

```text
vL(t) = L d/dt(i(t))
```

## Capacitor

```text
i(t) = C d/dt(v(t))
```

---

# Step 4: Apply KVL Around the Loop

Using Kirchhoff’s Voltage Law:

```text
u(t) = vR(t) + vL(t) + v(t)
```

---

# Step 5: Substitute Component Equations

From capacitor:

```text
i(t) = C d/dt(v(t))
```

### Substitute into resistor:

```text
vR(t) = R C d/dt(v(t))
```

### Substitute into inductor:

```text
vL(t) = L d/dt(C d/dt(v(t)))
```

Which becomes:

```text
vL(t) = L C d/dt(d/dt(v(t)))
```

---

# Step 6: Substitute into KVL

```text
u(t) = R C d/dt(v(t)) + L C d/dt(d/dt(v(t))) + v(t)
```

---

# Step 7: Rearrange into Standard Differential Equation Form

```text
L C d/dt(d/dt(v(t))) + R C d/dt(v(t)) + v(t) = u(t)
```

This is the **final mathematical model**.

---

# Transfer Function Version (Optional)

Take Laplace Transform:

```text
L C s² V(s) + R C s V(s) + V(s) = U(s)
```

Factor:

```text
V(s)(L C s² + R C s + 1) = U(s)
```

Transfer Function:

```text
V(s)/U(s) = 1 / (L C s² + R C s + 1)
```

---

# Easy Exam Structure to Copy

```text
Let the output be v(t).

Step 1 — Write component equations:
Resistor:  vR(t) = R i(t)
Inductor:  vL(t) = L d/dt(i(t))
Capacitor: i(t) = C d/dt(v(t))

Step 2 — Apply KVL:
u(t) = vR(t) + vL(t) + v(t)

Step 3 — Substitute:
vR(t) = R C d/dt(v(t))
vL(t) = L C d/dt(d/dt(v(t)))

Step 4 — Final model:
L C v''(t) + R C v'(t) + v(t) = u(t)
```

---

# Most Important Exam Tip

Even if you cannot fully finish:

```text
- Write component equations
- Write KVL
- Substitute
```

You still get marks for method.

Leaving it blank gets 0.