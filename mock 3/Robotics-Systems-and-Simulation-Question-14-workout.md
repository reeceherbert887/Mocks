# Simple Exam Guide – Mathematical Modelling (RLC Circuit, v(t) as Output)

# The Main Idea

For these questions you are normally doing ONE thing:

```text
Turn the diagram into equations
```

That is it.

Most exam questions follow the same pattern:

* Mechanical system → use Newton’s Law
* Electrical system → use KVL or KCL

Here we have an **electrical RLC circuit** and we want the **capacitor voltage v(t)**.

---

# PART 1 — Electrical Systems

Usually contains:

* Resistor (R)
* Inductor (L)
* Capacitor (C)

You will normally be asked to find:

```text
Voltage across capacitor v(t)
```

---

# STEP-BY-STEP METHOD

## Step 1 — Write the input and output

```text
Input = u(t)
Output = v(t)
```

---

## Step 2 — Remember the 3 equations

### Resistor

```text
vR(t) = R i(t)
```

### Inductor

```text
vL(t) = L d/dt(i(t))
```

### Capacitor

```text
i(t) = C d/dt(v(t))
```

---

## Step 3 — Apply KVL

KVL means:

```text
All voltages add together
```

So:

```text
u(t) = vR(t) + vL(t) + v(t)
```

---

## Step 4 — Substitute each voltage

From capacitor:

```text
i(t) = C d/dt(v(t))
```

So:

```text
vR(t) = R C d/dt(v(t))
vL(t) = L C d/dt(d/dt(v(t)))
```

---

## Step 5 — Put into KVL

```text
u(t) = R C d/dt(v(t)) + L C d/dt(d/dt(v(t))) + v(t)
```

---

# FINAL ANSWER

```text
L C d/dt(d/dt(v(t))) + R C d/dt(v(t)) + v(t) = u(t)
```

---

# QUICK MEMORY TRICK

```text
Inductor → acceleration of voltage
Resistor → velocity of voltage
Capacitor → voltage
```

So the order is:

```text
Acceleration + Velocity + Position
```