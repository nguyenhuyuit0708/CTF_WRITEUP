# CRYPTO_TRANING_1
## Các kiến thức toán học đã đáng chú ý 
### Kiến thức về modulo, chia hết và đồng dư
$gcd(a,b) = gcd(b-a,a) = gcd(b$%$a,a)$ với $b >=a$
#### Nghịch đảo modulo
Xét phương trình đồng dư $ax = b \mod m$
khi đó phương trình có nghiệm $x = b*inverse(a)$ trong đó $inverse(a)$ là giá trị mà khi đó $a*inverse(a)=1 \mod m$
#### Cách tìm nghịch đảo modulo bằng thư viện pycryptodome trong python
```python
import pycryptodome
a, m,= 3, 17
d = inverse(a,m)
d = pow(a,-1,m)
```
#### Hệ quả với p là số nguyên tố 
cho 2 số nguyên $a,b$ khi đó ta có 
$(a+b)^p=a^p+b^p \mod p$

## Các lệnh python thường xuyên gặp
### 1. Lệnh assert
Trong python dùng để bắt lỗi theo điều kiện cho trước theo cú pháp:
```python
assert condition
```
chương trình sẽ kiểm tra nếu $condition$ đúng sẽ chạy bình thường còn nếu $condition$ sai sẽ báo lỗi 
### Write up các bài đáng chú ý