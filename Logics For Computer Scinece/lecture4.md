## Lecture 4: Polynomial-time Formula Classes


**과목**(Subject): `<CS402>` 전산논리학개론
**교재 범위**(Scope): Lecture Notes Lecture 4
  
  >**ALERT1**: 전산논리학개론 요약 연재는 카이스트 전산논리학개론 교수님이 제공하는 강의 노트를 바탕으로 제작합니다. 강의 노트는 [깃허브 페이지](https://github.com/hongseok-yang/logic24)에서 확인하실 수 있습니다.
  
  >**ALERT2**: 본 문서는 교재에 있는 대부분의 내용을 포함하지만 모든 내용을 포함하지는 않습니다. 모든 내용을 빠짐없이 공부하고 싶은 분들은 교재를 직접 참고하시기 바랍니다.
  
  >**ALERT3**: 카이스트의 수업은 기본적으로 영어 강의이고, 강의 노트도 영어로 되어 있으며 개인적으로도 영어로 된 용어가 더 편하기 때문에 영어로 된 용어가 많이 등장하는 한영 혼용 서술 방식을 채택하고 있습니다. 혹시 불편하신 분들은 양해 부탁드립니다.

  >**TEMPORARY ALERT**: Lecture 2와 3에 해당하는 노트는 아직 준비 중입니다. 가까운 시일 내에 업로드할 예정이오니 조금만 기다려주시면 감사하겠습니다. Lecture 2와 3는 논리학의 매우 기초적인 개념들을 다루고 있으니 궁금하신 분들은 위의 깃허브 페이지에 가셔서 강의 노트나 ppt를 참고해 주십시오.

___  

## Horn Formula
**정의**: 각 절(clause)이 많아야 하나의 positive literal을 포함하는 CNF formula를 **Horn Formula**라고 한다.  
e.g.  
$$
p_1 \land (\lnot p_2 \lor \lnot p_3) \land (\lnot p_1 \lor \lnot p_2 \lor p_4)
$$
는 각 절의 positive literal이 각각 $p_1$, 없음, $p_4$ 뿐이므로, **Horn Formula**이다.  
positive literal이 최대 한 개 뿐이므로, implication form을 이용해 다음과 같이 변형할 수 있다:  
e.g.  
$$
(true \rightarrow p_1) \land (p_2 \land p_3 \rightarrow false) \land (p_1 \land p_2 \rightarrow p_4)
$$  
Horn Formula에 대한 Satisfiability 문제를 Horn-SAT라고 한다. 다음 알고리즘을 사용하면 polynomial-time으로 해결할 수 있다:
> **INPUT**: Horn formula $F$
> $T := \empty$
> **while** $T$ does not satisfy $F$ **do**
> **begin**
>   * pick an unsatisfied clause $p_1 \land \cdots \land p_k \rightarrow G$
>   * **if** $G$ is a variable **then** $T:=T\cup\{G\}$
>   * **if** $G = false $ **then return** `UNSAT`  
> 
> **end**
> **return** $T$

**Q**: $T$가 뭔가요?
**A**: true로 assign된 variable의 집합이다. $A_T$는 이를 바탕으로 한 assignment로, $T$에 속해 있는 variable은 true로 assign하고, 속해 있지 않은 variable은 false로 배정한 것이다. 즉 이 알고리즘은 처음에는 모든 variable을 false로 assign했다가, 이 assignment가 F를 satisfy시킬 때까지, satisfy되지 않은 절을 골라 conclusion 부분이 variable이면 그 variable에 T를 assign하고, false이면 satisfy될 수 없다는 뜻인 `UNSAT`을 return하는 방식으로 작동한다.  
  
**Q**: 어떻게 polynomial-time임을 알 수 있나요?
**A**: while 루프는 T가 F를 만족시킬 때까지 원소를 하나씩 늘리는 방식으로 작동하기 때문에 최대 n번 루프한다. 따라서 formula의 크기에 대해 polynomial-time으로 작동함을 알 수 있다.  
  
**Q**: 이 알고리즘이 옳음을 어떻게 증명할 수 있을까요?
**A**: 알고리즘이 UNSAT이 아닌, T를 return하는 경우에는 루프를 빠져나온 것이므로, $A_T$가 $F$를 satisfy시킴이 자명하다. 알고리즘이 UNSAT을 return하는 경우에 정말로 unsatisfiable인지 증명하기 위해 **Loop Invariant**를 사용한다:
  
  
> For any assignment $\mathcal{B}$ such that $\mathcal{B}\vDash{F}$, $\mathcal{A_T} \le \mathcal{B}$ is a loop invariant.  
>>:O**Reminder - Loop Invariant**: 각 루프 iteration 이전과 이후에 모두 성립하는 성질. 즉, 루프를 해도 계속 유지되는 성질을 뜻한다.
