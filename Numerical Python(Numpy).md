# Numerical Python(Numpy)

##  1. 개념

- 행렬이나 일반적으로 대규모 다차원 배열을 쉽게 처리 할 수 있도록 지원하는 파이썬의 라이브러리이다. Numpy는 데이터 구조 외에도 수치 계산을 위해 효율적으로 구현된 기능을 제공한다.

  

- 'import' 하여 사용

```python
import numpy as np
```



- 치트시트를 보고 하면 편하다

[치트시트](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf)



## 2. Numpy Dimensional array

```python
a = np.array([1,4,5,8], float)
print(a)
```

```python
array([1., 4., 5., 8.])
```



## 3. Array shape

### Array

- Vector(1차원)

``` python
vector = np.array([1,4,5,8])
```



- Matrix(2차원)

```python
matrix = np.array([[1,2,3], [4,5,16]])
```



- Tensor(3차원)

```python
tensor = np.arange(1,25).reshape(2,3,4)
```



### shape / reshape / flatten

- .shape 으로 array의 형태 확인 가능

```python
matrix.shape
```

```python
(2, 3)
```



- .reshape() 으로 형태 변환 가능

```python
matrix.reshape(6,)   # (2, 3) 2차원 행렬을 1차원 행렬로 변환
```



- .flatten 말 그대로 1차원 행렬로 만들어준다

```python
tensor.flatten()
```

```python
array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24])
```



## 4. Indexing & Slicing

### Indexing

- 여러 방법이 있음

```python
matrix[0][1]
matrix[0,1]
tensor[1,1,2]
```



###  slicing

- 원하는 부분 쏙 빼오기 (파이썬은 이게 한줄에 됨)

```python
# 예시 행렬
array([[ 0,  1,  2,  3],
       [ 4,  5,  6,  7],
       [ 8,  9, 10, 11],
       [12, 13, 14, 15]])  
```

```python
b[1:3, 1:3]
```

```python
array([[ 5,  6],
       [ 9, 10]])
```



```python
b[::2, 1::2]   # 주기가 2
```

```python
array([[ 1,  3],
       [ 9, 11]])
```

