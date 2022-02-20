# Markdown LaTeX

- Reference Websites
  - [마크다운 문법정리2_수식](https://huni0318.github.io/blog/blog-etc/2020-12-21-markdown-tutorial2/)
  - [위키백과:TeX 문법](https://ko.wikipedia.org/wiki/%EC%9C%84%ED%82%A4%EB%B0%B1%EA%B3%BC:TeX_%EB%AC%B8%EB%B2%95)
  - [[LaTex] Markdown 수식 작성법](https://velog.io/@d2h10s/LaTex-Markdown-%EC%88%98%EC%8B%9D-%EC%9E%91%EC%84%B1%EB%B2%95)
  - [[마크다운] LaTex 문법 정리](https://cheris8.github.io/etc/MD-LaTex/)

## 1. Line breaks

### 1-1. Use `\\`

```markdown
$$
f(x)=ax^2+bx+c\\
g(x)=Ax^4
$$
```

$$
f(x)=ax^2+bx+c\\
g(x)=Ax^4
$$

### 1-2. Use Case Symbol

```markdown
$\vert x\vert=
\begin{cases}
-x,\;if\;x<0\\
+x,\;if\;x\geq0
\end{cases}$
```

$\vert x\vert=
\begin{cases}
-x,\;if\;x<0\\
+x,\;if\;x\geq0
\end{cases}$

## 2. Blanks

1. -1 Blank
    - `a\!b`: $a\!b$
2. 0 Blank
    - `ab`: $ab$
3. 1 Blank
    - `a~b`: $a~b$
    - `a\,b`: $a\,b$
    - `a\>b`: $a\>b$
    - `a\;b`: $a\;b$
    - `a\ b`: $a\ b$
3. 4 Blanks
    - `a \quad b`: $a \quad b$
4. 8 Blnaks
    - `a \qquad b`: $a \qquad b$

## 3. Aligned

### 3-1. Left-Aligned: Use `$`

```markdown
$a^2+b^2=c^2$
```

$a^2+b^2=c^2$

### 3-2. Centered-Aligned: Use `$$`

```markdown
$$\int_\Omega \nabla u \cdot \nabla v~dx = \int_\Omega fv~dx$$
```

$$\int_\Omega \nabla u \cdot \nabla v~dx = \int_\Omega fv~dx$$

### 3-3. Sort by '='

1. Use `\begin{aligned} \end{aligned}`

```markdown
$$
\begin{aligned}
f(x)&=ax^2+bx+c\\
g(x)&=Ax^4
\end{aligned}
$$
```

$$
\begin{aligned}
f(x)&=ax^2+bx+c\\
g(x)&=Ax^4
\end{aligned}
$$

2. Use `\begin{matrix} \end{matrix}`

```markdown
$$
\begin{matrix}
f(n+1) &=& (n+1)^2 \\
       &=& n^2 + 2n + 1
\end{matrix}
$$
```

$$
\begin{matrix}
f(n+1) &=& (n+1)^2 \\
       &=& n^2 + 2n + 1
\end{matrix}
$$

## 4. Arithmetic Operations

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Addition|4 + 2 = 2|$4 + 2 = 2$|
|Subtraction|4 - 2 = 2|$4 - 2 = 2$|
|Division|4 \times 2 = 8|$4 \times 2 = 8$|
|Multiplication|4 \div 2 = 2|$4 \div 2 = 2$|

## 5. Root

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Surd|\surd {2}|$\surd {2}$|
|Squared Root|\sqrt {2}|$\sqrt {2}$|

- Surd: In Mathematics, surds are the values in square root that cannot be further simplified into whole numbers or integers. Surds are irrational numbers.

## 6. Factorial

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Factorial|n! = 1 \times 2 \times 3 \times \ldots n|$n! = 1 \times 2 \times 3 \times \ldots n$|
|Factorial|n! = \prod_{k=1}^n k|$n! = \displaystyle\prod_{k=1}^n k$|

## 7. Operators

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Vert|\vert x \vert|$\vert x \vert$|
|Vert|\left\lvert \frac{s^2+1}{s^3+2s^2+3s+1} \right\rvert|$\left\lvert \frac{s^2+1}{s^3+2s^2+3s+1} \right\rvert$|
|Limit|\lim_{x \to \infty} \exp(-x) = 0|$\lim_{x \to \infty} \exp(-x) = 0$|
|Limit|\displaystyle\lim_{s\rarr\infin}{s^2}|$\displaystyle\lim_{s\rarr\infin}{s^2}$|
|sigma|\sum_{i=1}^{10} t_i|$\sum_{i=1}^{10} t_i$|
|Sigma|\displaystyle\sum_{i=1}^{10} t_i|$\displaystyle\sum_{i=1}^{10} t_i$|
|Prod|\prod_{i=1}^N x_i|$\prod_{i=1}^N x_i$|
|Prod|n! = \displaystyle\prod_{k=1}^n k|$n! = \displaystyle\prod_{k=1}^n k$|
|log|\log_b a|$\log_b a$|
|Differential|\frac{df(x)}{dx} = \lim_{x\to0} \frac{f(x+h)-f(x)}{h}|$\frac{df(x)}{dx} = \displaystyle\lim_{x\to0} \frac{f(x+h)-f(x)}{h}$|
|Integral|\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x|$\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x$|
|Integral|\int_{0}^{1}{f(x)dx}|$\int_{0}^{1}{f(x)dx}$|

## 8. Parentheses

1. Common Parentheses
    - `(a+b)`: $(a+b)$
    - `\{a+b\}`: $\{a+b\}$
    - `[a+b]`: $[a+b]$
2. Auto Resizing Parentheses
    - `\left( A \right)`: $\left( A \right)$
    - `\left[ A \right]`: $\left[ A \right]$
    - `\left\{ A \right\}`: $\left\{ A \right\}$
    - `\left\langle A \right\rangle`: $\left\langle A \right\rangle$
    - `\left| A \right|`: $\left| A \right|$
    - `\left. {A \over B} \right\} \to X`: $\left. {A \over B} \right\} \to X$
    - `\lfloor\sqrt{n}\rfloor \lceil\sqrt{n}\rceil`: $\lfloor\sqrt{n}\rfloor \lceil\sqrt{n}\rceil$
3. Manual Resizing Parentheses
    - `\Bigg( A \Bigg)`: $\Bigg( A \Bigg)$
    - `\bigg( A \bigg)`: $\bigg( A \bigg)$
    - `\Big( A \Big)`: $\Big( A \Big)$
    - `\big( A \big)`: $\big( A \big)$
    - `\Bigg( \bigg( \Big( \big( A \big) \Big) \bigg) \Bigg)`: $$\Bigg( \bigg( \Big( \big( A \big) \Big) \bigg) \Bigg)$$

## 9. Dots

|Name|Input Formulas|Rendered Output|
|---|---|---|
|가운데 기준으로 점 표기|\dots|$\dots$|
|가로|\cdots|$\cdots$|
|세로|\vdots|$\vdots$|
|대각선|\ddots|$\ddots$|

## 10. 벡터

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Vector|\overrightarrow{AB}|$\overrightarrow{AB}$|
|Vector|\overline{AB}|$\overline{AB}$|

## 11. 첨자

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Power|a^2|$a^2$|
|Power|a^{2+4}|$a^{2+4}$|
|Indices|a_n|$a_n$|
|Indices|a_{n-1}|$a_{n-1}$|

## 12. Fractions

|Name|Input Formulas|Rendered Output|
|---|---|---|
|Common Fractions|\frac {a}{b}|$\frac {a}{b}$|
|Common Fractions|{a} \over {b}|${a} \over {b}$|
|Fractions in Cooking|^a/_b|$^a/_b$|

## 13. Matrix

|Name|Input Formulas|Rendered Output|
|---|---|---|
|(2x1) 행렬|{n \choose k}|${n \choose k}$|
|(2x2) 행렬 소괄호|\begin{pmatrix} x & y \\ z & v \end{pmatrix}|$\begin{pmatrix} x & y \\ z & v \end{pmatrix}$|
|(2x2) 행렬 중괄호|\begin{Bmatrix} x & y \\ z & v \end{Bmatrix}|$\begin{Bmatrix} x & y \\ z & v \end{Bmatrix}$|
|(2x2) 행렬 대괄호|\begin{vmatrix} x & y \\ z & v \end{vmatrix}|$\begin{vmatrix} x & y \\ z & v \end{vmatrix}$|
|(2x2) 행렬 이중괄호|\begin{Vmatrix} x & y \\ z & v \end{Vmatrix}|$\begin{Vmatrix} x & y \\ z & v \end{Vmatrix}$|
|(2x2) 행렬 無괄호|\begin{matrix} x & y \\ z & v \end{matrix}|$\begin{matrix} x & y \\ z & v \end{matrix}$|

- `bmatrix with (c,v,d)dots` 1

```markdown
$$
\begin{bmatrix}
0 & \cdots & 0 \\
\vdots & \ddots & \vdots \\
0 & \cdots & 0
\end{bmatrix}
$$
```

$$
\begin{bmatrix}
0 & \cdots & 0 \\
\vdots & \ddots & \vdots \\
0 & \cdots & 0
\end{bmatrix}
$$

- `bmatrix with (c,v,d)dots` 2

```markdown
$$A_{m,n} =
 \begin{pmatrix}
  a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
  a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
  \vdots  & \vdots  & \ddots & \vdots  \\
  a_{m,1} & a_{m,2} & \cdots & a_{m,n}
 \end{pmatrix}$$
```

$$
A_{m,n} =
 \begin{pmatrix}
  a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\
  a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\
  \vdots  & \vdots  & \ddots & \vdots  \\
  a_{m,1} & a_{m,2} & \cdots & a_{m,n}
 \end{pmatrix}
$$

## 14. 논문에 자주 나오는 기호

1. **특수문자**

| 이름   | 명령어   | 반환 |      | 이름     | 명령어   | 반환 |
| ------ | -------- | ---- | ---- | -------- | -------- | ---- |
| 알파   | \alpha   | α    |      | 크사이   | \xi      | ξ    |
| 베타   | \beta    | β    |      | 오미크론 | o        | o    |
| 감마   | \gamma   | γ    |      | 파이     | \pi      | π    |
| 델타   | \delta   | δ    |      | 로       | \rho     | ρ    |
| 엡실론 | \epsilon | ϵ    |      | 시그마   | \sigma   | σ    |
| 제타   | \zeta    | ζ    |      | 타우     | \tau     | τ    |
| 에타   | \eta     | η    |      | 입실론   | \upsilon | υ    |
| 세타   | \theta   | θ    |      | 파이     | \phi     | ϕ    |
| 이오타 | \iota    | ι    |      | 카이     | \chi     | χ    |
| 카파   | \kappa   | κ    |      | 오메가   | \omega   | ω    |
| 람다   | \lambda  | λ    |      | 뉴       | \nu      | ν    |
| 뮤     | \mu      | μ    |      |          |          |      |

2. **관계연산자**

| 이름        | 명령어  | 반환 |      | 이름        | 명령어  | 반환 |
| ----------- | ------- | ---- | ---- | ----------- | ------- | ---- |
| 합동        | \equiv  | ≡    |      | 근사        | \approx | ≈    |
| 비례        | \propto | ∝    |      | 같고 근사   | \simeq  | ≃    |
| 닮음        | \sim    | ∼    |      | 같지 않음   | \neq    | ≠    |
| 작거나 같음 | \leq    | ≤    |      | 크거나 같음 | \geq    | ≥    |
| 매우작음    | \ll     | ≪    |      | 매우 큼     | \gg     | ≫    |

3. **논리기호**

| 이름               | 명령어          | 반환 |      | 이름                 | 명령어      | 반환 |
| ------------------ | --------------- | ---- | ---- | -------------------- | ----------- | ---- |
| 불릿               | \bullet         | ∙    |      | 부정                 | \neq        | ≠    |
| wedge              | \wedge          | ∧    |      | vee                  | \vee        | ∨    |
| 논리합             | \oplus          | ⊕    |      | 어떤                 | \exists     | ∃    |
| 오른쪽 </br>화살표 | \rightarrow     | →    |      | 왼쪽 <\br>화살표     | \leftarrow  | ←    |
| 왼쪽 <\br>큰화살표 | \Leftarrow      | ⇐    |      | 오른쪽 <\br>큰화살표 | \Rightarrow | ⇒    |
| 양쪽 <\br>큰화살표 | \Leftrightarrow | ⇔    |      | 양쪽 <\br>화살표     | \leftarrow  | ←    |
| 모든               | \forall         | ∀    |      |                      |             |      |

4. **집합기호**

| 이름         | 명령어      | 반환 |      | 이름       | 명령어                 | 반환 |
| ------------ | ----------- | ---- | ---- | ---------- | ---------------------- | ---- |
| 교집합       | \cap        | ∩    |      | 합집합     | \cup                   | ∪    |
| 상위집합     | \supset     | ⊃    |      | 진상위집합 | \supseteq              | ⊇    |
| 하위집합     | \subset     | ⊂    |      | 진하위집   | \subseteq              | ⊆    |
| 부분집합아님 | \not\subset | ⊄    |      | 공집합     | \emptyset, \varnothing | ∅ ∅  |
| 원소         | \in         | ∈    |      | 원소아님   | \notin                 | ∉    |

5. **기타**

| 이름         | 명령어      | 반환 |      | 이름       | 명령어        | 반환 |
| ------------ | ----------- | ---- | ---- | ---------- | ------------- | ---- |
| 각도          | 90^\circ     | $90^\circ$   |      |     |    |    |
| hat          | \hat{x}     | x^   |      | widehat    | \widehat{x}   | x^   |
| 물결         | \tilde{x}   | x~   |      | wide물결   | \widetilde{x} | x~   |
| bar          | \bar{x}     | x¯   |      | overline   | \overline{x}  | x¯   |
| check        | \check{x}   | xˇ   |      | acute      | \acute{x}     | x´   |
| grave        | \grave{x}   | x`   |      | dot        | \dot{x}       | x˙   |
| ddot         | \ddot{x}    | x¨   |      | breve      | \breve{x}     | x˘   |
| vec          | \vec{x}     | x→   |      | 델,나블라  | \nabla        | ∇    |
| 수직         | \perp       | ⊥    |      | 평행       | \parallel     | ∥    |
| 부분집합아님 | \not\subset | ⊄    |      | 공집합     | \emptyset     | ∅    |
| 가운데 점    | \cdot       | ⋅    |      | …          | \dots         | …    |
| 가운데 점들  | \cdots      | ⋯    |      | 세로점들   | \vdots        | ⋮    |
| 나누기       | \div        | ÷    |      | 물결표     | \sim          | ∼    |
| 플마,마플    | \pm, \mp    | ± ∓  |      | 겹물결표   | \approx       | ≈    |
| prime        | \prime      | ′    |      | 무한대     | \infty        | ∞    |
| 적분         | \int        | ∫    |      | 편미분     | \partial      | ∂    |
| 한칸띄어     | x \, y      | xy   |      | 두칸       | x\;y          | xy   |
| 네칸띄어     | x \quad y   | xy   |      | 여덟칸띄어 | x \qquad y    | xy   |
