# RegEx XV: Alternation

-   [RegEx XV: Alternation](https://edabit.com/challenge/9ZAHTYWTP5c7FW4RY)

**The vertical bar** `|` is the equivalent to "or" in RegEx. The regular expression `x|y` matches either "x" or "y". Write the **regular expression** that will match all `red flag` and `blue flag` in a string. You must use `|` in your expression. Flags can come in any order.

**Examples**

```
txt1 = "red flag blue flag"
txt2 = "yellow flag red flag blue flag green flag"
txt3 = "pink flag red flag black flag blue flag green flag red flag"
pattern = "yourregularexpressionhere"

re.findall(pattern, txt1) ➞ ["red flag", "blue flag"]
re.findall(pattern, txt2) ➞ ["red flag", "blue flag"]
re.findall(pattern, txt3) ➞ ["red flag", "blue flag", "red flag"]
```

**Notes**

You **don't** need to write a function, just the pattern.
Do **not** remove `import re` from the code.
Find more info on RegEx and alternation in the Resources tab.
You can find all the challenges of this series in my [Basic RegEx](https://edabit.com/collection/8PEq2azWDtAZWPFe2) collection.

**Solution** 

```
import re

pattern = "red flag|blue flag"
```

**Solution 2**  

- [cvf](https://edabit.com/user/yjtdwc2AC4jA2RWtn)

```
import re

pattern = "(?:red|blue) flag"
```