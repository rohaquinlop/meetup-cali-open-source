---
# try also 'default' to start simple
theme: the-unnamed
# background: https://cover.sli.dev
# some information about your slides, markdown enabled
title: Mi experiencia haciendo Open-Source
# apply any unocss classes to the current slide
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
# drawings:
#   persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-up
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true

# <img src="https://github-readme-stats.vercel.app/api/pin/?username=rohaquinlop&repo=automathon&show_owner=true" width="500" height="300">
---

# Mi experiencia haciendo Open-Source

---
layout: about-me

hello-msg: ¡Hola!
name: Robin Hafid
imageSrc: './imgs/profile-pic.JPG'
job: Security Developer @ Fluid Attacks *
line1: Functional Programming Enthusiast *
line2: Open-Source Contributor *
social1: github.com/sponsors/rohaquinlop
social2: linkedin.com/in/robin-hafid
---

---
layout: center
---

# Proyectos

- [cp-algorithms](https://cp-algorithms.com/)
- [automathon](https://github.com/rohaquinlop/automathon)
- [Rust](https://www.rust-lang.org/es)
- [Makes](https://github.com/fluidattacks/makes)
- [terraform-aws-gitlab-runner](https://github.com/cattle-ops/terraform-aws-gitlab-runner)
- [complexipy](https://github.com/rohaquinlop/complexipy)

---
layout: center
---

# [cp-algorithms](https://cp-algorithms.com/)

#### Algorithms for Competitive Programming

<br>

<img src="/imgs/cp-algorithms.svg" width="500" height="300">

<br>

<v-click>

```diff
- vector<char> is_prime(n+1, true);
+ vector<bool> is_prime(n+1, true);
```

</v-click>

<v-click>

```diff
- return t.substr(bestpos - best + 1, best);
+ return T.substr(bestpos - best + 1, best);
```

</v-click>

---
layout: two-cols
---

# [automathon](https://github.com/rohaquinlop/automathon)

<br>

<img src="/imgs/automathon.svg" width="350" height="200">

![](http://www.r9paul.org/wp-content/uploads/2008/12/nfa_example.jpg)

Imagen tomada de: [r9paul.org](http://www.r9paul.org/blog/2008/nondeterministic-finite-state-machine/)

::right::

<v-click>

```python
from automathon import NFA

## Epsilon Transition is denoted by '' -> Empty string
q = {'q1', 'q2', 'q3', 'q4'}
sigma = {'0', '1'}
delta = {
    'q1' : {
            '0' : {'q1'},
            '1' : {'q1', 'q2'}
            },
    'q2' : {
            '0' : {'q3'},
            '' : {'q3'}
            },
    'q3' : {
            '1' : {'q4'},
            },
    'q4' : {
            '0' : {'q4'},
            '1' : {'q4'},
            },
}
initial_state = 'q1'
f = {'q4'}

automata = NFA(q, sigma, delta, initial_state, f)
```

</v-click>

---
layout: two-cols
---

# [automathon](https://github.com/rohaquinlop/automathon)

![NFA Visualization](https://github.com/rohaquinlop/automathon/assets/50106623/966f4389-7862-4e5f-a5f4-c007c3a836b4)

```python
automata.accept("0000011")   #True
automata.accept("000001")    #False
```


::right::

```python
from automathon import NFA

## Epsilon Transition is denoted by '' -> Empty string
q = {'q1', 'q2', 'q3', 'q4'}
sigma = {'0', '1'}
delta = {
    'q1' : {
            '0' : {'q1'},
            '1' : {'q1', 'q2'}
            },
    'q2' : {
            '0' : {'q3'},
            '' : {'q3'}
            },
    'q3' : {
            '1' : {'q4'},
            },
    'q4' : {
            '0' : {'q4'},
            '1' : {'q4'},
            },
}
initial_state = 'q1'
f = {'q4'}

automata = NFA(q, sigma, delta, initial_state, f)
```

---
layout: center
---

# [Rust](https://www.rust-lang.org/es)

A language empowering everyone
to build reliable and efficient software.

---
layout: center
---

# Contáctame

<br>

Github

<img src="/imgs/qr-code.png" width="300" height="300">
