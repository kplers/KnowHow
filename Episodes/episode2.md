## 에피소드2: 예산제약

*Budget Cosntraint*
**과목**(Subject): `<BTM210>` 미시경제학  
**교재 범위**(Scope): [B&B]Ch4 [P]Ch4 **[V]Ch2**
  
  >**알림**: 에피소드 2를 포함한 미시경제학 요약 연재는 David A. Besanko, Ronald R. Braeutigam의 Microeconomics 제6판의 한글 번역본 **(B&B)**, Jeffrey M. Perloff, Addison Wesley의 Microeconomics 제8판 원서 **(P)**, Hal R. Varian의 Intermediate Microeconomics: A Modern Approach 제9판 원서 **(V)** 를 바탕으로 했습니다. 모든 교재를 보실 필요는 없고 1~2권만 참고하시면 됩니다.  
  
  >**알림**: 본 문서는 교재에 있는 대부분의 내용을 포함하지만 모든 내용을 포함하지는 않습니다. 모든 내용을 빠짐없이 공부하고 싶은 분들은 교재를 직접 참고하시기 바랍니다.
  
>   
> ## 목차
> ### 1. 예산제약
> #### 재화 개수는 두 개로 충분하다
> ### 2. 예산선과 예산 세트
> * #### 예산 세트의 특징
> * #### 예산선의 변화
> * #### 뉴메레르
> * #### 세금, 보조금, 물량할당
> ### 정리

___
## 예산제약
*Budget Constraint*

* **예산제약**(Budget Constraint): 소비자가 제한된 소득으로 구입할 수 있는 일련의 바구니. 이때 소비자가 선택할 수 있는 재화의 개수들의 묶음을 **소비묶음** (Consumption Basket)이라고 하고, $(x_{1},x_{2})$와 같이 표시한다. 1번 상품을 $x_1$개, 2번 상품을 $x_2$개 소비한다는 뜻. 그냥 $X$라고 표기하기도 한다.
* **예산세트**(Budget Set): 소비자가 선택할 수 있는 모든 소비묶음의 집합.
* **예산선**(Budget Line): 소비자가 자신의 소득을 모두 두 재화에 지출할 경우 구입할 수 있는 재화의 모든 조합. 예산제약의 한계선이라 할 수 있다.
* 예를 들어 소비자 철수가 단 두 개의 재화, 식료품과 의복을 구입한다고 하자. 철수가 매월 구입하는 식료품 단위 수를 $x$, 의복 단위 수를 $y$라 하고 각각의 가격을 $P_x$, $P_y$라 하자. 또, 철수의 매월 소득이 $I$로 고정되어 있다고 하자. 이때 예산제약, 예산세트, 소비묶음, 예산선은 다음과 같다.
  * 예산제약: $P_{x}x+P_{y}y \leq I$
  * 예산세트: $\set{(x, y)|P_{x}x+P_{y}y \leq I}$
  * 소비묶음: $(x, y)$
  * 예산선: $P_{x}x+P_{y}y=I$

### 재화 개수는 두 개로 충분하다.
* 앞선 예시에서 우리는 재화의 개수를 두 개로 제한했다. 그 예시뿐만 아니라 **일반적인 경우에도 재화의 개수를 두 개로 가정**할 수 있는데, 한 개의 재화를 소비자가 소비하고 싶은, 다른 재화가 아닌 모든 재화들을 대표하는 것으로 해석하면 되기 때문이다.
* 이렇게 해석할 때, 다른 모든 재화를 대표하는 재화 2는 **소비자가 다른 재화를 구매하는 데 사용할 수 있는 현금**으로 생각하면 편리하다. 이때 1달러의 가격은 당연히 1달러이므로, $p_2=1$이 된다. 따라서 자연스럽게 예산제약은 $p_1x_1+x_2\leq m$과 같이 된다. 이는 재화 1에 소비하는 돈의 양인 $p_1x_1$에 다른 재화에 소비하는 돈의 양인 $x_2$를 더한 값이 소비하는 돈의 총량인 $m$ 이하여야 한다는 뜻이 된다. 재화 2와 같은 재화를 **복합재**라 한다. 
  * **복합재**(composite good): 관련 예산에서 하나를 제외한 **모든 재화**를 나타내는 추상화.
