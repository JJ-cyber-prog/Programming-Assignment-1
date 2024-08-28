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
def emotify(sentence):
    emoticons = {
        "smile": "🙂",
        "grin": "😃",
        "sad": "🙁",
        "mad": "😠"
    }
    
    words = sentence.split()
    
    replaced_sentence = ' '.join([emoticons[word] if word in emoticons else word for word in words])
    
    return replaced_sentence

print(emotify("She makes me smile"))  
print(emotify("That classmate makes me mad"))      
print(emotify("Aww, it's okay. Don't be sad"))   
print(emotify("You make me grin"))
```

    She makes me 🙂
    That classmate makes me 😠
    Aww, it's okay. Don't be 🙁
    You make me 😃
    


```python
def unpack_list(lst):
    first, *middle, last = lst
    print(f"first: {first} middle: {middle} last: {last}")

lst = [4, 5, 6, 7, 8, 9]
unpack_list(lst)
```
