# Simple Exam Guide – Mathematical Modelling

# The Main Idea

For these questions you are normally doing ONE thing:

```text
Turn the diagram into equations
```

That is it.

Most exam questions follow the same pattern:

* Mechanical system → use Newton’s Law
* Electrical system → use KVL or KCL

---

# PART 1 — Mechanical Systems

Usually looks like:

* Mass
* Spring
* Damper

Example:

```text
Force → [Mass] -- [Spring] -- [Damper]
```

You will normally be asked to find:

```text
x(t)
```

which is displacement/position.

---

# STEP-BY-STEP METHOD

## Step 1 — Write the input and output

Example:

```text
Input = F(t)
Output = x(t)
```

---

## Step 2 — Remember the 3 equations

### Mass

```text
M d/dt(d/dt(x(t)))
```

Meaning:

```text
Mass × acceleration
```

---

### Damper

```text
B d/dt(x(t))
```

Meaning:

```text
Damping × velocity
```

---

### Spring

```text
Kx(t)
```

Meaning:

```text
Spring force
```

---

## Step 3 — Add everything together

Newton’s Law:

```text
Input force = all opposing forces
```

So:

```text
F(t) = M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t)
```

---

# FINAL ANSWER

```text
M d/dt(d/dt(x(t))) + B d/dt(x(t)) + Kx(t) = F(t)
```

That alone is usually worth most marks.

---

# QUICK MEMORY TRICK

```text
Mass = acceleration
Damper = velocity
Spring = position
```

So the order is:

```text
Acceleration + Velocity + Position
```

---

# PART 2 — Electrical Systems

Usually contains:

* Resistor (R)
* Capacitor (C)
* Inductor (L)

You will normally be asked to find:

```text
Voltage across capacitor vc(t)
```

or:

```text
Current i(t)
```

---

# STEP-BY-STEP METHOD

## Step 1 — Write component equations

### Resistor

```text
v(t) = R i(t)
```

---

### Capacitor

```text
i(t) = C d/dt(v(t))
```

---

### Inductor

```text
v(t) = L d/dt(i(t))
```

---

# STEP 2 — Use KVL

KVL means:

```text
All voltages add together
```

Example:

```text
vin(t) = vR(t) + vL(t) + vc(t)
```

---

# STEP 3 — Replace each voltage with equations

### Resistor

```text
vR(t) = RC d/dt(vc(t))
```

---

### Inductor

```text
vL(t) = LC d/dt(d/dt(vc(t)))
```

---

# STEP 4 — Put into KVL

```text
vin(t) = LC d/dt(d/dt(vc(t))) + RC d/dt(vc(t)) + vc(t)
```

---

# FINAL ANSWER

```text
LC d/dt(d/dt(vc(t))) + RC d/dt(vc(t)) + vc(t) = vin(t)
```

---

# SIMPLE EXAM METHOD

When stuck:

## Mechanical:

```text
1. Write mass equation
2. Write damper equation
3. Write spring equation
4. Add them together
```

---

## Electrical:

```text
1. Write resistor equation
2. Write capacitor equation
3. Write inductor equation
4. Use KVL
5. Substitute everything in
```

---

# EASY THINGS TO REMEMBER

## Mechanical

```text
Mass → acceleration
Damper → velocity
Spring → position
```

---

## Electrical

```text
Resistor → Ri
Capacitor → derivative of voltage
Inductor → derivative of current
```

---

# VERY IMPORTANT EXAM TIP

Even if you cannot finish:

ALWAYS write:

* component equations
* KVL / Newton’s Law
* substitutions

You still get marks for method.

Leaving it blank gets 0.
