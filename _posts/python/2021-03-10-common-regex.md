---
title: Hello world! for Regex
toc: true
comments: true
layout: post
description: Pinch of regex is what you need when writing a preprocessing code for ML
categories: [Python]
---

## Commonly used regex for data preprocessing

1.  Adding a space before a punctuation if it is not already spaced.

```python
import re

ex_str = 'This house is very old.'
ex_str = re.sub(r"([?.!,])", r" \1 ", ex_str)
ex_str = re.sub(r'[" "]+', " ", ex_str)
ex_str = re.sub("[^a-zA-Z?.!]+". " ", w)
ex_str = ex_str.strip()
print(ex_str)
```

2.  Identifiers
    1.  `*`
    2.  `.`
    3.  `+`
    4.  `?`
    5.  `[]`
    6.  `\1`
    7.  `.*`
    8.  `.+`
    9.  `.?`
    10.
