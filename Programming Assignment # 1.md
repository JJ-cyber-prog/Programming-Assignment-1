```python
def alphabet_soup(s):
    sorted_chars = sorted(s)
    sorted_string = ''.join(sorted_chars)
    return sorted_string

print(alphabet_soup("electronics"))  
print(alphabet_soup("engineering"))
print(alphabet_soup("microelectronics"))
```


```python
def emotify(phrase: str):
    words = phrase.split()
    
    if words[-1].lower() == "smile":
        words[-1] = ":)"
    elif words[-1].lower() == "grin":
        words[-1] = ":D"
    elif words[-1].lower() == "sad":
        words[-1] = ":(("
    elif words[-1].lower() == "mad":
        words[-1] = ">:("
        
    new_phrase = ' '.join(words)
    
    return new_phrase

print(emotify("Make me smile"))
print(emotify("Make me grin"))
print(emotify("I am sad"))
print(emotify("I am mad"))
```

    Make me :)
    Make me :D
    I am :((
    I am :((
    
