# Quine-fizzbuzz
QuineになっているFizzBuzzプログラム

### 例

出力の`n`が現在のカウント、`r`がfizzbuzzの出力となっている。

```
ruby fizzbuzz.rb
```
```ruby
n=2;r=2;eval(s=%q(puts(%(n=#{n+1};r=#{(n+1)%15==0?"FizzBuzz".dump():(n+1)%3==0?"Fizz".dump():(n+1)%5==0?"Buzz".dump():n+1};eval(s=%q(#{s}))))))
```

n=3の時

```
ruby fizzbuzz.rb | ruby | ruby
```
```ruby
n=3;r="Fizz";eval(s=%q(puts(%(n=#{n+1};r=#{(n+1)%15==0?"FizzBuzz".dump():(n+1)%3==0?"Fizz".dump():(n+1)%5==0?"Buzz".dump():n+1};eval(s=%q(#{s}))))))
```

n=5の時

```
ruby fizzbuzz.rb | ruby | ruby | ruby | ruby
```

n=15の時

```
ruby fizzbuzz.rb | ruby | ruby | ruby | ruby | ruby | ruby | ruby | ruby | ruby | ruby | ruby | ruby | ruby
```
```ruby
n=15;r="FizzBuzz";eval(s=%q(puts(%(n=#{n+1};r=#{(n+1)%15==0?"FizzBuzz".dump():(n+1)%3==0?"Fizz".dump():(n+1)%5==0?"Buzz".dump():n+1};eval(s=%q(#{s}))))))
```
