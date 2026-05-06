# Full Exam Method – Mathematical Modelling

# Universal Method

For these modelling questions, use the same repeatable exam method every time.

---

# Step 1: Identify Input and Output

Write:

```text
Input = applied force / voltage / current
Output = required variable, e.g. x(t), vc(t), speed, angle
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

Use Newton’s Second Law:

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
v(t) = R i(t)
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

Example:

```text
vin(t) = vR(t) + vL(t) + vc(t)
```

---

# Capacitor Current

```text
i(t) = C d/dt(vc(t))
```

---

# Resistor Voltage

```text
vR(t) = R i(t)
```

Substitute current:

```text
vR(t) = RC d/dt(vc(t))
```

---

# Inductor Voltage

```text
vL(t) = L d/dt(i(t))
```

Substitute capacitor current:

```text
vL(t) = LC d/dt(d/dt(vc(t)))
```

---

# Substitute Into KVL

```text
vin(t) = LC d/dt(d/dt(vc(t))) + RC d/dt(vc(t)) + vc(t)
```

Final Model:

```text
LC d/dt(d/dt(vc(t))) + RC d/dt(vc(t)) + vc(t) = vin(t)
```

---

# Transfer Function

Take Laplace Transform:

```text
Vin(s) = LCs²Vc(s) + RCsVc(s) + Vc(s)
```

Factor out Vc(s):

```text
Vin(s) = Vc(s)(LCs² + RCs + 1)
```

Transfer Function:

```text
Vc(s)/Vin(s) = 1 / (LCs² + RCs + 1)
```

---

# Easy Exam Structure to Copy

## Mechanical System

```text
Let the output be x(t).

Using Newton’s Second Law:

Sum of forces = M d/dt(d/dt(x(t)))

The spring force is Kx(t)
The damping force is B d/dt(x(t))

Therefore:

F(t) = M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t)

Rearranging:

M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t) = F(t)
```

---

# Electrical System

```text
Let the output be vc(t).

Using KVL:

vin(t) = vR(t) + vL(t) + vc(t)

For the capacitor:

i(t) = C d/dt(vc(t))

For the resistor:

vR(t) = R i(t) = RC d/dt(vc(t))

For the inductor:

vL(t) = L d/dt(i(t)) = LC d/dt(d/dt(vc(t)))

Therefore:

vin(t) = LC d/dt(d/dt(vc(t))) + RC d/dt(vc(t)) + vc(t)

Final model:

LC d/dt(d/dt(vc(t))) + RC d/dt(vc(t)) + vc(t) = vin(t)
```

---

# Most Important Exam Tip

Even if you cannot fully finish:

ALWAYS write:

```text
- component equations
- Newton’s Law / KVL / KCL
- substitutions
```

You still get marks for method.

Leaving it blank gets 0.
