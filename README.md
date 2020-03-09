# python puzzles

#Given a string, we'll say that the front is the first 3 chars of the string. If the string length is less than 3, the front is whatever is there. Return a new string which is 3 copies of the front.#

def front3(str):
  if len(str) <= 3:
    return (str+str+str)
  elif len(str) >= 3:
    def split(word):
      return list(word)
    word = str
    li = word[0:3]
    return (li+li+li)
    
#Given an int n, return the absolute difference between n and 21, except return double the absolute difference if n is over 21.#

def diff21(n):
  if n <= 21:
    return 21 - n
  elif n > 21:
    return 2*(abs(21-n))   
    
#Given a string, return a new string where the first and last chars have been exchanged.#
    
def front_back(str):
  if len(str) <=1 :
    return str
  else:
    return str[-1:] + str[1:-1] + str[:1]    
