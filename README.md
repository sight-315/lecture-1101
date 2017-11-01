# テクノロジー（藤原） 11/1授業

```
pry
[1] pry(main)> num = 2
=> 2
[2] pry(main)> if num % 2 == 0
[2] pry(main)*   puts "偶数です。"
[2] pry(main)* end
偶数です。
=> nil
[3] pry(main)> num = 1000
=> 1000
[4] pry(main)> if num >= 1500
[4] pry(main)*   puts "送料無料です。"
[4] pry(main)* elsif 0 < num && num < 1500
[4] pry(main)*   puts "送料300円です。"
[4] pry(main)* else
[4] pry(main)*   puts "入力が間違ってます。"
[4] pry(main)* end
送料300円です。
=> nil
[5] pry(main)> num = rand 3
=> 0
[6] pry(main)> case num
[6] pry(main)* when 0
[6] pry(main)*   puts "吉です。"
[6] pry(main)* when 1
[6] pry(main)*   puts "凶です。"
[6] pry(main)* else
[6] pry(main)*   puts "大凶です。"
[6] pry(main)* end
吉です。
=> nil
[7] pry(main)> メソッド (p.66)
SyntaxError: unexpected tINTEGER, expecting '('
メソッド (p.66)
                  ^
[7] pry(main)> PythonやJavaScriptでいう関数と同じ
NameError: uninitialized constant PythonやJavaScriptでいう関数と同じ
from (pry):22:in `__pry__'
[8] pry(main)> p.67の例（三角形の面積・改変）
/usr/local/rvm/gems/ruby-2.4.0@global/gems/method_source-0.9.0/lib/method_source/code_helpers.rb:140:in `===': invalid byte sequence in UTF-8 (ArgumentError)
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/method_source-0.9.0/lib/method_source/code_helpers.rb:140:in `==='
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/method_source-0.9.0/lib/method_source/code_helpers.rb:76:in `rescue in complete_expression?'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/method_source-0.9.0/lib/method_source/code_helpers.rb:80:in `complete_expression?'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_instance.rb:290:in `handle_line'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_instance.rb:243:in `block (2 levels) in eval'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_instance.rb:242:in `catch'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_instance.rb:242:in `block in eval'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_instance.rb:241:in `catch'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_instance.rb:241:in `eval'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/repl.rb:77:in `block in repl'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/repl.rb:67:in `loop'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/repl.rb:67:in `repl'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/repl.rb:38:in `block in start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/input_lock.rb:61:in `__with_ownership'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/input_lock.rb:79:in `with_ownership'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/repl.rb:38:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/repl.rb:13:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/pry_class.rb:192:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/lib/pry/cli.rb:116:in `start'
        from /usr/local/rvm/gems/ruby-2.4.0@global/gems/pry-0.11.1/bin/pry:12:in `<top (required)>'
        from /usr/local/rvm/rubies/ruby-2.4.0/bin/pry:22:in `load'
        from /usr/local/rvm/rubies/ruby-2.4.0/bin/pry:22:in `<main>'
        from /usr/local/rvm/gems/ruby-2.4.0/bin/ruby_executable_hooks:15:in `eval'
        from /usr/local/rvm/gems/ruby-2.4.0/bin/ruby_executable_hooks:15:in `<main>'
sight315:~/workspace $ def triangle(b, h)
bash: syntax error near unexpected token `('
sight315:~/workspace $   result = b * h / 2.0
bash: result: command not found
sight315:~/workspace $   result  # 返り値は最後の1行
bash: result: command not found
sight315:~/workspace $ end
bash: end: command not found
sight315:~/workspace $ 
sight315:~/workspace $ triangle(11, 9)  #=> 49.5
bash: syntax error near unexpected token `11,'
sight315:~/workspace $ triangle 
bash: triangle: command not found
sight315:~/workspace $ pry
[1] pry(main)> def triangle(b, h)
[1] pry(main)*   result = b * h / 2.0  
[1] pry(main)*   result  # 返り値は最後の1行  
[1] pry(main)* end  
=> :triangle
[2] pry(main)> 
[3] pry(main)> triangle(11, 9)  #=> 49.5
=> 49.5
[4] pry(main)> triangle 11, 9
=> 49.5
[5] pry(main)> 
```