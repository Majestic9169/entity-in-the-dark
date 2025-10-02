---
marp: true
lang: en-US
title: Identification Schemes and Entity Authentication
description: Bala Dharnesh, Sai Pragnaan, Tegan Jain
theme: default
paginate: true
style: |
  section {
    background: #181a20;
    color: #eaeaea;
    font-family: 'Fira Mono', 'JetBrains Mono', 'Consolas', 'Liberation Mono', 'Courier New', monospace;
  }
  h1, h2, h3 {
    color: #46c646;
    font-family: inherit;
    border-bottom: 2px solid #3b3e43;
  }
  .terminal-accent {
    color: #8be9fd;
  }
  .box {
    background: #21222c;
    color: #f8f8f2;
    padding: 1.2em 1.8em;
    border-radius: 8px;
    border: 1.5px solid #44475a;
    margin: 1em 0;
  }
  .mono-accent {
    color: #fdbe31;
    font-weight: bold;
  }
  table {
    background: #262626;
    color: #f8f8f2;
    border: 1px solid #44475a;
  }
---

<!-- _class: lead terminal-accent -->
# Identification Schemes `&` Entity Authentication

- Bala Dharnesh  
- Sai Pragnaan  
- Tegan Jain

---

# Table of Contents

1. Identification Schemes
1. Entity Authentication
1. Deception Probabilities
1. References

---

![bg fit](https://img.ifunny.co/images/c507464316caee4e0eeffdc7a5cef1f93ee4a09bd2d77cecae8de6dd1fa5e9f9_1.jpg)

---

# Authentication Codes

An authentication code is a four-tuple $(\mathcal{S, A, K, E})$
- $\mathcal{S}$ is a finite set of possible **source states**
- $\mathcal{A}$ is a finite set of possible **authentication tags**
- $\mathcal{K}$ is a finite set of possible **keys**
- $\mathcal{E}$ is a finite set of possible **authentication rules**

for each $K \in \mathcal{K}$ there is an authentication rule $E_K \in \mathcal{E}$ such that $E_K : \mathcal{S} \to \mathcal{A}$

the message set if defined to be $\mathcal{M} = \mathcal{S} \times \mathcal{A}$

a message $m = (s, a)$ is *valid* under key $K$ if $E_K(s) = a$