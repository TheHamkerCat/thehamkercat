# TheHamkerCat (ダハムカーキャット)
### Hey there <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="25px">
<!-- Zero width character is used to put extra blank lines before and after code -->

<h3>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple[str, ...] = (".Py", ".C", ".Sh", ".HTML", ".CSS")
    misc        : tuple[str, ...] = ("Linux", "FastAPI", "Pyrogram")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```
</h3>
