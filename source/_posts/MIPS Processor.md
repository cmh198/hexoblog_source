---
title: MIPS Processor
categories:
- CS
- 컴퓨터 구조

tag:
- MIPS

---

## MIPS Processor의 원리
- MIPS 프로세서에서 Instruction을 실행하는 과정은 크게 5 Stage가 있다.
```
IF -> ID -> EX -> MEM -> WB
```

- IF: Instruction Fetch 메모리(DRAM)으로부터 Instruction 한 줄(32bit)을 가져온다.
- ID: Instruction Decode 가져온 Instruction을 Decode하고 레지스터로부터 값을 가져온다.
- EX: Execute 레지스터로부터 가져온 값으로 연산을 한다.
- MEM: Memory Write 메모리로부터 데이터를 불러오거나 저장하는 작업을 한다 EX. lw, sw
- WB: Write Back 연산을 끝낸 값을 저장할 레지스터에 접근하여 레지스터에 값을 저장한다.

## Instruction의 종류
1. R-Format
- 
2. I-Format
- 
3. J-Format
- 