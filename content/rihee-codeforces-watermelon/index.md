---
emoji: π
title: (Codeforces)4A Watermelon
date: '2022-02-22 00:00:00'
author: rihee
tags: rihee algorithm codeforces watermelon
categories: Codeforces
---

Watermelon μλ³Έ λ¬Έμ λ₯Ό λ³΄κ³  μΆμΌμ  λΆλ€μ [π μ¬κΈ°](https://codeforces.com/problemset/problem/4/A)λ₯Ό ν΄λ¦­ν΄μ£ΌμΈμ.

If you want to see the original, Click [here](https://codeforces.com/problemset/problem/4/A).

## 1. Translation

### π λ³Έλ¬Έ λ΄μ©
>A.	Watermelon
>
>λμ΄ μ¬λ¦λ , Peteμ κ·Έμ μΉκ΅¬ Billyλ μλ°μ μ¬κΈ°λ‘ νλ€. κ·Έλ€μ μ μΌ ν¬κ³ , μ μ΅μ μλ°μ κ³¨λλ€.
> μλ°μ λ¬΄κ²λ wν¬λ‘μλ€. κ·Έλ€μ λͺ©μ΄ λλ¬΄ λ§λΌμ μ§μΌλ‘ λ¬λ €κ°κ³  μλ°μ λλκΈ°λ‘ νλ€. νμ§λ§ κ·Έλ€μ μ΄λ €μ΄ λ¬Έμ μ μ§λ©΄νλ€.
>
>Peteμ Billyλ μ§μλ₯Ό μμ²­ μ’μν΄μ **<span style = "color:green">κ·Έλ€μ μλ°μ λ λΆλΆμ λ¬΄κ²κ° κ°κ° μ§μλ‘ λλκΈ°λ₯Ό μνλ€. λμμ λ λΆλΆμ΄ κ°μ§ μμλ λλ€.<span>**
>κ·Έλ€μ λ§€μ° νΌκ³€ν΄μ λΉ¨λ¦¬ μμ¬λ₯Ό μμνκ³  μΆμ΄νκΈ° λλ¬Έμ λΉμ μ κ·Έλ€μ λμμ μμλ΄μΌ νλ€. κ·Έλ€μ΄ μνλ λ°©μμΌλ‘ μλ°μ λλ μ μλμ§ μλμ§.
>λ¬Όλ‘ , κ·Έλ€μ κ°κ° μμ λ¬΄κ²μ¬μΌνλ€.

### βοΈ vocabulary
the berry : μ΄λ§€  
in such a way : κ·Έλ° μμΌλ‘  
in such a way that S + V : ~ν λ°©μμΌλ‘

## 2. Solution

### π°π· Korean
μ λ΄μ©μμ μ€μν λΆλΆμ `λ μ¬λμ΄ λͺ¨λ μ§μ λ¬΄κ²μ μλ°μ μνλ€λ κ²`κ³Ό `λ λ¬΄κ²κ° κ°μ§ μμλ λλ€λ κ²`μ΄λ€.

>μ§μ + μ§μ = μ§μ  
>μ§μ + νμ = νμ

κ·Έλ¬λ―λ‘ λ¬΄κ² wλ μ§μμΌ λ μ‘°κ±΄μ λ§μ‘±νκ² λ©λλ€.
λ€λ§ μ«μ 2λ λ λΆλΆμΌλ‘ λλλ©΄ νμ 1 + 1μ΄ λκΈ°λλ¬Έμ μ μΈλ©λλ€.  

### π¬π§ English

The important things of the above content are `They want to get even number of weight` and `The weights don't have to be equal`.

>even + even  = even  
>odd + odd = odd

So, Weight w must be even number.

However, The number 2 should be excluded because it is result of 1 + 1.  
Weight is unable to be odd number.

## 3. Code

μμ νμ΄ λ΄μ©μ λ°λΌ μμ±ν μ½λλ μλμ κ°μ΅λλ€.

```bash
#include<stdio.h>

int main(void)
{
	int input  = 0;
	scanf("%d", &input);
	if(input % 2 == 0 && input != 2)
	{
		printf("YES");
		return 0;
	}
	printf("NO");
	return 0;
}
```


</br>
</br>

> π  μμ, λ²μ­μ νλ¦° λΆλΆμ΄ μλ€λ©΄ λκΈ λ¨κ²¨μ£ΌμΈμ!  
> π  Please let me know if I'm wrong in code or english.


```toc

```
