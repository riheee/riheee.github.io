---
emoji: 🍉
title: (Codeforces)4A Watermelon
date: '2022-02-22 00:00:00'
author: rihee
tags: rihee algorithm codeforces watermelon
categories: Codeforces
---

Watermelon 원본 문제를 보고 싶으신 분들은 [📝 여기](https://codeforces.com/problemset/problem/4/A)를 클릭해주세요.

If you want to see the original, Click [here](https://codeforces.com/problemset/problem/4/A).

## 1. Translation

### 🔖 본문 내용
>A.	Watermelon
>
>더운 여름날, Pete와 그의 친구 Billy는 수박을 사기로 했다. 그들은 제일 크고, 잘 익은 수박을 골랐다.
> 수박의 무게는 w킬로였다. 그들은 목이 너무 말라서 집으로 달려갔고 수박을 나누기로 했다. 하지만 그들은 어려운 문제에 직면했다.
>
>Pete와 Billy는 짝수를 엄청 좋아해서 **<span style = "color:green">그들은 수박을 두 부분의 무게가 각각 짝수로 나누기를 원한다. 동시에 두 부분이 같지 않아도 된다.<span>**
>그들은 매우 피곤해서 빨리 식사를 시작하고 싶어하기 때문에 당신은 그들을 도와서 알아내야 한다. 그들이 원하는 방식으로 수박을 나눌 수 있는지 없는지.
>물론, 그들은 각각 양수 무게여야한다.

### ✏️ vocabulary
the berry : 열매  
in such a way : 그런 식으로  
in such a way that S + V : ~한 방식으로

## 2. Solution

### 🇰🇷 Korean
위 내용에서 중요한 부분은 `두 사람이 모두 짝수 무게의 수박을 원한다는 것`과 `두 무게가 같지 않아도 된다는 것`이다.

>짝수 + 짝수 = 짝수  
>짝수 + 홀수 = 홀수

그러므로 무게 w는 짝수일 때 조건을 만족하게 됩니다.
다만 숫자 2는 두 부분으로 나누면 홀수 1 + 1이 되기때문에 제외됩니다.  

### 🇬🇧 English

The important things of the above content are `They want to get even number of weight` and `The weights don't have to be equal`.

>even + even  = even  
>odd + odd = odd

So, Weight w must be even number.

However, The number 2 should be excluded because it is result of 1 + 1.  
Weight is unable to be odd number.

## 3. Code

위의 풀이 내용에 따라 작성한 코드는 아래와 같습니다.

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

> 👉  영작, 번역에 틀린 부분이 있다면 댓글 남겨주세요!  
> 😂  Please let me know if I'm wrong in code or english.


```toc

```
