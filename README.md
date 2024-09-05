This is my submission for the First Programming Assignment. The code demonstrates the implementation of algorithms to solve the given problem.


def alphabet_soup(s):
    sorted_chars = sorted(s)
    sorted_string = ''.join(sorted_chars)
    return sorted_string

print(alphabet_soup("electronics"))  
print(alphabet_soup("engineering"))
print(alphabet_soup("microelectronics"))


def emotify(phrase: str):
    words = phrase.split()
    
    if words[-1].lower() == "smile":
        words[-1] = ":)"
    elif words[-1].lower() == "grin":
        words[-1] = ":D"
    elif words[-1].lower() == "sad":
        words[-1] = ":D"
    elif words[-1].lower() == "mad":
        words[-1] = ":D"
        
    new_phrase = ' '.join(words)
    
    return new_phrase

print(emotify("Make me smile"))
print(emotify("Make me grin"))
print(emotify("I am sad"))
print(emotify("I am sad"))


def separation(arr):
    if len(arr) < 2:
        print("Array must have two elements")
        
    first = arr[0]
    middle = arr[1:-1]
    last = arr[-1]
    
    print(f"First: {first}")
    print(f"Middle: {middle}")
    print(f"Last: {last}")
    
list = [8, 1, 2, 3, 5, 6, 7, 4]
separation(list)