___
## 예산선과 예산 세트
*Budget Line and Budget Set*

#### 예산 세트의 특징
예산선을 다시 생각해보자. 예산선은 총 가격이 정확히 m인 소비묶음들의 집합이라 할 수 있다. 즉, $p_1x_1+p_2x_2=m$을 만족하는 모든 $x_1,x_2$의 집합이다.
이 식을 $x_2$에 대한 식으로 정리하면 $x_2= {m\over p_2}-{p_1\over p_2}x_1$이 된다. 즉, $x_2$를 세로축, $x_1$을 가로축에 놓는다면 기울기가 $-{p_1\over p_2}$이고 $x_1, x_2$절편이 각각 ${m\over p_1},{m\over p_2}$인 직선이 된다.
그리고 이 직선, 즉 예산선 밑에 있는 모든 소비묶음들의 집합이 **예산 세트**가 된다.
![](https://velog.velcdn.com/images/kplers/post/d6d437f3-324a-4675-a179-f56ffd1b52fb/image.png)

* 예산선을 쉽게 그리는 방법은, 한 재화만 소비한다고 했을 때 얼마나 소비할 수 있는지 생각해보는 것이다. 돈이 $m$만큼 있을 때 가격이 $p_1$인 재화 1만 소비한다면, $m/p_1$만큼 살 수 있을 것이므로, 자연스럽게 $x_1$절편이 $m/p_1$임을 알 수 있다. 마찬가지로 $x_2$절편도 $m/p_2$임을 쉽게 알 수 있으므로 이 두 점을 연결해서 직선을 그리면 된다.
* 예산선의 **기울기**는 재화 1의 소비량이 변화할 때 재화 2의 소비량이 얼마나 변화해야 하는지를 의미한다. 예를 들어 기울기가 -3이라면, 재화 1의 소비량을 1 늘릴 때 총 소비 금액을 유지하려면 재화 2의 소비량을 3 줄여야 한다는 뜻이다.
* 그래서 예산선의 기울기는 재화 1을 소비하는 것의 **기회비용**을 의미한다고 보기도 한다. 재화 1을 더 소비하려면 예산선의 기울기에 따라 재화 2를 포기해야 하기 때문이다.
___
#### 예산선의 변화
* 가격이나 소득이 변화하면 예산선도 변한다.
* **소득이 변화하는 경우**: $m\rarr m' $인 경우, 예산선의 기울기는 소득과 무관하므로 유지되고 $x_1, x_2$절편만 $m'/m$배가 된다. 소득이 증가하는 경우의 변화는 다음과 같다.
![](https://velog.velcdn.com/images/kplers/post/ee9c2ae3-8b7a-4672-b5ff-931173b7d7a3/image.png)

* **가격이 변화하는 경우**: 재화1의 가격이 $p_1 \rarr p'_1$으로 변화한다면, 그와 무관한 $x_2$절편은 유지되고 $x_1$절편이 $p'_1/p_1$배가 되고, 그에 따라 기울기는 $p_1/p'_1$배가 된다. 재화2의 가격이 변화한다면 같은 방법으로 $x_2$절편이 변화할 것이다. 둘 다 변화한다면 두 절편 모두 그에 따라 변화할 것이다. 재화1의 가격이 상승하는 경우의 변화는 다음과 같다.
![](https://velog.velcdn.com/images/kplers/post/87b2b437-1cb6-484b-a26b-cbaf9a2f7a10/image.png)

* 소득과 가격이 모두 변화하는 경우는 두 변화를 차례대로 생각해 보면 쉽게 알 수 있다.
___
#### 뉴메레르
*Numeraire*
예산선은 두 개의 가격과 소득, 총 세 개의 변수로 정의되지만 그 중 하나는 소거할 수 있다. 바로 $p_2=1$ 또는 $m=1$로 고정하면 된다. 이렇게 해도 예산 세트는 변하지 않는다.
즉, $p_1x_1+p_2x_2=m$을,
* ${p_1 \over p_2}x_1+x_2={m\over p_2}$
* ${p_1 \over m}x_1+{p_2 \over m}x_2 = 1$  

로 변형시켜 재화 2의 가격이나 소득을 1로 고정시키는 것이다. 원래 식의 양변에 어떤 수를 나누어서 변형시킨 것이므로 식을 만족시키는 $x_1, x_2$의 집합은 변하지 않는다.  

이때 재화 2의 가격을 1로 고정하는 경우 이를 **뉴메레르 가격**(numeraire price)이라고 한다. 다른 재화의 가격을 측정할 때 기준이 되는 가격을 의미한다. 이렇게 하면 재화 1의 재화 2에 대한 상대 가격 하나만 고려하면 되므로 편리할 수 있다.
___
#### 세금, 보조금, 물량할당
*Taxes, Subsidies, and Rationing*

세금, 보조금, 물량할당과 같은 경제 정책은 소비자의 예산제약에 영향을 줄 수 있다.
* **세금**(Tax)의 경우, 재화의 가격이 상승하는 효과와 같다. **단위당 세금**(Per Unit Tax) 또는 **수량 세금**(Quantity Tax) 의 경우 구매하는 재화 한 단위당 특정량의 세금 $t$을 내야 하는 방식인데, 이 경우 가격이 $p_1 \rarr p_1+t$와 같이 오르는 효과를 낼 것이다. 가치세 (Value Tax)의 경우 재화의 가격에 세금 $\tau$%를 매기는 방식인데, 이 경우에는 가격이 $p_1 \rarr (1+\tau)p_1$와 같이 오르는 효과를 낼 것이다.
* **보조금**(Subsidy)의 경우, 반대로 재화의 가격이 하락하는 효과와 같다. 단위당 s의 **수량 보조금**(Quantity Subsidy)은 $p_1 \rarr p_1-s$, $\sigma$의 가치 보조금 (Ad Valorem Subsidy)는 $p_1 \rarr (1-\sigma)p_1$와 같이 가격이 하락하는 효과를 낼 것이다.
* **정액**(lump-sum) 방식의 세금이나 보조금의 경우는 소비자의 행위에 관계없이 특정량의 세금을 걷거나 보조금을 주는 것으로, 이 경우 소득이 감소하거나 증가하는 효과와 같다.
* **물량할당**(rationing) 정책은 특정 재화의 소비량을 일정 수준 이하로 제한하는 정책이다. 만약 정부가 소비자 한 명당 재화 1을 $\bar{x_1}$로 제한했다면 아래 그림과 같이 예산 세트에서 $x_1>\bar{x_1}$인 구역이 잘려나갈 것이다.
![](https://velog.velcdn.com/images/kplers/post/3f3dcfc7-363a-4fe2-abc1-7f1f031b1c48/image.png)

* 세 정책이 혼합된 경우도 있다. 예를 들어 재화 1을 $\bar{x_1}$ 이상 구입하면 초과분에 대해 세금을 부과하는 경우, 아래 그림과 같이 $x_1>\bar{x_1}$인 구역에서 가격이 오르는 효과가 생기므로, 기울기가 가파라질 것이다.
![](https://velog.velcdn.com/images/kplers/post/e479575c-39f1-47d8-ba2f-8dc512a0f44d/image.png)



___

## 정리
이번 에피소드에서는 예산제약과 예산선 등을 분석해 보았다. 주요 용어를 살펴보며 마무리하도록 하자. 
* 예산제약
* 예산선
* 예산 세트
* 소비묶음
* 세금
* 보조금
* 뉴메레르 가격
* 물량할당


다음 에피소드에서는 선호(Preference)와 효용(Utility)에 대해 다룰 예정이다. 이번 에피소드에서 배운 예산제약, 예산선의 개념도 쓰일 예정이니 잘 복습해 두도록 하자.

