import math
d_i = None
d_j = None
d_arr = [ ]#Масив с вершинами
ma_x = 6
print('-----------------------------------------------------------------------')
print('-----------------------------------------------------------------------')
for n in range(5, ma_x+1):
    for m in range(0, int(2**(((n)/2)-1))-1):
        d_arr.append(m)
    print(d_arr)
    # Наглядно выводим значения
    i = 1
    while i <= len(d_arr):
          if i < len(d_arr):
              d_i = d_arr[i-1]
              d_j = d_arr[i]
          else:
              d_i = d_arr[i-1]
              d_j = d_arr[i-i]
          print(d_i,'d_i', end='/')
          print(d_j,'d_j', end=' ')
          print('||', end=' ')
          i += 1
    print(" ")
    print(" ")
    d_arr.clear()
input()
