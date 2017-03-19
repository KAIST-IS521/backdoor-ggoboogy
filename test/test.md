# Life is gambling: Coffee betting!

### Description
* This program randomly chooses a **donation angel** who will buy others coffee.
* When we execute this program, it accepts people number who is ready to lose money as a first input. Then, it accepts name of each player, and then returns the name of donation angel along with an apology message.
* This program may be really useful when we go to 'Twosome Place' (this is not a PPL).

* This program tests(uses) all instructions except `ge`.
* People number should be a number, which is equal or larger than 1 and smaller than 10 (`n >= 1 && n < 10`). 
* The length of name should be equal or longer thatn 1 and shorter than 20 (`name.length >= 1 && name.length < 20`).

### pseudocode
```c
#include <stdio.h>

void main(void)
{
    char name[9][20];
    int num = 0, i = 0, result = 0;
    
    puts("<Life is gambling. Coffee betting!>");
    puts("people num : ");
    scanf("%d",&num);
    
    for(i=0; i<num; i++)
        scanf("%s", name[i]);
    
    result = ((int)name[0][0] % num);
    printf("============\n");
    printf("%s\n", name[result]);
    printf("============\n");
    printf("Sorry man~\n");
}
```

### Example of execution result
```
<Life is gambling. Coffee betting!>
people num :
6
moonbeom
soomin
jaeseung
jihyeon
sungil
daramg
============
soomin
============
Sorry man~
```
