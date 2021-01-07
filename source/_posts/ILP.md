---
title: Instruction-Level Parallelism
categories:
- CS
- 컴퓨터 구조 

---

## ILP
- ILP의 핵심은 instruction간의 dependency를 찾는 것이다. 

___
## Instruction 간의 의존성이 있는 경우
- 아래 MIPS 코드를 잘 살펴보면,
```
add $t0 $s1 $s2
add $t1 $t0 $s3
add $t2 $t1 $t0
```

- Line 1과 Line 2가 서로 의존성이 있음을 알 수 있다. 즉, Line2에서는 Line 1의 결과가 나와야만 원하는 연산이 가능하기 때문에 한 번 stall을 해야한다.
