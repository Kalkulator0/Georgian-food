# Georgian-food
The code was written on: 30.01.26
```Python
import random

class Georgian:
    def __init__(self):
        self.khinkali = random.randint(1, 30)
        self.khachapuri = random.randint(1, 20)
    
    def eat(self, what):
        if what == "khinkali":
            if self.khinkali > 0:
                self.khinkali -= 1
                print(f"khinkali left: {self.khinkali}, and 1 eaten")
            elif self.khinkali < 0:
                print("Hey, no khinkali!")
                
        elif what == "khachapuri":
            if self.khachapuri > 0:
                self.khachapuri -= 1
                print(f"khachapuri left: {self.khachapuri}, and 1 eaten")
            elif self.khachapuri < 0:
                print("Hey, no khachapuri!")
        else:
            print("We only have khinkali and khachapuri")
