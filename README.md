# Challenge-1

### START
def symmetrical_sum(a):
    
    import numpy as np
    
    list_length = len(a)-1
    list_length_Bool = np.array([z==a[list_length-i] for i,z in enumerate(a)])
    list_length_indx = np.where(list_length_Bool==True)[0]
    if len(list_length_indx):
        list_result = a[min(list_length_indx):max(list_length_indx)+1]
    else:
        list_result = []
    return (list_result, sum(list_result))
### END 
